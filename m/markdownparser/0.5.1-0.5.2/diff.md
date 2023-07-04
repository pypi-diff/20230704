# Comparing `tmp/markdownparser-0.5.1.tar.gz` & `tmp/markdownparser-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdownparser-0.5.1.tar", max compression
+gzip compressed data, was "markdownparser-0.5.2.tar", max compression
```

## Comparing `markdownparser-0.5.1.tar` & `markdownparser-0.5.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 markdownparser-0.5.1/LICENSE
--rw-r--r--   0        0        0       92 2023-06-06 07:15:33.183694 markdownparser-0.5.1/MarkdownParser/__init__.py
--rw-r--r--   0        0        0     5798 2023-04-28 16:45:24.751198 markdownparser-0.5.1/MarkdownParser/base_class.py
--rw-r--r--   0        0        0    23723 2023-06-07 17:45:16.263585 markdownparser-0.5.1/MarkdownParser/block_parser.py
--rw-r--r--   0        0        0     6831 2023-06-07 17:43:22.492464 markdownparser-0.5.1/MarkdownParser/core.py
--rw-r--r--   0        0        0     3329 2023-04-28 12:24:15.406020 markdownparser-0.5.1/MarkdownParser/preprocess_parser.py
--rw-r--r--   0        0        0    21511 2023-05-24 14:55:53.230047 markdownparser-0.5.1/MarkdownParser/tree_parser.py
--rw-r--r--   0        0        0      442 2023-06-07 17:47:12.001165 markdownparser-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     4743 2023-06-07 17:14:23.962993 markdownparser-0.5.1/README.md
--rw-r--r--   0        0        0     5516 1970-01-01 00:00:00.000000 markdownparser-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2022-12-05 18:27:07.136320 markdownparser-0.5.2/LICENSE
+-rw-r--r--   0        0        0       92 2023-06-06 07:15:33.183694 markdownparser-0.5.2/MarkdownParser/__init__.py
+-rw-r--r--   0        0        0     5714 2023-07-04 02:43:15.157813 markdownparser-0.5.2/MarkdownParser/base_class.py
+-rw-r--r--   0        0        0    24198 2023-07-04 02:42:34.319849 markdownparser-0.5.2/MarkdownParser/block_parser.py
+-rw-r--r--   0        0        0     6816 2023-07-04 02:43:23.168362 markdownparser-0.5.2/MarkdownParser/core.py
+-rw-r--r--   0        0        0     3294 2023-07-04 02:43:24.968451 markdownparser-0.5.2/MarkdownParser/preprocess_parser.py
+-rw-r--r--   0        0        0    21725 2023-07-04 02:43:27.560920 markdownparser-0.5.2/MarkdownParser/tree_parser.py
+-rw-r--r--   0        0        0      442 2023-07-04 02:43:51.562365 markdownparser-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0     4743 2023-07-04 02:30:14.376256 markdownparser-0.5.2/README.md
+-rw-r--r--   0        0        0     5516 1970-01-01 00:00:00.000000 markdownparser-0.5.2/PKG-INFO
```

### Comparing `markdownparser-0.5.1/LICENSE` & `markdownparser-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.1/MarkdownParser/base_class.py` & `markdownparser-0.5.2/MarkdownParser/base_class.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 import re
 
 
 class Container:
     # 用于记录全局解析时的中间变量替换
 
     def __init__(self) -> None:
@@ -11,187 +10,167 @@
             #
         }
 
         self._counter = 0
         self.__str__ = self.__repr__
 
     def __repr__(self) -> str:  # pragma: no cover
-
-        split_line = '-' * 50 + '\n'
-        info = f'Total number: {self._counter}\n\n'
+        split_line = "-" * 50 + "\n"
+        info = f"Total number: {self._counter}\n\n"
 
         for k, v in self._container.items():
-            info += f'[{k}]'.ljust(30)
-            if v.input.get('word') is not None:
-                info += ' < word = ' + v.input['word'] + ' >'
-            info += '\n'
+            info += f"[{k}]".ljust(30)
+            if v.input.get("word") is not None:
+                info += " < word = " + v.input["word"] + " >"
+            info += "\n"
         return split_line + info + split_line
 
     def __getitem__(self, key):
         return self._container.get(key, None)
 
     def register(self, class_object):
-        _name = f'{class_object.__class__.__name__}-{str(self._counter)}'
+        _name = f"{class_object.__class__.__name__}-{str(self._counter)}"
         self._counter += 1
         self._container[_name] = class_object
-        return '{-%' + _name + '%-}'
+        return "{-%" + _name + "%-}"
 
 
 CONTAINER = Container()
 
 
 class Parser:
-
     def __init__(self) -> None:
         self._handlers = []  # 保存所有注册的方法
         self.is_sorted = False
 
     def _sort(self):
-
         # 按照优先级从高到低排序,使得解析时依次调用方法
-        self._handlers.sort(key=lambda item: item['priority'], reverse=True)
+        self._handlers.sort(key=lambda item: item["priority"], reverse=True)
 
     def __call__(self, *args, **kwargs):  # pragma: no cover
-
         raise NotImplementedError
 
     def info(self):  # pragma: no cover
         # 查看所有已注册的方法
         if not self.is_sorted:
             self._sort()
         for method in self._handlers:
-            name = method['name']
-            class_name = method['object'].__class__.__name__
-            priority = method['priority']
-            print(f'[{name}]({priority}) : {class_name}')
+            name = method["name"]
+            class_name = method["object"].__class__.__name__
+            priority = method["priority"]
+            print(f"[{name}]({priority}) : {class_name}")
 
     def register(self, class_object: object, priority: int = 0) -> None:
-
-        new_method = {
-            'priority': priority,
-            'object': class_object
-        }
+        new_method = {"priority": priority, "object": class_object}
 
         self._handlers.append(new_method)
 
 
 class Block:
-
     def __init__(self, **kwargs) -> None:
         self.input = kwargs
-        self.input['text']: str  # 输入的纯文本,用于恢复原始信息
-        self.input['word']: str  # 解析提取后的核心文本信息
-        self.sub_blocks = []   # 子模块
+        self.input["text"]: str  # 输入的纯文本,用于恢复原始信息
+        self.input["word"]: str  # 解析提取后的核心文本信息
+        self.sub_blocks = []  # 子模块
         self.block_name = self.__class__.__name__
 
     def register(self, class_object):
-
         global CONTAINER
         return CONTAINER.register(class_object)
 
     def restore(self, TextBlock):
         # restore用于恢复嵌套的block替换
         # 这里传入 TextBlock 是因为 TextBlock 还未定义
         global CONTAINER
-        RE = re.compile(r'({-%.*?%-})')
-        split_strings = RE.split(self.input['word'])
+        RE = re.compile(r"({-%.*?%-})")
+        split_strings = RE.split(self.input["word"])
         count = 0
 
         for string in split_strings:
             # 正常文本字符
             if count % 2 == 0:
                 if string:
                     self.addBlock(TextBlock(word=string, text=string))
             else:
                 id = string[3:-3]
                 class_object: Block = CONTAINER[id]
                 class_object.restore(TextBlock)
-                self.input['text'] = self.input['text'].replace(
-                    string, class_object.input['text'])
+                self.input["text"] = self.input["text"].replace(string, class_object.input["text"])
                 self.addBlock(class_object)
             count += 1
 
     def addBlock(self, block):
-
         self.sub_blocks.append(block)
 
     def __str__(self):  # pragma: no cover
-
         if not self.input:
-            return ''
-        output = '< '
+            return ""
+        output = "< "
         for k, v in self.input.items():
-            if k == 'text':
+            if k == "text":
                 continue
-            output += f'{k} = \"{v}\" | '
-        if output == '< ':
-            output = ''
+            output += f'{k} = "{v}" | '
+        if output == "< ":
+            output = ""
         else:
-            output = output[:-3] + ' >'
+            output = output[:-3] + " >"
         return output
 
     def info(self, deep: int = 0):  # pragma: no cover
         # root.info()
         # 递归输出信息
 
         if self.sub_blocks == []:
             return
         else:
             for block in self.sub_blocks:
-                print(' '*4*deep, end='')
-                print(f'[{block.__class__.__name__}] {str(block)}')
-                block.info(deep+1)
+                print(" " * 4 * deep, end="")
+                print(f"[{block.__class__.__name__}] {str(block)}")
+                block.info(deep + 1)
 
     def printInfo(self, deep: int = 0) -> str:  # pragma: no cover
         # print(root.printInfo())
         # 递归输出信息
-        output_str = ''
+        output_str = ""
         if self.sub_blocks == []:
             return output_str
         else:
             for block in self.sub_blocks:
