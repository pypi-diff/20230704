# Comparing `tmp/doc_spell-0.1.0-py3-none-any.whl.zip` & `tmp/doc_spell-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,14 @@
-Zip file size: 7035 bytes, number of entries: 9
+Zip file size: 9890 bytes, number of entries: 12
+-rw-rw-r--  2.0 unx      856 b- defN 16-Jan-01 00:00 doc_spell/.doc-spell.yml
 -rw-rw-r--  2.0 unx      160 b- defN 16-Jan-01 00:00 doc_spell/__init__.py
--rw-rw-r--  2.0 unx     1439 b- defN 16-Jan-01 00:00 doc_spell/__main__.py
--rw-rw-r--  2.0 unx     9848 b- defN 16-Jan-01 00:00 doc_spell/cspell.py
+-rw-rw-r--  2.0 unx     2050 b- defN 16-Jan-01 00:00 doc_spell/__main__.py
+-rw-rw-r--  2.0 unx     1592 b- defN 16-Jan-01 00:00 doc_spell/conf.py
+-rw-rw-r--  2.0 unx     7316 b- defN 16-Jan-01 00:00 doc_spell/cspell.py
+-rw-rw-r--  2.0 unx     5470 b- defN 16-Jan-01 00:00 doc_spell/formatters.py
 -rw-rw-r--  2.0 unx       21 b- defN 16-Jan-01 00:00 doc_spell/__version__.py
-?rw-------  2.0 unx       53 b- defN 16-Jan-01 00:00 doc_spell-0.1.0.dist-info/entry_points.txt
-?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 doc_spell-0.1.0.dist-info/WHEEL
-?rw-------  2.0 unx     1201 b- defN 16-Jan-01 00:00 doc_spell-0.1.0.dist-info/METADATA
--rw-rw-r--  2.0 unx     1103 b- defN 16-Jan-01 00:00 doc_spell-0.1.0.dist-info/licenses/LICENSE
-?rw-------  2.0 unx      718 b- defN 16-Jan-01 00:00 doc_spell-0.1.0.dist-info/RECORD
-9 files, 14630 bytes uncompressed, 5797 bytes compressed:  60.4%
+?rw-------  2.0 unx       53 b- defN 16-Jan-01 00:00 doc_spell-0.2.0.dist-info/entry_points.txt
+?rw-------  2.0 unx       87 b- defN 16-Jan-01 00:00 doc_spell-0.2.0.dist-info/WHEEL
+?rw-------  2.0 unx     1223 b- defN 16-Jan-01 00:00 doc_spell-0.2.0.dist-info/METADATA
+-rw-rw-r--  2.0 unx     1103 b- defN 16-Jan-01 00:00 doc_spell-0.2.0.dist-info/licenses/LICENSE
+?rw-------  2.0 unx      952 b- defN 16-Jan-01 00:00 doc_spell-0.2.0.dist-info/RECORD
+12 files, 20883 bytes uncompressed, 8296 bytes compressed:  60.3%
```

## zipnote {}

```diff
@@ -1,28 +1,37 @@
+Filename: doc_spell/.doc-spell.yml
+Comment: 
+
 Filename: doc_spell/__init__.py
 Comment: 
 
 Filename: doc_spell/__main__.py
 Comment: 
 
+Filename: doc_spell/conf.py
+Comment: 
+
 Filename: doc_spell/cspell.py
 Comment: 
 
+Filename: doc_spell/formatters.py
+Comment: 
+
 Filename: doc_spell/__version__.py
 Comment: 
 
-Filename: doc_spell-0.1.0.dist-info/entry_points.txt
+Filename: doc_spell-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: doc_spell-0.1.0.dist-info/WHEEL
+Filename: doc_spell-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: doc_spell-0.1.0.dist-info/METADATA
+Filename: doc_spell-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: doc_spell-0.1.0.dist-info/licenses/LICENSE
+Filename: doc_spell-0.2.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: doc_spell-0.1.0.dist-info/RECORD
+Filename: doc_spell-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## doc_spell/__main__.py

```diff
@@ -1,65 +1,78 @@
 """
-Demonstrates pydevkit features.
+Code documentation spell checker.
+
+`doc-spell` extracts documentation and comments from a code and sends them to
+spell checker.
+
+It features
+ * support for programming languages: python, shell, makefile and more
+ * support for configuration files: YAML, INI, TOML
+ * private dictionaries, either as separate file or inline comments.
+ * reports in gcc format 'file:line:column'
+
+It does not work with markup (html, markdown or xml).
+
+Please see `https://github.com/aanatoly/doc-spell` for details.
 
 EPILOG:
-Example 1:
-```
-PYDEVKIT_LOG_HANDLER=app ./script --log-level=debug
+Example:
+Spell check python project, having python code, makefile and yaml
 ```
+doc-spell src/*.py Makefile *.yml
 
-Example 2:
-```
-./script --log-level=debug --log-handler=json
 ```
+
 """
 
 
 import pydevkit.log.config  # noqa: F401
 from pydevkit.log import prettify
 from pydevkit.argparse import ArgumentParser
-import yaml
-import os
-from yaml.loader import SafeLoader
-from .cspell import spell_checker
+from .cspell import spell_checker, UnsupportedFileError, SpellingError
 from . import __version__
-
+from .conf import conf_get, conf_init, CONFIG
 import sys
 import logging
 
 log = logging.getLogger(__name__)
 
-CONFIG = ".doc-spell.yml"
-
 
 def get_args():
     p = ArgumentParser(help=__doc__, version=__version__)
     p.add_argument("-c", help="configuration file", dest="config", default=CONFIG)
-    p.add_argument("files", help="files to check", nargs="+")
+    p.add_argument(
+        "--init", help="create sample configuration file", action="store_true"
+    )
+    p.add_argument("files", help="files to check", nargs="*")
 
     return p.parse_known_args()
 
 
 def main():
     args, unknown_args = get_args()
     if unknown_args:
         log.warning("Unknown arguments: %s", unknown_args)
         sys.exit(1)
-    log.info("reading configuration from `%s`", args.config)
-    try:
-        path = os.path.expanduser(args.config)
-        conf = yaml.load(open(path, "r"), Loader=SafeLoader)
-    except Exception as exp:
-        log.error("%s", exp)
-        conf = {}
+
+    if args.init:
+        conf_init()
+
+    conf = conf_get(args.config)
     log.debug("config: %s", prettify(conf))
     rc = 0
     for f in args.files:
         try:
             spell_checker(f, conf)
+            log.info("%s: spelling is ok", f)
+        except UnsupportedFileError as exp:
+            log.warning("%s: %s", exp.path, exp)
+        except SpellingError as exp:
+            log.error("%s: %s", exp.path, exp)
+            rc = 1
         except Exception as exp:
             log.error("%s", exp)
             rc = 1
     return rc
 
 
 if __name__ == "__main__":
```

## doc_spell/cspell.py

```diff
@@ -8,154 +8,84 @@
  * code snippets
  * variable references, function names
  * technical comments, like `noqa`, `pylint`
 
 """
 
 from pygments import highlight
-from pygments.lexers import get_lexer_by_name
-from pygments.token import Token
-from pygments.formatter import Formatter
+from pygments.lexers import (
+    get_lexer_by_name,
+    guess_lexer_for_filename,
+)
 import subprocess as sp
 import re
 import sys
 import os
 import tempfile
 from identify import identify
 import logging
 from pydevkit.log import prettify
+from .formatters import CodeFormatter
+
 
 log = logging.getLogger(__name__)
 
 
-def repl(matchobj):
-    txt = matchobj.group(0)
-    return tr(txt)
-
-
-def tr(txt):
-    rc = ""
-    for c in txt:
-        if c.isspace():
-            rc += c
-        else:
-            rc += " "
-    return rc
+# {{{ hunspell invocation
+class SpellingError(Exception):
+    def __init__(self, path, errors):
+        self.path = path
+        self.message = "%d spellng errors" % errors
 
+    def __str__(self):
+        return self.message
 
-class CodeFormatter(Formatter):
-    """
-    Retrieve human text from the code.
 
-    The flow:
-     1. collect all comments and doc strings
-     2. strip tech text
-         * fenced block - multi-line text between 3 back ticks, similar to
-           `<pre>` tag
-         * in-line code - text between back ticks, similar to `<code>`
-         * special comment - e.g. `noqa`, `pylint`
-         * custom regex - lines matching user-defined regex
-    """
+def hunspell_run(path, code, dict_fname):
+    p = sp.Popen(
+        ["hunspell", "-a", "-p", dict_fname],
+        universal_newlines=True,
+        stdin=sp.PIPE,
+        stdout=sp.PIPE,
+    )
+
+    # read one-line header
+    p.stdout.readline()
 
-    # comment directive consists from 3 parts: header, command and value.
-    # for example: `docspell: accept foo,bar`
-    comment_prefix = "docspell"
-    command_accept_len = 2
-
-    def __init__(self, comment_delims, ignore_lines, **options):
-        log.debug("%s init", self.__class__.__name__)
-        log.debug("arg: comment_delims '%s'", comment_delims)
-        log.debug("arg: ignore_lines '%s'", ignore_lines)
-        log.debug("arg: options '%s'", options)
-        Formatter.__init__(self, **options)
-        self.comment_delims = comment_delims
-        self.ignore_lines = ignore_lines
-        self.spell_dict = []
-
-    def format(self, tokensource, outfile):  # noqa: A003
-        txt = self.tr_code(tokensource)
-        txt = self.tr_comment_delims(txt)
-        txt = self.tr_line(txt)
-        txt = self.tr_directive(txt)
-        txt = self.tr_md_code_block(txt)
-        txt = self.tr_md_code(txt)
-        outfile.write(txt)
-
-    def tr_code(self, tokensource):
-        tokens = []
-        for ttype, value in tokensource:
-            if log.getEffectiveLevel() == logging.DEBUG:
-                log.debug(
-                    "token: type %s, value '%s'", ttype, value.replace("\n", "\\n")
-                )
-            if (
-                ttype == Token.Comment
-                or ttype == Token.Comment.Single
-                or ttype == Token.Comment.Multiline
-                or ttype == Token.Literal.String.Doc
-            ):
-                log.debug("token: accept")
-                nv = value
-            else:
-                nv = tr(value)
-            tokens.append(nv)
-        return "".join(tokens)
-
-    def tr_comment_delims(self, txt):
-        if not self.comment_delims:
-            return txt
-        prefix_reg = [re.escape(i) for i in self.comment_delims]
-        reg = "(?m)^[ \\t]*(" + "|".join(prefix_reg) + ")"
-        return re.sub(reg, repl, txt)
-
-    def tr_line(self, txt):
-        if not self.ignore_lines:
-            return txt
-        line_reg = [re.escape(i) for i in self.ignore_lines]
-        reg = "(?m)^[ \\t]*(" + "|".join(line_reg) + ")(\\W.*)?$"
-        return re.sub(reg, repl, txt)
-
-    def tr_directive(self, txt):
-        line_reg = [re.escape(self.comment_prefix)]
-        reg = "(?m)^[ \\t]*(" + "|".join(line_reg) + ")(\\W.*)?$"
-        return re.sub(reg, self.mk_dict, txt)
-
-    def mk_dict(self, matchobj):
-        otxt = txt = matchobj.group(0)
-        # rm leading '#'
-        txt = txt.split(None, 1)[-1]
-        txt = txt.split()
-        log.debug("internal command: %s", txt)
-        if len(txt) == self.command_accept_len and txt[0] == "accept":
-            log.debug("accept words '%s'", txt[1])
-            self.spell_dict += txt[1].split(",")
-        return tr(otxt)
-
-    def tr_md_code(self, txt):
-        reg = "(?P<open>`+)[^`\\n]+?(?P=open)"
-        return re.sub(reg, repl, txt)
-
-    def tr_md_code_block(self, txt):
-        reg_indent = "(?P<indent>^[ \\t]*)"
-        reg = "(?m)" + reg_indent + "(?P<open>`{3,})[ \\t]*$\\n"
-        reg += "((?P=indent).*$\\n)*?"
-        reg += "(?P=indent)(?P=open)[ \\t]*$"
-        return re.sub(reg, repl, txt)
+    errors = 0
+    for no, line in enumerate(code.splitlines()):
+        if line == "" or line.isspace():
+            continue
+        log.debug("line %d '%s'", no, line)
+        for wm in re.finditer("\\b\\w+\\b", line):
+            log.debug(">> %s", wm.group(0))
+            # feed a line with one word
+            p.stdin.write(wm.group(0) + "\n")
+            p.stdin.flush()
+            # read an answer for a word
+            txt = p.stdout.readline().strip()
+            # read an answer for a line
+            p.stdout.readline()
+            log.debug("<< '%s'", txt)
+            if txt == "*":
+                continue
+            errors += 1
+            msg = "%s:%s:%s: %s" % (path, no + 1, wm.start(0), txt)
+            print(msg, file=sys.stderr)
+    return errors
 
 
 def hunspell(code, path, conf, spell_dict):
     """
     Pipe code to `hunspell` and print errors in gcc format `file:line:column`.
 
     `spell_dict` is a personal dictionary. Is is loaded for the single run and
     not saved to disk.
     """
-    tconf = conf.get("hunspell", {})
-    log.debug("tconf: %s", prettify(tconf))
-
+    tconf = conf["hunspell"]
     # add personal word list
     dict_fp, dict_fname = tempfile.mkstemp(prefix="doc-spell-dict-")
     dict_fp = open(dict_fname, "w")
 
     def add_word_list(name, words):
         log.debug("add dictionary '%s'", name)
         for word in words:
@@ -178,150 +108,160 @@
 
     # save code for debugging
     code_fp, code_fname = tempfile.mkstemp(prefix="doc-spell-code-")
     code_fp = open(code_fname, "w")
     code_fp.write(code)
     code_fp.close()
 
-    p = sp.Popen(
-        ["hunspell", "-a", "-p", dict_fname],
-        universal_newlines=True,
-        stdin=sp.PIPE,
-        stdout=sp.PIPE,
-    )
-
-    # read one-line header
-    p.stdout.readline()
-
-    rc = True
-    for no, line in enumerate(code.splitlines()):
-        if line == "" or line.isspace():
-            continue
-        log.debug("line %d '%s'", no, line)
-        for wm in re.finditer("\\b\\w+\\b", line):
-            log.debug(">> %s", wm.group(0))
-            # feed a line with one word
-            p.stdin.write(wm.group(0) + "\n")
-            p.stdin.flush()
-            # read an answer for a word
-            txt = p.stdout.readline().strip()
-            # read an answer for a line
-            p.stdout.readline()
-            log.debug("<< '%s'", txt)
-            if txt == "*":
-                continue
-            rc = False
-            msg = "%s:%s:%s: %s" % (path, no + 1, wm.start(0), txt)
-            print(msg, file=sys.stderr)
-
+    errors = hunspell_run(path, code, dict_fname)
     if log.getEffectiveLevel() != logging.DEBUG:
         os.unlink(dict_fname)
         os.unlink(code_fname)
     else:
         log.debug("remove tmp code: %s", code_fname)
         log.debug("remove tmp dict: %s", dict_fname)
-    return rc
+    if errors:
+        raise SpellingError(path, errors)
+
+
+# }}} noqa ERA001
+
+
+class UnsupportedFileError(Exception):
+    def __init__(self, path, msg):
+        self.path = path
+        self.message = "unsupported file type: " + msg
+
+    def __str__(self):
+        return self.message
 
 
 # weights of lexer aliases, to find best match
 aliases = {
+    "text": -1,
     "shell": 1,
     "bash": 2,
     "c": 1,
     "c++": 2,
 }
 
 
-def get_lexer(tags, *, debug=False):
-    log.debug("search for lexer")
-    rc = (None, None)
+def get_lexer(path, *, debug=False):
+    tags = identify.tags_from_path(path)
+    if "symlink" in tags:
+        path = os.path.realpath(path)
+        log.debug("redirect to '%s'", path)
+        tags = identify.tags_from_path(path)
+
+    accept = {"file", "text"}
+    rc = accept - tags
+    if len(rc):
+        raise UnsupportedFileError(path, "not a text file")
+
+    if "plain-text" in tags:
+        return get_lexer_by_name("text", stripall=False)
+
+    tags = tags - accept
+    tags = tags - {"executable", "non-executable"}
+    tags = sorted(tags, key=lambda x: aliases.get(x, 0), reverse=True)
+    log.debug("get lexer from identify tags %s", tags)
+    rc = None
     for tag in tags:
         try:
-            lexer = get_lexer_by_name(tag, stripall=True)
+            lexer = get_lexer_by_name(tag, stripall=False)
         except Exception:
             lexer = None
-        log.debug("tag %s, lexer %s", tag, lexer)
-        if rc == (None, None):
-            rc = (lexer, tag)
+        log.debug("lexer for '%s': %s", tag, lexer)
+        if rc is None:
+            rc = lexer
         if not debug:
             break
-    return rc
+    if rc:
+        return rc
 
-
-def parse_rule(rule, comment_delims, ignore_lines):
-    log.debug("matched rule %s", rule)
-    err = "configuration error: rule '%s'" % rule["name"]
-
-    def get_list(key, dst):
-        tmp = rule.get(key, [])
-        if tmp is None:
-            return
-        if not isinstance(tmp, list):
-            log.error("%s: '%s' must be a list", err, key)
-            sys.exit(1)
-        dst += tmp
-
-    get_list("comment-delims", comment_delims)
-    get_list("ignore-lines", ignore_lines)
+    log.debug("get lexer from guess_lexer_for_filename")
+    buf = open(path, "r").read(1024)
+    try:
+        return guess_lexer_for_filename(path, buf)
+    except Exception:
+        return None
+
+
+doc_types = {
+    "text",
+    "html",
+    "markdown",
+    "xml",
+    "qml",
+    "rst",
+    "xhtml",
+    "pug",
+    "jade",
+    "scaml",
+    "xslt",
+}
 
 
 def get_formatter(conf, tags):
-    comment_delims = []
-    ignore_lines = []
-    log.debug("search configuration for matching rules")
-    for r in conf["rules"]:
-        if r["tag"] in tags:
-            parse_rule(r, comment_delims, ignore_lines)
-    comment_delims = list(set(comment_delims))
-    ignore_lines = list(set(ignore_lines))
-    return CodeFormatter(comment_delims=comment_delims, ignore_lines=ignore_lines)
+    stags = set(tags)
+    rc = stags - doc_types
+    if len(stags) != len(rc):
+        return None
+
+    def rule_get_value(rule, name, keys):
+        try:
+            for key in keys:
+                rule = rule.get(key)
+        except Exception:
+            rule = None
+        log.debug("rule '%s', path %s, value %s", name, keys, rule)
+        return rule
+
+    def rule_match(r, name, stags):
+        rtypes = rule_get_value(r, name, ["match", "types"])
+        if rtypes is None:
+            return False
+        if "*" in rtypes:
+            log.debug("rule '%s', match by type '*'", name)
+            return True
+        rc = stags.intersection(set(rtypes))
+        if len(rc):
+            log.debug("rule '%s', match by type %s", name, rc)
+            return True
+        return False
+
+    kwargs = {}
+    ignore_keys = ["block-marks", "custom", "linters"]
+    for no, rule in enumerate(conf["rules"]):
+        name = "%d %s" % (no, rule.get("name", "noname"))
+        if not rule_match(rule, name, stags):
+            continue
+        ignore = rule_get_value(rule, name, ["ignore"])
+        if ignore is None:
+            continue
+        for k, v in ignore.items():
+            if k in ignore_keys and v and isinstance(v, list):
+                kwargs[k] = kwargs.get(k, []) + v
+    log.debug("kwargs %s", prettify(kwargs))
+    return CodeFormatter(kwargs)
 
 
 def spell_checker(path, conf):
     """
     Obtain human text from the code and pipe it via hunspell.
 
     In case of spelling errors, raises an exception.
     """
-    log.info("check '%s'", path)
-    tags = identify.tags_from_path(path)
-    if "symlink" in tags:
-        path = os.readlink(path)
-        log.info("redirect to '%s'", path)
-        tags = identify.tags_from_path(path)
-    log.debug("identify %s", tags)
-    accept = {"file", "text"}
-    rc = accept - tags
-    if len(rc):
-        log.error("only text files are supported")
-        msg = "%s: unsupported type %s" % (path, tags)
-        raise Exception(msg)
-
-    doc_types = {
-        "html",
-        "markdown",
-        "xml",
-        "qml",
-        "rst",
-        "xhtml",
-        "pug",
-        "jade",
-        "scaml",
-        "xslt",
-    }
-    rc = doc_types - tags
-    if len(rc) != len(doc_types):
-        log.error("only programming languages are supported, no markup")
-        msg = "%s: unsupported type %s" % (path, tags)
-        raise Exception(msg)
-
-    tags = tags - accept
-    tags = tags - {"executable", "non-executable", "plain-text"}
-    tags = sorted(tags, key=lambda x: aliases.get(x, -1), reverse=True)
-    log.debug("sorted tags %s", tags)
-    lexer, tag = get_lexer(tags, debug=True)
+    log.info("%s: starting", path)
+    lexer = get_lexer(path, debug=True)
+    log.debug("lexer: %s, aliases %s", lexer, lexer.aliases if lexer else None)
+    if not lexer:
+        raise UnsupportedFileError(path, "no lexer found")
+    tags = [t.split("+")[0] for t in lexer.aliases]
+    tags = list(set(tags))
+    log.info("%s: associated types: %s", path, lexer.aliases)
     formatter = get_formatter(conf, tags)
+    if not formatter:
+        raise UnsupportedFileError(path, "no formatter found")
     code = open(path, "r").read()
     code = highlight(code, lexer, formatter)
-    if not hunspell(code, path, conf, formatter.spell_dict):
-        msg = "spelling errors in '%s'" % path
-        raise Exception(msg)
+    hunspell(code, path, conf, formatter.spell_dict)
```

## doc_spell/__version__.py

```diff
@@ -1 +1 @@
-__version__ = '0.1.0'
+__version__ = '0.2.0'
```

## Comparing `doc_spell-0.1.0.dist-info/METADATA` & `doc_spell-0.2.0.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: doc-spell
-Version: 0.1.0
+Version: 0.2.0
 Summary: code documentation spell checker
 Author-email: Anatoly Asviyan <aanatoly@gmail.com>
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
 Requires-Dist: identify
 Requires-Dist: pyaml
 Requires-Dist: pydevkit<4.0.0,>=3.1.2
 Requires-Dist: pygments
+Requires-Dist: schema
 Project-URL: Homepage, https://github.com/aanatoly/doc-spell
 Project-URL: Repository, https://github.com/aanatoly/doc-spell
 Description-Content-Type: text/markdown
 
 # doc spell
 
 Code documentation spell checker.
```

## Comparing `doc_spell-0.1.0.dist-info/licenses/LICENSE` & `doc_spell-0.2.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `doc_spell-0.1.0.dist-info/RECORD` & `doc_spell-0.2.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,12 @@
+doc_spell/.doc-spell.yml,sha256=lzqF24tSKo8wars2IXq3sWtZ_ZRuBUrwbHldDKfqI6g,856
 doc_spell/__init__.py,sha256=z6wfs6rLKrBxFKviVD4mhopUYd8p9VKRhEIsCmVDZ1I,160
-doc_spell/__main__.py,sha256=Qq7VR5ga6cVyFuOSQzJAlLhP8rXztOM--wG0BIM7FcM,1439
-doc_spell/cspell.py,sha256=iCvU9S8-gWdneLASwXhv0J6BquPMJLMf0qjL9NjkygI,9848
-doc_spell/__version__.py,sha256=L6zbQIZKsAP-Knhm6fBcQFPoVdIDuejxze60qX23jiw,21
-doc_spell-0.1.0.dist-info/entry_points.txt,sha256=lR1yKMV6utzwatjTlaDOc1oYbKLbV_jwoa03FGhvSTM,53
-doc_spell-0.1.0.dist-info/WHEEL,sha256=B19PGBCYhWaz2p_UjAoRVh767nYQfk14Sn4TpIZ-nfU,87
-doc_spell-0.1.0.dist-info/METADATA,sha256=kwX4pbCdpcXaKRNoKd3kugpaJMt9cMl-LgKa5OkHT0o,1201
-doc_spell-0.1.0.dist-info/licenses/LICENSE,sha256=TZ52n6XUyJFPMHXZ2evCCSYnunrYn-7LRPZV8n4FvSw,1103
-doc_spell-0.1.0.dist-info/RECORD,,
+doc_spell/__main__.py,sha256=y_cBrCcxH5-YWdGMqBsKDIlzFwyYwFDP5rCjr1WuKLs,2050
+doc_spell/conf.py,sha256=eSlHLxXzMnVCrUVnEzpDGI6c5XbMPBqvB2x5p5Lk_R0,1592
+doc_spell/cspell.py,sha256=godZbCllau0P4-fto2F0NAlV90gDk-kuFRZ4yFtrBQM,7316
+doc_spell/formatters.py,sha256=W4nG-7nXx1tz6wtQn9wxBBkfifUy0_fAExpge0pAU8w,5470
+doc_spell/__version__.py,sha256=clN3TnyYyt5T_wUJLVBmutS2kYLLBET4JFB2QXnRm2Q,21
+doc_spell-0.2.0.dist-info/entry_points.txt,sha256=lR1yKMV6utzwatjTlaDOc1oYbKLbV_jwoa03FGhvSTM,53
+doc_spell-0.2.0.dist-info/WHEEL,sha256=B19PGBCYhWaz2p_UjAoRVh767nYQfk14Sn4TpIZ-nfU,87
+doc_spell-0.2.0.dist-info/METADATA,sha256=AU3gLcQeLu68pa6ER400_kSJd939ObrbKNOCG-V3GHU,1223
+doc_spell-0.2.0.dist-info/licenses/LICENSE,sha256=TZ52n6XUyJFPMHXZ2evCCSYnunrYn-7LRPZV8n4FvSw,1103
+doc_spell-0.2.0.dist-info/RECORD,,
```