-                output_str += ' '*4*deep
-                output_str += f'[{block.__class__.__name__}] {str(block)}\n'
-                output_str += block.printInfo(deep+1)
+                output_str += " " * 4 * deep
+                output_str += f"[{block.__class__.__name__}] {str(block)}\n"
+                output_str += block.printInfo(deep + 1)
             return output_str
 
     def toHTML(self, header_navigater=None):
         # 转换成HTML格式
-        content = ''
+        content = ""
         for block in self.sub_blocks:
             content += block.toHTML()
         if header_navigater:
             return f"{header_navigater}<div class='markdown-body'>{content}</div>"
         else:
             return f"<div class='markdown-body'>{content}</div>"
 
 
 class Handler:
-
     def __init__(self, parser=None) -> None:
-
         self.RE = None
         self.parser: Parser = parser
 
     def match(self, text: str, *args):  # pragma: no cover
-
         if self.RE is None:
             raise NotImplementedError
 
         return bool(self.RE.search(text))
 
     def __call__(self, root: Block, text: str):  # pragma: no cover
-
         raise NotImplementedError
 
 
 class Optimizer:
-
     def __init__(self) -> None:
-
         # 优化器针对的Block
         self.target_block_names = []
         self.is_match = False
 
     def __call__(self, root: Block):  # pragma: no cover
-
         raise NotImplementedError
```

### Comparing `markdownparser-0.5.1/MarkdownParser/block_parser.py` & `markdownparser-0.5.2/MarkdownParser/block_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,76 +1,70 @@
-
 from .base_class import Parser, Handler, Block, CONTAINER
 from typing import List
 import re
 
 
 class BlockParser(Parser):
-
     def __init__(self) -> None:
         super().__init__()
 
     def __call__(self, lines: List[str]):
-
-        self.root = Block(text='')
+        self.root = Block(text="")
         if not self.is_sorted:
             self._sort()
             self.is_sorted = True
 
         for text in lines:
             self.match(self.root, text)
         # self.root.info()
         return self.root
 
     def match(self, root: Block, text: str):
-
         for method in self._handlers:
-            if method['object'].match(text):
+            if method["object"].match(text):
                 # print(method['object'].__class__.__name__,'matched')
-                method['object'](root, text)
+                method["object"](root, text)
                 return
 
 
 class ComplexBlock(Block):
     # 用于处理复杂嵌套
 
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)  # pragma: no cover
 
     def toHTML(self):
-
-        content = ''
+        content = ""
         for block in self.sub_blocks:
             content += block.toHTML()
 
         return content
 
 
 class HTMLBlock(Block):
     # 处理HTML标签
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)  # pragma: no cover
 
     def __str__(self):
-        return '<html>'  # pragma: no cover
+        return "<html>"  # pragma: no cover
 
     def toHTML(self):
-        return self.input['text']
+        return self.input["text"]
 
 
 class AnnotateBlock(Block):
-
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
     def __str__(self):
-        return '<!-->'  # pragma: no cover
+        return "<!-->"  # pragma: no cover
 
     def toHTML(self):
-        return ''
+        return ""
 
 
 class EmptyBlockHandler(Handler):
     # 处理空行
 
     def __init__(self, parser) -> None:
         super().__init__(parser)
@@ -79,449 +73,454 @@
         return not text.strip()
 
     def __call__(self, root: Block, text: str):
         root.addBlock(EmptyBlock(text=text))
 
 
 class EmptyBlock(Block):
-
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
     def toHTML(self):
-        return ''
+        return ""
 
 
 class EscapeCharacterHandler(Handler):
     # 解释一下这里
     # 这里的方法名和preprocess_parser中有着同名方法EscapeCharacterHandler
     # 这里用于处理恢复为纯文本后再处理的情况, 因为预处理阶段优先级较高
     # 对于类似table的匹配会出现重新恢复文本,分割后再依次匹配的情况
 
     def __init__(self, parser=None) -> None:
         super().__init__(parser)
-        self.RE = re.compile(r'\\(.)')
+        self.RE = re.compile(r"\\(.)")
 
     def subFunc(self, match):
         global CONTAINER
         word = match.group(1)
-        block = EscapeCharacterBlock(word=word, text='\\'+word)
+        block = EscapeCharacterBlock(word=word, text="\\" + word)
         replace_name = self.block.register(block)  # 注册并替换名字
         return replace_name
 
     def __call__(self, root: Block, text: str):
-
         self.block = ComplexBlock(text=text)
         # 替换所有匹配项并重新解析new_text
         new_text = re.sub(self.RE, self.subFunc, text)
         self.parser.match(self.block, new_text)
         # 单匹配去掉外层 ComplexBlock
         if len(self.block.sub_blocks) == 1:
             self.block = self.block.sub_blocks[0]
         root.addBlock(self.block)
 
 
 class EscapeCharacterBlock(Block):
-
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
+        self.special_characters = [
+            "*",
+            "[",
+            "]",
+            "{",
+            "}",
+            "(",
+            ")",
+            ".",
+            '"',
+            "'",
+            "\\",
+            "`",
+            "+",
+            "-",
+            "<",
+            ">",
+            "?",
+            "/",
+            "~",
+            "|",
+            "!",
+            "@",
+            "#",
+            "$",
+            "%",
+            "^",
+            "&",
+            ";",
+            ":",
+        ]
 
     def toHTML(self):
-        return self.input['word']
+        if self.input["word"] in self.special_characters:
+            return self.input["word"]
+        else:
+            return "\\" + self.input["word"]
+
 
 # 已废弃
 
 
 class ExtensionBlockHandler(Handler):  # pragma: no cover
     # 自定义扩展
     # {% note %}
     # asdklja
     # {%end%}
 
     def __init__(self, parser=None) -> None:
         super().__init__(parser)
-        self.RE = re.compile(r"""(
+        self.RE = re.compile(
+            r"""(
             (^{[ ]*%[ ]*note[ ]*%[ ]*}[ ]*)|
             (^{[ ]*%[ ]*info[ ]*%[ ]*}[ ]*)|
             (^{[ ]*%[ ]*success[ ]*%[ ]*}[ ]*)|
             (^{[ ]*%[ ]*end[ ]*%[ ]*}[ ]*)
-        )""", re.VERBOSE)
+        )""",
+            re.VERBOSE,
+        )
 
-        self.groupid_tag = {
-            2: 'note',
-            3: 'info',
-            4: 'success',
-            5: 'end'
-        }
+        self.groupid_tag = {2: "note", 3: "info", 4: "success", 5: "end"}
 
     def __call__(self, root: Block, text: str):
         match = re.match(self.RE, text)
         # print(match)
         for k, v in self.groupid_tag.items():
             if match.group(k):
                 tag = v
                 break
 
         self.block = ExtensionBlock(text=text, tag=tag)
         root.addBlock(self.block)
 
 
 class ExtensionBlock(Block):  # pragma: no cover
-
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
     def toHTML(self):
-
-        tag = self.input['tag']
+        tag = self.input["tag"]
         content = ""
         for block in self.sub_blocks:
             content += block.toHTML()
-        return f'<div id=\"{tag}\">{content}</div>'
+        return f'<div id="{tag}">{content}</div>'
 
 
 class SplitBlockHandler(Handler):
-
     def __init__(self, parser) -> None:
         super().__init__(parser)
-        self.RE = re.compile(r'^[-=\*]{3,} *$')      # 分隔符
+        self.RE = re.compile(r"^[-=\*]{3,} *$")  # 分隔符
 
     def __call__(self, root: Block, text: str):
         root.addBlock(SplitBlock(text=text))
 
 
 class SplitBlock(Block):
-
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
     def __str__(self):  # pragma: no cover
-        return '---<hr>---'
+        return "---<hr>---"
 
     def toHTML(self):
-        return '<hr>'
+        return "<hr>"
 
 
 class HierarchyIndentHandler(Handler):
     # 匹配层次缩进
     # - 123
     #   hello world
     #   good luck
 
     def __init__(self, parser) -> None:
         super().__init__(parser)
-        self.RE = re.compile(r'^([ ]{1,})(.*)')
+        self.RE = re.compile(r"^([ ]{1,})(.*)")
 
     def __call__(self, root: Block, text: str):
-
         match_group = re.match(self.RE, text)
         space_number = len(match_group.group(1))
         word = match_group.group(2)
 
         self.block = HierarchyBlock(space_number=space_number, text=text)
         self.parser.match(self.block, word)
         # 因为多重 Complex 传递的问题导致的 escape 字符的bug(test8.md)
         # 暂时没有更好的修改方法...
         if len(self.block.sub_blocks) == 1:
-            self.block.input['text'] = ' ' * space_number + self.block.sub_blocks[0].input['text']
+            self.block.input["text"] = " " * space_number + self.block.sub_blocks[0].input["text"]
         root.addBlock(self.block)
 
 
 class HierarchyBlock(Block):
-
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
 
 class CodeBlockHandler(Handler):
     # 匹配代码段
     # ```python
     # a = 1
     # ```
 
     def __init__(self, parser) -> None:
         super().__init__(parser)
-        self.RE = re.compile(r'`{3,}(.*)')
+        self.RE = re.compile(r"`{3,}(.*)")
 
     def __call__(self, root: Block, text: str):
-
         match_group = re.match(self.RE, text)
         language = match_group.group(1).strip()
 
         if language:
             # 代码段开头
             root.addBlock(CodeBlock(language=language, text=text))
         else:
             # 代码段结尾
-            root.addBlock(CodeBlock(language='UNKNOWN', text=text))
+            root.addBlock(CodeBlock(language="UNKNOWN", text=text))
 
 
 class CodeBlock(Block):
-
     def __init__(self, **kwargs) -> None:
         # code用于在优化阶段用于整合所有的代码
-        super().__init__(code='', **kwargs)
+        super().__init__(code="", **kwargs)
 
     def toHTML(self):
-        code = self.input['code']
-        code = re.sub('<', '&lt;', code)
-        code = re.sub('>', '&gt;', code)
-        language = self.input['language']
-        return f'<pre><code class=\"language-{language}\">{code}</code></pre>'
+        code = self.input["code"]
+        code = re.sub("<", "&lt;", code)
+        code = re.sub(">", "&gt;", code)
+        language = self.input["language"]
+        return f'<pre><code class="language-{language}">{code}</code></pre>'
 
 
 class HashHeaderHandler(Handler):
     # 匹配标题
     # ### 123
 
     def __init__(self, parser) -> None:
         super().__init__(parser)
         self.parser = parser
 
         # #开头,1-6个#均可 + 一个空格 + 文字
         # Typora               r'(^#{1,6}) (.+)'
         # Markdown All in One  r'(^#{1,6}) (.?)'
-        self.RE = re.compile(r'(^#{1,6}) (.+)')
+        self.RE = re.compile(r"(^#{1,6}) (.+)")
 
     def __call__(self, root: Block, text: str):
-
         match_group = re.match(self.RE, text)
         level = len(match_group.group(1))
         header = match_group.group(2).strip()  # 去掉头尾多余空格
 
         # 继续匹配header中的文字
         block = HashHeaderBlock(level=level, word=header, text=text)
         self.parser.match(block, header)
         root.addBlock(block)
 
 
 class HashHeaderBlock(Block):
-
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
         self.child_blocks = []
         self.parent_block = None
         self.UID = None
 
     def toHTML(self):
-        
-        head_level = str(self.input['level'])
-        tag = f'h{head_level}'
+        head_level = str(self.input["level"])
+        tag = f"h{head_level}"
         if self.UID is not None:
-            tag_id = f'id=\"{tag}-{str(self.UID)}\"'
+            tag_id = f'id="{tag}-{str(self.UID)}"'
         else:
-            tag_id = ''
-        return f'<{tag} {tag_id}>{self.sub_blocks[0].toHTML()}</{tag}>'
-    
+            tag_id = ""
+        return f"<{tag} {tag_id}>{self.sub_blocks[0].toHTML()}</{tag}>"
+
     def to_href(self):
-        '''
+        """
         纯文字形式
-        '''
-        word = ''
+        """
+        word = ""
         if self.sub_blocks[0].block_name == "ComplexBlock":
             block = self.sub_blocks[0]
             for sblock in block.sub_blocks:
-                word += sblock.input['word']
+                word += sblock.input["word"]
         else:
-            word = self.sub_blocks[0].input['word']
+            word = self.sub_blocks[0].input["word"]
         return word
 
-class TaskListHandler(Handler):
 
+class TaskListHandler(Handler):
     def __init__(self, parser) -> None:
         super().__init__(parser)
-        self.RE = re.compile(r'(?<=^[-+\*] )\[([ x])\] (.*)')
+        self.RE = re.compile(r"(?<=^[-+\*] )\[([ x])\] (.*)")
 
     def subFunc(self, match: re.Match):
         is_complete = match.group(1)
         word = match.group(2)
 
-        task_block = TaskListBlock(
-            complete=is_complete, word=word, text=match.group())
+        task_block = TaskListBlock(complete=is_complete, word=word, text=match.group())
         replace_name = self.block.register(task_block)  # 注册并替换名字
         return replace_name
 
     def __call__(self, root: Block, text: str):
-
         self.block = ComplexBlock(text=text)
         # 替换所有匹配项并重新解析new_text
         new_text = re.sub(self.RE, self.subFunc, text)
         self.parser.match(self.block, new_text)
         # 单匹配去掉外层 ComplexBlock
         if len(self.block.sub_blocks) == 1:
             self.block = self.block.sub_blocks[0]
         root.addBlock(self.block)
 
 
 class TaskListBlock(Block):
-
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
     def toHTML(self):
-
-        checked = "checked" if self.input['complete'] == 'x' else ''
-        word = self.input['word']
+        checked = "checked" if self.input["complete"] == "x" else ""
+        word = self.input["word"]
         return f'<div><input type="checkbox" disabled {checked}>{word}</div>'
 
 
 class OListHandler(Handler):
     # 匹配有序列表
     # 1. 123
     # 2. 123
 
     def __init__(self, parser) -> None:
         super().__init__(parser)
-        self.RE = re.compile(r'^(\d+)\. (.*)')
+        self.RE = re.compile(r"^(\d+)\. (.*)")
 
     def __call__(self, root: Block, text: str):
-
         match_group = re.match(self.RE, text)
         serial_number = match_group.group(1)
         align_space_number = len(serial_number) + 2
         word = match_group.group(2)
 
-        block = OListBlock(serial_number=serial_number,
-                           align_space_number=align_space_number,
-                           word=word, text=text)
+        block = OListBlock(
+            serial_number=serial_number, align_space_number=align_space_number, word=word, text=text
+        )
         self.parser.match(block, word)
         root.addBlock(block)
 
 
 class OListBlock(Block):
-
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
     def toHTML(self):
-
-        content = ''
+        content = ""
         for block in self.sub_blocks:
             content += block.toHTML()
-        serial_number = self.input['serial_number']
-        return f'<ol start=\"{serial_number}\"><li>{content}</li></ol>'
+        serial_number = self.input["serial_number"]
+        return f'<ol start="{serial_number}"><li>{content}</li></ol>'
 
 
 class UListHandler(Handler):
-
     def __init__(self, parser) -> None:
         super().__init__(parser)
-        self.RE = re.compile(r'^[-+\*] (.*)')
+        self.RE = re.compile(r"^[-+\*] (.*)")
 
     def __call__(self, root: Block, text: str):
-
         match_group = re.match(self.RE, text)
         word = match_group.group(1)
         align_space_number = 2
 
-        block = UListBlock(
-            word=word, align_space_number=align_space_number, text=text)
+        block = UListBlock(word=word, align_space_number=align_space_number, text=text)
         self.parser.match(block, word)
         root.addBlock(block)
 
 
 class UListBlock(Block):
-
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
     def toHTML(self):
-
-        content = ''
+        content = ""
         for block in self.sub_blocks:
             content += block.toHTML()
 
-        return f'<ul><li>{content}</li></ul>'
+        return f"<ul><li>{content}</li></ul>"
 
 
 class QuoteHandler(Handler):
     # 匹配引用
     # > 123
     def __init__(self, parser) -> None:
         super().__init__(parser)
-        self.RE = re.compile(r'^>[ ]*(.*)')
+        self.RE = re.compile(r"^>[ ]*(.*)")
 
     def __call__(self, root: Block, text: str):
-
         match_group = re.match(self.RE, text)
         word = match_group.group(1)
         block = QuoteBlock(word=word, text=text)
         self.parser.match(block, word)
         root.addBlock(block)
 
 
 class QuoteBlock(Block):
-
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
     def toHTML(self):
-
-        content = ''
+        content = ""
         for block in self.sub_blocks:
             content += block.toHTML()
 
-        return f'<blockquote>{content}</blockquote>'
+        return f"<blockquote>{content}</blockquote>"
 
 
 class PictureHandler(Handler):
     # 匹配图片
     # ![asd](123)
 
     def __init__(self, parser) -> None:
         super().__init__(parser)
-        self.RE = re.compile(r'!\[([^\!\[\]]*?)\]\((.*?)\)')
+        self.RE = re.compile(r"!\[([^\!\[\]]*?)\]\((.*?)\)")
 
     def subFunc(self, match: re.Match):
         word = match.group(1)
         url = match.group(2)
         pic_block = PictureBlock(word=word, url=url, text=match.group())
         replace_name = self.block.register(pic_block)  # 注册并替换名字
         return replace_name
 
     def __call__(self, root: Block, text: str):
-
         self.block = ComplexBlock(text=text)
         # 替换所有匹配项并重新解析new_text
         new_text = re.sub(self.RE, self.subFunc, text)
 
         self.parser.match(self.block, new_text)
         # 单匹配去掉外层 ComplexBlock
         if len(self.block.sub_blocks) == 1:
             self.block = self.block.sub_blocks[0]
 
         root.addBlock(self.block)
 
 
 class PictureBlock(Block):
-
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
     def toHTML(self):
-        word = self.input['word']
-        url = self.input['url']
-        return f'<img src=\"{url}\" alt=\"{word}\">'
+        word = self.input["word"]
+        url = self.input["url"]
+        return f'<img src="{url}" alt="{word}">'
 
 
 class ReferenceHandler(Handler):
     # 处理引用
     # [1](abc)
 
     def __init__(self, parser) -> None:
         super().__init__(parser)
         # 匹配嵌套 + 忽略末尾多余 )
 
         # Typora               r'\[([^\[\]]*?)\]\((.*?)\)'
         # Markdown All in One  ...
-        self.RE = re.compile(r"""(
+        self.RE = re.compile(
+            r"""(
             \[(.*?)\]\((.*?)\)|
             <(https?:\/\/[\w\-_]+(?:\.[\w\-_]+)+(?:[\w\-\.,@?^=%&:\/~\+#]*[\w\-\@?^=%&\/~\+#])?)>|
             \bhttps?:\/\/[\w\-_]+(?:\.[\w\-_]+)+(?:[\w\-\.,@?^=%&:\/~\+#]*[\w\-\@?^=%&\/~\+#])?\b
-        )""", re.VERBOSE)
+        )""",
+            re.VERBOSE,
+        )
 
     def subFunc(self, match: re.Match):
         word = match.group(2)
         url = match.group(3)
 
         if url is None:
             # <> 的匹配
@@ -531,229 +530,216 @@
                 url = match.group(1)
             word = url
         ref_block = ReferenceBlock(word=word, url=url, text=match.group())
         replace_name = self.block.register(ref_block)  # 注册并替换名字
         return replace_name
 
     def __call__(self, root: Block, text: str):
-
         self.block = ComplexBlock(text=text)
         # 替换所有匹配项并重新解析new_text
         new_text = re.sub(self.RE, self.subFunc, text)
         self.parser.match(self.block, new_text)
         # 单匹配去掉外层 ComplexBlock
         if len(self.block.sub_blocks) == 1:
             self.block = self.block.sub_blocks[0]
         root.addBlock(self.block)
 
 
 class ReferenceBlock(Block):
-
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
         # 默认Markdown启用的是_self, 这里存粹是因为我自己的习惯所以改成 _blank
-        self.target = '_blank'
+        self.target = "_blank"
         # self.target = '_self'
 
     def toHTML(self):
-
-        url = self.input['url']
-        content = ''
+        url = self.input["url"]
+        content = ""
         for block in self.sub_blocks:
             content += block.toHTML()
-        return f"<a href=\"{url}\" target=\"{self.target}\">{content}</a>"
+        return f'<a href="{url}" target="{self.target}">{content}</a>'
 
 
 class SpecialTextHandler(Handler):
     # 处理特殊字符
     # 不考虑 * 的多级嵌套
 
     def __init__(self, parser) -> None:
         super().__init__(parser)
-        self.RE = re.compile(r"""(
+        self.RE = re.compile(
+            r"""(
             \*{3}(.+?)\*{3}|                           # 粗体+斜体
             \*{2}(.+?)\*{2}|                           # 粗体
             \*(.+?)\*|                                 # 斜体
             ~~(.+?)~~|                                 # 删除线
             ``(.+?)``|                                 # 高亮
             `(.+?)`                                    # 高亮
-        )""", re.VERBOSE)
+        )""",
+            re.VERBOSE,
+        )
         self.groupid_tag = {
-            2: 'bold+italics',
-            3: 'bold',
-            4: 'italic',
-            5: 'delete',
-            6: 'highlight',
-            7: 'highlight'
+            2: "bold+italics",
+            3: "bold",
+            4: "italic",
+            5: "delete",
+            6: "highlight",
+            7: "highlight",
         }
 
     def subFunc(self, match: re.Match):
-
         for k, v in self.groupid_tag.items():
             if match.group(k):
                 word = match.group(k)
                 tag = v
                 break
-        special_text_block = SpecialTextBlock(
-            word=word, tag=tag, text=match.group())
+        special_text_block = SpecialTextBlock(word=word, tag=tag, text=match.group())
         replace_name = self.block.register(special_text_block)  # 注册并替换名字
         return replace_name
 
     def __call__(self, root: Block, text: str):
-
         self.block = ComplexBlock(text=text)
         # 替换所有匹配项并重新解析new_text
         new_text = re.sub(self.RE, self.subFunc, text)
 
         self.parser.match(self.block, new_text)
         # 单匹配去掉外层 ComplexBlock
         if len(self.block.sub_blocks) == 1:
             self.block = self.block.sub_blocks[0]
         root.addBlock(self.block)
 
 
 class SpecialTextBlock(Block):
-
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
     def toHTML(self):
-
-        tag = self.input['tag']
-        content = ''
+        tag = self.input["tag"]
+        content = ""
         for block in self.sub_blocks:
             content += block.toHTML()
-        if tag == 'bold+italics':
-            return f'<i><b>{content}</b></i>'
-        elif tag == 'bold':
-            return f'<b>{content}</b>'
-        elif tag == 'italic':
-            return f'<i>{content}</i>'
-        elif tag == 'delete':
-            return f'<del>{content}</del>'
-        elif tag == 'highlight':
-            return f'<code>{content}</code>'
+        if tag == "bold+italics":
+            return f"<i><b>{content}</b></i>"
+        elif tag == "bold":
+            return f"<b>{content}</b>"
+        elif tag == "italic":
+            return f"<i>{content}</i>"
+        elif tag == "delete":
+            return f"<del>{content}</del>"
+        elif tag == "highlight":
+            return f"<code>{content}</code>"
 
 
 class TableHandler(Handler):
     # 处理表格
     # 不想支持原生表格...
 
     def __init__(self, parser) -> None:
         super().__init__(parser)
-        self.RE = re.compile(r'^\|(?: *:?-{1,}:? *\|)+')  # 判断表格出现
+        self.RE = re.compile(r"^\|(?: *:?-{1,}:? *\|)+")  # 判断表格出现
 
     def __call__(self, root: Block, text: str):
         # 判断对齐方式
-        lines = text.split('|')[1:-1]
+        lines = text.split("|")[1:-1]
         alignments = []
         for line in lines:
-            if re.search(r':-+:', line):
-                alignments.append('center')
-            elif re.search(r'-:', line):
-                alignments.append('right')
+            if re.search(r":-+:", line):
+                alignments.append("center")
+            elif re.search(r"-:", line):
+                alignments.append("right")
             else:
-                alignments.append('left')
+                alignments.append("left")
         root.addBlock(TableBlock(text=text, alignments=alignments))
 
 
 class TableBlock(Block):
-
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
         # self.input['header'] 表格头节点
         # self.input['alignments'] 表格对齐方式
         # self.input['length'] 表格列数
         # self.input['table_items'] 每一行的表格项(Block)
 
     def _addTableItem(self, block: Block):
         # 将一个table表项添加到Block中
         self.sub_blocks.extend(block.sub_blocks)
 
     def toHTML(self):
+        alignments = self.input["alignments"]
 
-        alignments = self.input['alignments']
-
-        table_header_content = '<tr>'
-        for block in self.input['header'].sub_blocks:
-            table_header_content += f'<th>{block.toHTML()}</th>'
-        table_header_content += '</tr>'
+        table_header_content = "<tr>"
+        for block in self.input["header"].sub_blocks:
+            table_header_content += f"<th>{block.toHTML()}</th>"
+        table_header_content += "</tr>"
 
-        table_items_content = ''
+        table_items_content = ""
         for i in range(len(self.sub_blocks)):
             if i % len(alignments) == 0:
-                table_items_content += '<tr>'
+                table_items_content += "<tr>"
             align_style = alignments[i % len(alignments)]
-            table_items_content += f'<td style=\"text-align:{align_style}\">\
+            table_items_content += f'<td style="text-align:{align_style}">\
                 {self.sub_blocks[i].toHTML()}</td>'
-            if (i+1) % len(alignments) == 0:
-                table_items_content += '</tr>'
+            if (i + 1) % len(alignments) == 0:
+                table_items_content += "</tr>"
 
-        return f'<table>{table_header_content}{table_items_content}</table>'
+        return f"<table>{table_header_content}{table_items_content}</table>"
 
 
 class TextHandler(Handler):
     # 处理常规文本
 
     def __init__(self, parser) -> None:
         super().__init__(parser)
 
     def match(self, text: str):
         return True
 
     def __call__(self, root: Block, text: str):
-
         global CONTAINER
-        RE = re.compile(r'({-%.*?%-})')
+        RE = re.compile(r"({-%.*?%-})")
         split_strings = RE.split(text.strip())
 
         count = 0
         temp_block = ComplexBlock(text=text)
 
         for string in split_strings:
             # 正常文本字符
             if count % 2 == 0:
                 if string:
                     temp_block.addBlock(TextBlock(word=string, text=string))
             else:
                 id = string[3:-3]
                 class_object: Block = CONTAINER[id]
-                replace_str = class_object.input['text']
+                replace_str = class_object.input["text"]
                 if class_object is not None:
                     class_object.restore(TextBlock)
-                    temp_block.input['text'] = temp_block.input['text'].replace(
-                        string, replace_str)
-                    root.input['text'] = root.input['text'].replace(
-                        string, replace_str)
+                    temp_block.input["text"] = temp_block.input["text"].replace(string, replace_str)
+                    root.input["text"] = root.input["text"].replace(string, replace_str)
                     temp_block.addBlock(class_object)
                 else:
                     # 由于在解析过程中中间变量使用了{-%.*?%-}的格式进行代替
                     # 所以如果原本的Markdown输入中就包含类似的 {-%asdjkl%-}文字则会出现无法找到的情况
-                    temp_block.addBlock(
-                        TextBlock(word=string, text=string))  # pragma: no cover
+                    temp_block.addBlock(TextBlock(word=string, text=string))  # pragma: no cover
             count += 1
 
         if len(temp_block.sub_blocks) <= 1:
             root.addBlock(temp_block.sub_blocks[0])
         else:
             root.addBlock(temp_block)
 
 
 class TextBlock(Block):
-
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
     def toHTML(self):
-
         # fix bug: 修复一些 <abc> 这种虽然不匹配网址, 但是会被 html 解析为标签的情况
         # 见 test14.md
-        self.input['word'] = self.input['word'].replace('<','&lt').replace('>','&gt')
+        self.input["word"] = self.input["word"].replace("<", "&lt").replace(">", "&gt")
 
-        return self.input['word']
+        return self.input["word"]
 
 
 def buildBlockParser():
     # block parser 用于逐行处理文本, 并将结果解析为一颗未优化的树
     block_parser = BlockParser()
     block_parser.register(EmptyBlockHandler(block_parser), 100)
     block_parser.register(EscapeCharacterHandler(block_parser), 98)
```

### Comparing `markdownparser-0.5.1/MarkdownParser/core.py` & `markdownparser-0.5.2/MarkdownParser/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,56 @@
-
-
 from .preprocess_parser import buildPreprocessParser
 from .block_parser import buildBlockParser
 from .tree_parser import buildTreeParser
 
 
 class Markdown:
     def __init__(self) -> None:
         self.build_parser()
 
     def build_parser(self):
-
         self.preprocess_parser = buildPreprocessParser()
         self.block_parser = buildBlockParser()
         self.tree_parser = buildTreeParser()
 
     def parse(self, text: str) -> str:
-
         # 去除空行/注释/html标签
         lines = self.preprocess_parser(text)
         # print(lines)
         # 逐行解析,得到一颗未优化的树
         root = self.block_parser(lines)
         # root.info()
         # 优化,得到正确的markdown解析树
         tree = self.tree_parser(root)
         # tree.info()
         # 输出到屏幕 / 导出html文件
         return tree.toHTML()
 
     def parse_with_tag(self, text: str):
-
         # 去除空行/注释/html标签
         lines = self.preprocess_parser(text)
         # print(lines)
         # 逐行解析,得到一颗未优化的树
         root = self.block_parser(lines)
         # root.info()
         # 优化,得到正确的markdown解析树
         tree = self.tree_parser(root)
         # 输出到屏幕 / 导出html文件
         header_navigater = self.get_header_list(tree)
         return tree.toHTML(header_navigater)
 
     def get_header_list(self, tree):
-
         UID = 0
         H0_block = []
         activate_block = None  # 激活节点
         activate_block_level = 0
         for block in tree.sub_blocks:
             # 对所有 HashHeaderBlock 统计树结构
             if block.block_name == "HashHeaderBlock":
-                current_head_level = block.input['level']
+                current_head_level = block.input["level"]
                 # 第一次匹配
                 if activate_block is None:
                     activate_block = block
                     activate_block_level = current_head_level
                     activate_block.parent_block = None
                     activate_block.UID = UID
                     UID += 1
@@ -91,15 +85,15 @@
                     # 当前 block 是激活节点高层级的
                     else:
                         # 一直向上找
                         while activate_block_level >= current_head_level:
                             activate_block = activate_block.parent_block
                             if activate_block is None:
                                 break
-                            activate_block_level = activate_block.input['level']
+                            activate_block_level = activate_block.input["level"]
 
                         # 到达根部
                         if activate_block is None:
                             block.UID = UID
                             UID += 1
                             H0_block.append(block)
                             activate_block = block
@@ -113,77 +107,77 @@
                             block.parent_block = activate_block
                             activate_block = block
                             activate_block_level = current_head_level
 
         return self.get_header_navigator(H0_block)
 
     def get_header_navigator(self, H0_block):
-
-        navigator_html = ''
+        navigator_html = ""
         for block in H0_block:
             navigator_html += self._get_header_navigator(block)
-        navigator_html = f'<div class=\"header-navigator\">{navigator_html}</div>'
+        navigator_html = f'<div class="header-navigator">{navigator_html}</div>'
         return navigator_html
 
     def _get_header_navigator(self, block):
-
-        navigator_html = ''
-        level = block.input['level']
-        tag = f'h{str(level)}-{str(block.UID)}'
+        navigator_html = ""
+        level = block.input["level"]
+        tag = f"h{str(level)}-{str(block.UID)}"
         word = block.to_href()
         if len(block.child_blocks) == 0:
-            navigator_html = f'<ul><li><a href=\"#{tag}\">{word}</a></li></ul>'
+            navigator_html = f'<ul><li><a href="#{tag}">{word}</a></li></ul>'
         else:
-            sub_navigator_html = ''
+            sub_navigator_html = ""
             for cblock in block.child_blocks:
                 sub_navigator_html += self._get_header_navigator(cblock)
-            navigator_html = f'<ul><li><a href=\"#{tag}\">{word}</a>{sub_navigator_html}</li></ul>'
+            navigator_html = f'<ul><li><a href="#{tag}">{word}</a>{sub_navigator_html}</li></ul>'
 
         return navigator_html
 
 
-def parse(text: str, ) -> str:
-    '''
+def parse(
+    text: str,
+) -> str:
+    """
     解析 markdown 文本转 html
-    '''
+    """
     assert type(text) == str, "输入应为字符串"
 
     # 空输入
     if not text.strip():
-        return ''
+        return ""
 
     md = Markdown()
     return md.parse(text)
 
 
 def parse_file(file_name: str) -> str:
-    '''
+    """
     解析 md 文件转 html
-    '''
-    with open(file_name, 'r', encoding='utf-8') as f:
+    """
+    with open(file_name, "r", encoding="utf-8") as f:
         text = f.read()
 
     return parse(text)
 
 
 def parse_toc(text: str) -> str:
-    '''
+    """
     解析 markdown 文本, 带目录树
-    '''
+    """
     assert type(text) == str, "输入应为字符串"
 
     # 空输入
     if not text.strip():
-        return ''
+        return ""
 
     md = Markdown()
     return md.parse_with_tag(text)
 
 
 def parse_file_toc(file_name: str) -> str:
-    '''
+    """
     解析 md 文件, 带目录树
-    '''
-    with open(file_name, 'r', encoding='utf-8') as f:
+    """
+    with open(file_name, "r", encoding="utf-8") as f:
         text = f.read()
 
     return parse_toc(text)
```

### Comparing `markdownparser-0.5.1/MarkdownParser/preprocess_parser.py` & `markdownparser-0.5.2/MarkdownParser/preprocess_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,32 @@
-
-
 from .base_class import Parser, Handler
 import re
 from .block_parser import HTMLBlock, EscapeCharacterBlock, AnnotateBlock
 from .base_class import CONTAINER
 
 
 class PreprocessParser(Parser):
-
     def __init__(self) -> None:
         super().__init__()
 
     def __call__(self, data: str):
         self._sort()
         # 按优先级逐步执行相应处理方法
         for method in self._handlers:
-            data = method['object'](data)
+            data = method["object"](data)
 
-        lines = data.split('\n')
+        lines = data.split("\n")
         return lines
 
 
 class TabHandler(Handler):
-
     def __init__(self) -> None:
         super().__init__()
 
     def __call__(self, text: str):
-
         text = text.replace("\r\n", "\n").replace("\r", "\n")
         text = text.expandtabs(tabsize=4)
 
         return text
 
 
 class EscapeCharacterHandler(Handler):
@@ -39,20 +34,19 @@
 
     def __init__(self, parser=None) -> None:
         super().__init__(parser)
 
     def subFunc(self, match):
         global CONTAINER
         word = match.group(1)
-        block = EscapeCharacterBlock(word=word, text='\\'+word)
+        block = EscapeCharacterBlock(word=word, text="\\" + word)
         return CONTAINER.register(block)
 
     def __call__(self, text: str):
-
-        text = re.sub(r'\\(.)', self.subFunc, text)
+        text = re.sub(r"\\(.)", self.subFunc, text)
         return text
 
 
 class AnnotateHandler(Handler):
     # 去除注释
 
     def __init__(self, parser=None) -> None:
@@ -61,48 +55,46 @@
     def subFunc(self, match):
         global CONTAINER
         word = match.group()
         block = AnnotateBlock(word=word, text=word)
         return CONTAINER.register(block)
 
     def __call__(self, text: str):
-
-        text = re.sub(r'\<!--[\s\S]*?--\>', self.subFunc,
-                      text)                # 去除注释
+        text = re.sub(r"\<!--[\s\S]*?--\>", self.subFunc, text)  # 去除注释
         return text
 
 
 class HTMLLabelHandler(Handler):
-
     # TODO: 标签不自闭合的处理
 
     def __init__(self) -> None:
-
         super().__init__()
 
-        self.RE = re.compile(r"""
+        self.RE = re.compile(
+            r"""
             (<div[\s\S]*?>[\s\S]*?<\/div>|         # div
             <span[\s\S]*?>[\s\S]*?<\/span>|        # span
             <p[\s\S]*?>[\s\S]*?<\/p>|            # p
             <img[\s\S]*?>(?:<\/img>)?|   # image
             <iframe[\s\S]*?>[\s\S]*?<\/iframe>|    # iframe
             <br\/?>|
             <kbd>[\s\S]*?</kbd>
-            )""", re.VERBOSE)
+            )""",
+            re.VERBOSE,
+        )
 
     def __call__(self, text: str):
-
         def subFunc(match):
             global CONTAINER
             src = match.group(0)
             block = HTMLBlock(text=src, word=src)
             return CONTAINER.register(block)
 
         text = re.sub(self.RE, subFunc, text)
-        text = re.sub(r'^[\n]+', '', text)                    # 去除开头连续空换行
+        text = re.sub(r"^[\n]+", "", text)  # 去除开头连续空换行
         # text = re.sub(r'[\n]+$', '', text)                    # 去除结尾连续空换行
         # text = re.sub(r'[\n]{3,}', '\n\n', text)              # 去除连续换行
         # print(text)
         return text
 
 
 def buildPreprocessParser():
```

### Comparing `markdownparser-0.5.1/MarkdownParser/tree_parser.py` & `markdownparser-0.5.2/MarkdownParser/tree_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,78 +1,84 @@
-
 import re
 from .base_class import Parser, Optimizer, Block
-from .block_parser import TableBlock, BlockParser, TextBlock, EmptyBlockHandler, EscapeCharacterHandler, PictureHandler, ReferenceHandler, SpecialTextHandler, TableHandler, TextHandler
+from .block_parser import (
+    TableBlock,
+    BlockParser,
+    TextBlock,
+    EmptyBlockHandler,
+    EscapeCharacterHandler,
+    PictureHandler,
+    ReferenceHandler,
+    SpecialTextHandler,
+    TableHandler,
+    TextHandler,
+)
 
 
 class TreeParser(Parser):
-
     def __init__(self) -> None:
         super().__init__()
 
     def __call__(self, root: Block):
-
-        root.input['align_space_number'] = 0  # 用于 HierarchyEliminate 阶段的对齐空格调整
+        root.input["align_space_number"] = 0  # 用于 HierarchyEliminate 阶段的对齐空格调整
 
         self.checkBlock(root)
         return root
 
     def checkBlock(self, block: Block):
         # 深度优先的遍历root的所有节点,
         # 如果遇到相应的可优化项则将节点交由对应的优化器处理
         for optimizer in self._handlers:
-            optimizer['object'](block)
+            optimizer["object"](block)
 
         if block.sub_blocks == []:
             return
         else:
             for sub_block in block.sub_blocks:
                 self.checkBlock(sub_block)
 
 
 class HierarchyMerge(Optimizer):
     # 合并相同层级(space_number)
 
     def __init__(self) -> None:
         super().__init__()
-        self.target_block_names = ['HierarchyBlock', 'EmptyBlock']
+        self.target_block_names = ["HierarchyBlock", "EmptyBlock"]
 
     def __call__(self, root: Block):
-
         new_sub_blocks = []
         activite_block = None
         activite_space_number = 0
 
         for i in range(len(root.sub_blocks)):
             block: Block = root.sub_blocks[i]
             if block.block_name in self.target_block_names:
                 # EmptyBlock的处理相当于任意的space_number的HierarchyBlock
                 # space_number = -1
 
                 # first meet
                 if activite_block is None:
-                    activite_space_number = block.input.get('space_number', -1)
+                    activite_space_number = block.input.get("space_number", -1)
                     # 未在匹配状态的EmptyBlock不算入
                     if activite_space_number == -1:
                         new_sub_blocks.append(block)
                     else:
                         activite_block = block
                 else:
-                    current_space_number = block.input.get('space_number', -1)
+                    current_space_number = block.input.get("space_number", -1)
 
                     # 不处理连续的EmptyBlock
                     if current_space_number == -1:
-                        if activite_block.sub_blocks[-1].block_name == 'EmptyBlock':
+                        if activite_block.sub_blocks[-1].block_name == "EmptyBlock":
                             continue
                         else:
                             activite_block.sub_blocks.append(block)
                     # 层次相同,合并
                     elif current_space_number == activite_space_number:
-                        activite_block.input['text'] += '\n' + \
-                            block.input['text']
+                        activite_block.input["text"] += "\n" + block.input["text"]
                         activite_block.sub_blocks.extend(block.sub_blocks)
                     else:
                         # 层次缩进改变
                         new_sub_blocks.append(activite_block)
                         activite_block = block
                         activite_space_number = current_space_number
             else:
@@ -89,28 +95,27 @@
 
 class QuoteBlockMerge(Optimizer):
     # 合并相同层级的引用模块
     # 与HierarchyBlock不同的是,引用模块中EmptyBlock作为区分符
 
     def __init__(self) -> None:
         super().__init__()
-        self.target_block_names = ['QuoteBlock']
+        self.target_block_names = ["QuoteBlock"]
 
     def __call__(self, root: Block):
-
         new_sub_blocks = []
         activite_block = None
 
         for i in range(len(root.sub_blocks)):
             block: Block = root.sub_blocks[i]
             if block.block_name in self.target_block_names:
                 if activite_block is None:
                     activite_block = block
                 else:
-                    activite_block.input['text'] += '\n' + block.input['text']
+                    activite_block.input["text"] += "\n" + block.input["text"]
                     activite_block.sub_blocks.extend(block.sub_blocks)
             else:
                 if activite_block is not None:
                     new_sub_blocks.append(activite_block)
                     activite_block = None
                 new_sub_blocks.append(block)
 
@@ -121,102 +126,105 @@
 
 
 class CodeBlockOptimizer(Optimizer):
     # 将代码段之间的代码恢复为纯文本并保存在input['code']
 
     def __init__(self) -> None:
         super().__init__()
-        self.target_block_names = ['CodeBlock']
+        self.target_block_names = ["CodeBlock"]
 
     def __call__(self, root: Block):
-
         activite_CodeBlock = None
         restore_text = False
         new_sub_blocks = []
 
         for i in range(len(root.sub_blocks)):
-
             block: Block = root.sub_blocks[i]
             # 开始恢复纯文本
             if restore_text:
                 # 再一次遇到代码段标志,意味着结束
                 if block.block_name in self.target_block_names:
                     restore_text = False
                     # 去掉结尾换行符
-                    activite_CodeBlock.input['code'] = activite_CodeBlock.input['code'][:-1]
+                    activite_CodeBlock.input["code"] = activite_CodeBlock.input["code"][:-1]
                     new_sub_blocks.append(activite_CodeBlock)
                     activite_CodeBlock = None
                     continue
-                activite_CodeBlock.input['code'] += block.input['text'] + '\n'
+                activite_CodeBlock.input["code"] += block.input["text"] + "\n"
             else:
                 if block.block_name in self.target_block_names:
                     restore_text = True
                     activite_CodeBlock = block
                 else:
                     new_sub_blocks.append(block)
 
         # 代码段不匹配,一直到结尾全部恢复为文本
         if activite_CodeBlock is not None:
             # 去掉结尾换行符
-            activite_CodeBlock.input['code'] = activite_CodeBlock.input['code'][:-1]
+            activite_CodeBlock.input["code"] = activite_CodeBlock.input["code"][:-1]
             new_sub_blocks.append(activite_CodeBlock)
 
         root.sub_blocks = new_sub_blocks
 
 
 class HierarchyEliminate(Optimizer):
     # 消除多余EmptyBlock
     # 消除Hierarchy标签,调整UList OList对齐关系
 
     def __init__(self) -> None:
         super().__init__()
-        self.target_block_names = ['UListBlock', 'OListBlock']
+        self.target_block_names = ["UListBlock", "OListBlock"]
 
         self.interrupt_block_names = [
-            'CodeBlock', 'HashHeaderBlock', 'TableBlock', 'QuoteBlock', 'SplitBlock']
+            "CodeBlock",
+            "HashHeaderBlock",
+            "TableBlock",
+            "QuoteBlock",
+            "SplitBlock",
+        ]
         # 递进级层次缩进被打断
         # 例子:
         #
         # - 123
         # # abc
         #   - aaa
 
     def __call__(self, root: Block):
-
         # 当前节点的所需的对齐空格长度
         # 如果没有该属性则说明不需要考虑层次缩进的情况
-        root_align_space_number = root.input.get('align_space_number', None)
+        root_align_space_number = root.input.get("align_space_number", None)
         if root_align_space_number is None:
             return
 
         new_sub_blocks = []
         activite_block = None
         deeper_indent = False
 
         for i in range(len(root.sub_blocks)):
             block: Block = root.sub_blocks[i]
             if block.block_name in self.target_block_names:
                 # 对齐长度从根节点依次传递下去
-                block.input['align_space_number'] += root_align_space_number
+                block.input["align_space_number"] += root_align_space_number
                 # 切换
                 if deeper_indent:
                     new_sub_blocks.append(activite_block)
                 deeper_indent = True
                 activite_block = block
             elif block.block_name in self.interrupt_block_names:
                 deeper_indent = False
                 if activite_block is not None:
                     new_sub_blocks.append(activite_block)
                     activite_block = None
                 new_sub_blocks.append(block)
 
-            elif block.block_name == 'HierarchyBlock':
+            elif block.block_name == "HierarchyBlock":
                 if deeper_indent:
-                    left_space_number = block.input['space_number'] - \
-                        activite_block.input['align_space_number']
+                    left_space_number = (
+                        block.input["space_number"] - activite_block.input["align_space_number"]
+                    )
                     # 刚好满足缩进,直接展开
                     if left_space_number == 0:
                         activite_block.sub_blocks.extend(block.sub_blocks)
                     # 空格数多余缩进所需,归入activite_block节点放到下层处理
                     elif left_space_number > 0:
                         activite_block.addBlock(block)
                     # 空格数少于缩进所需, 归并到根节点
@@ -227,21 +235,24 @@
                             deeper_indent = False
                         new_sub_blocks.extend(block.sub_blocks)
                 # 递进级层次缩进被打断
                 else:
                     new_sub_blocks.extend(block.sub_blocks)
             else:
                 # EmptyBlock 先补齐在 UList OListBlock 下
-                if block.block_name == 'EmptyBlock':
+                if block.block_name == "EmptyBlock":
                     if deeper_indent:
                         # 忽略连续的EmptyBlock
-                        if activite_block.sub_blocks[-1].block_name != 'EmptyBlock':
+                        if activite_block.sub_blocks[-1].block_name != "EmptyBlock":
                             activite_block.addBlock(block)
                     else:
-                        if len(new_sub_blocks) > 1 and new_sub_blocks[-1].block_name == 'EmptyBlock':
+                        if (
+                            len(new_sub_blocks) > 1
+                            and new_sub_blocks[-1].block_name == "EmptyBlock"
+                        ):
                             continue
                         else:
                             new_sub_blocks.append(block)
                 else:
                     if activite_block is not None:
                         new_sub_blocks.append(activite_block)
                         activite_block = None
@@ -255,156 +266,151 @@
 
 
 class OListSerialOptimizer(Optimizer):
     # 优化 Olist 序号顺序
 
     def __init__(self) -> None:
         super().__init__()
-        self.target_block_names = ['OListBlock', 'EmptyBlock']
+        self.target_block_names = ["OListBlock", "EmptyBlock"]
 
     def __call__(self, root: Block):
-
         new_sub_blocks = []
         first_number = None
 
         for i in range(len(root.sub_blocks)):
             block: Block = root.sub_blocks[i]
             if block.block_name in self.target_block_names:
-                if block.block_name == 'EmptyBlock':
+                if block.block_name == "EmptyBlock":
                     continue
                 if first_number is None:
-                    first_number = int(block.input['serial_number'])
+                    first_number = int(block.input["serial_number"])
                 else:
                     first_number += 1
-                    block.input['serial_number'] = str(first_number)
+                    block.input["serial_number"] = str(first_number)
             else:
                 first_number = None
                 new_sub_blocks.append(block)
 
+
 # abort
 
 
 class ExtensionOptimizer(Optimizer):  # pragma: no cover
-
     def __init__(self) -> None:
         super().__init__()
-        self.target_block_names = ['ExtensionBlock']
-        self.extension_tag = ['note', 'info', 'success']
+        self.target_block_names = ["ExtensionBlock"]
+        self.extension_tag = ["note", "info", "success"]
 
     def __call__(self, root: Block):
-
         activite_block = None
         new_sub_blocks = []
 
         for i in range(len(root.sub_blocks)):
             block: Block = root.sub_blocks[i]
             if block.block_name in self.target_block_names:
-                if block.input['tag'] in self.extension_tag:
+                if block.input["tag"] in self.extension_tag:
                     if activite_block is None:
                         activite_block = block
                     # 不支持嵌套使用, 恢复为纯文本
                     else:
                         activite_block.addBlock(
-                            TextBlock(text=block.input['text'], word=block.input['text']))
-                elif block.input['tag'] == 'end':
+                            TextBlock(text=block.input["text"], word=block.input["text"])
+                        )
+                elif block.input["tag"] == "end":
                     if activite_block is None:
                         new_sub_blocks.append(
-                            TextBlock(text=block.input['text'], word=block.input['text']))
+                            TextBlock(text=block.input["text"], word=block.input["text"])
+                        )
                     else:
                         new_sub_blocks.append(activite_block)
                         activite_block = None
                 else:
-                    raise KeyError("Unknown tag " + block.input['tag'])
+                    raise KeyError("Unknown tag " + block.input["tag"])
             else:
                 if activite_block is not None:
                     activite_block.addBlock(block)
                 else:
                     new_sub_blocks.append(block)
 
         if activite_block is not None:
             new_sub_blocks.append(activite_block)
 
         root.sub_blocks = new_sub_blocks
 
 
 class TableBlockOptimizer(Optimizer):
-
     def __init__(self) -> None:
         super().__init__()
-        self.RE = re.compile(r'(?<!\\)\|')
-        self.block_parser = BlockParser()  # 初始化一个block parser 用于解析表格中出现的每一个表项, 
+        self.RE = re.compile(r"(?<!\\)\|")
+        self.block_parser = BlockParser()  # 初始化一个block parser 用于解析表格中出现的每一个表项,
         # 只注册下面这些 Handler, 不解析其他的
         self.block_parser.register(EmptyBlockHandler(self.block_parser), 100)
         self.block_parser.register(EscapeCharacterHandler(self.block_parser), 98)
         self.block_parser.register(PictureHandler(self.block_parser), 15)
         self.block_parser.register(ReferenceHandler(self.block_parser), 10)
         self.block_parser.register(SpecialTextHandler(self.block_parser), 5)
         self.block_parser.register(TableHandler(self.block_parser), 4)
         self.block_parser.register(TextHandler(self.block_parser), 0)
         # 匹配的
-        self.table_block_names = ['TableBlock']
+        self.table_block_names = ["TableBlock"]
 
         # 表格匹配,其余中断
-        self.header_block_names = ['TextBlock', 'ComplexBlock']
-        self.body_block_names = ['TextBlock', 'ComplexBlock', 'TableBlock']
+        self.header_block_names = ["TextBlock", "ComplexBlock"]
+        self.body_block_names = ["TextBlock", "ComplexBlock", "TableBlock"]
 
     def _createTableBlock(self, header_block: Block, table_block: Block):
         # 判断header和table列是否匹配
         # 匹配返回一个TableBlock对象实例,用于后续补充表格
         # 不匹配返回None
-        table_length = len(table_block.input['alignments'])
-        header_text = header_block.input['text']  # 获取原文
+        table_length = len(table_block.input["alignments"])
+        header_text = header_block.input["text"]  # 获取原文
 
         header = self.RE.split(header_text)
-        if len(header)-2 != table_length:
+        if len(header) - 2 != table_length:
             return None
 
         # 匹配,创建实例
         header = header[1:-1]
         for i in range(len(header)):
             header[i] = header[i].strip()
         # 重新解析每一个table的表项
         table_header_node = self.block_parser(header)
 
-        header_info = [i.input['word'] for i in table_header_node.sub_blocks]
-        table_header_node.input['info'] = header_info
+        header_info = [i.input["word"] for i in table_header_node.sub_blocks]
+        table_header_node.input["info"] = header_info
         new_table_block = TableBlock(
-            header=table_header_node,
-            alignments=table_block.input['alignments'],
-            length=len(header)
+            header=table_header_node, alignments=table_block.input["alignments"], length=len(header)
         )
         return new_table_block
 
     def _addTableItem(self, table_block: TableBlock, table_item_block: Block):
         # 添加表格项,多去少补
 
-        table_items = self.RE.split(table_item_block.input['text'])
+        table_items = self.RE.split(table_item_block.input["text"])
         if not table_items[0]:
             table_items.pop(0)
         if not table_items[-1]:
             table_items.pop()
-        table_length = table_block.input['length']
+        table_length = table_block.input["length"]
         if len(table_items) > table_length:
             table_items = table_items[:table_length]
         else:
-            table_items.extend(
-                [' ' for _ in range(table_length-len(table_items))])
+            table_items.extend([" " for _ in range(table_length - len(table_items))])
 
         for i in range(len(table_items)):
             table_items[i] = table_items[i].strip()
 
         table_item_node = self.block_parser(table_items)
         for i in range(len(table_item_node.sub_blocks)):
-            if table_item_node.sub_blocks[i].__class__.__name__ == 'EmptyBlock':
-                table_item_node.sub_blocks[i] = TextBlock(text='', word='')
+            if table_item_node.sub_blocks[i].__class__.__name__ == "EmptyBlock":
+                table_item_node.sub_blocks[i] = TextBlock(text="", word="")
         table_block._addTableItem(table_item_node)
         # table_item_node.info()
 
     def __call__(self, root: Block):
-
         new_sub_blocks = []
         table_block = None
         # 分两步匹配
         # 1. header + table 的BlockName匹配
         # 2. header 和 table 的列个数匹配
         match_table = False
         # root.info()
@@ -419,32 +425,31 @@
                     table_block = None
                 else:
                     self._addTableItem(table_block, block)
                     continue
             # 尝试匹配 TableBlock, 开头不可以
             if block.block_name in self.table_block_names and i != 0:
                 # 第一步匹配
-                if root.sub_blocks[i-1].block_name in self.header_block_names:
+                if root.sub_blocks[i - 1].block_name in self.header_block_names:
                     # 第二步匹配
-                    table_block = self._createTableBlock(
-                        root.sub_blocks[i-1], block)
+                    table_block = self._createTableBlock(root.sub_blocks[i - 1], block)
                     # 匹配成功
                     if table_block is not None:
                         match_table = True
                         # 把上一项header的TextBlock那一项退出来,已经整合到table_block中了
                         new_sub_blocks.pop()
                     else:
                         # 将TableBlock变为纯文本
                         new_sub_blocks.append(
-                            TextBlock(text=block.input['text'], word=block.input['text']))
+                            TextBlock(text=block.input["text"], word=block.input["text"])
+                        )
                         match_table = False
                 else:
                     # 第一步匹配失败则将 block 回退为 TextBlock
-                    block = TextBlock(
-                        text=block.input['text'], word=block.input['text'])
+                    block = TextBlock(text=block.input["text"], word=block.input["text"])
                     new_sub_blocks.append(block)
             else:
                 new_sub_blocks.append(block)
 
         if table_block is not None:
             new_sub_blocks.append(table_block)
         root.sub_blocks = new_sub_blocks
@@ -452,33 +457,46 @@
 
 class ParagraphOptimizer(Optimizer):
     # 将元素使用 ParagraphBlock 包裹起来
     # 以便创建p标签换行
 
     def __init__(self) -> None:
         super().__init__()
-        self.target_block_names = ['TextBlock', 'ComplexBlock', 'ReferenceBlock',
-                                   'PictureBlock', 'SpecialTextBlock', 'EscapeCharacterBlock']
-        self.interrupt_block_names = ['ParagraphBlock', 'HashHeaderBlock', 'EscapeCharacterBlock',
-                                      'TableBlock', 'HTMLBlock',
-                                      'ComplexBlock', 'ReferenceBlock', 'PictureBlock',
-                                      'SpecialTextBlock', 'AnnotateBlock']
+        self.target_block_names = [
+            "TextBlock",
+            "ComplexBlock",
+            "ReferenceBlock",
+            "PictureBlock",
+            "SpecialTextBlock",
+            "EscapeCharacterBlock",
+        ]
+        self.interrupt_block_names = [
+            "ParagraphBlock",
+            "HashHeaderBlock",
+            "EscapeCharacterBlock",
+            "TableBlock",
+            "HTMLBlock",
+            "ComplexBlock",
+            "ReferenceBlock",
+            "PictureBlock",
+            "SpecialTextBlock",
+            "AnnotateBlock",
+        ]
 
     def __call__(self, root: Block):
-
         if root.__class__.__name__ in self.interrupt_block_names:
             return
         activite_block = None
         new_sub_blocks = []
 
         for i in range(len(root.sub_blocks)):
             block: Block = root.sub_blocks[i]
             if block.block_name in self.target_block_names:
                 # 特殊情况,不划入ParagraphBlock
-                if root.__class__.__name__ in ['OListBlock', 'UListBlock'] and i == 0:
+                if root.__class__.__name__ in ["OListBlock", "UListBlock"] and i == 0:
                     new_sub_blocks.append(block)
                 elif activite_block is None:
                     activite_block = ParagraphBlock()
                     activite_block.addBlock(block)
                 else:
                     activite_block.addBlock(block)
             else:
@@ -490,43 +508,40 @@
         if activite_block is not None:
             new_sub_blocks.append(activite_block)
 
         root.sub_blocks = new_sub_blocks
 
 
 class ParagraphBlock(Block):
-
     def __init__(self, **kwargs) -> None:
         super().__init__(**kwargs)
 
     def toHTML(self):
-
-        content = ''
+        content = ""
         for block in self.sub_blocks:
             content += block.toHTML()
-        return f'<p>{content}</p>'
+        return f"<p>{content}</p>"
 
 
 class SpecialTextOptimizer(Optimizer):
     # 将高亮的文本恢复回
     def __init__(self) -> None:
         super().__init__()
-        self.target_block_names = ['SpecialTextBlock']
+        self.target_block_names = ["SpecialTextBlock"]
 
     def __call__(self, root: Block):
         # return
-        if root.__class__.__name__ in self.target_block_names and root.input['tag'] == 'highlight':
+        if root.__class__.__name__ in self.target_block_names and root.input["tag"] == "highlight":
             for i in range(len(root.sub_blocks)):
                 block: Block = root.sub_blocks[i]
-                origin_text = block.input['text']
+                origin_text = block.input["text"]
                 # 替换以消除html元素影响
-                origin_text = re.sub('<', '&lt;', origin_text)
-                origin_text = re.sub('>', '&gt;', origin_text)
-                root.sub_blocks[i] = TextBlock(
-                    text=origin_text, word=origin_text)
+                origin_text = re.sub("<", "&lt;", origin_text)
+                origin_text = re.sub(">", "&gt;", origin_text)
+                root.sub_blocks[i] = TextBlock(text=origin_text, word=origin_text)
 
 
 def buildTreeParser():
     # tree parser 用于优化并得到正确的解析树
     tree_parser = TreeParser()
     tree_parser.register(HierarchyMerge(), 100)
     tree_parser.register(QuoteBlockMerge(), 95)
```

### Comparing `markdownparser-0.5.1/README.md` & `markdownparser-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `markdownparser-0.5.1/PKG-INFO` & `markdownparser-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdownparser
-Version: 0.5.1
+Version: 0.5.2
 Summary: 
 Home-page: https://github.com/luzhixing12345/MarkdownParser
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

