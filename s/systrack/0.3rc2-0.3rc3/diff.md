# Comparing `tmp/systrack-0.3rc2.tar.gz` & `tmp/systrack-0.3rc3.tar.gz`

## Comparing `systrack-0.3rc2.tar` & `systrack-0.3rc3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 systrack-0.3rc2/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/__init__.py
--rw-r--r--   0        0        0    11563 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/__main__.py
--rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/elf.py
--rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/kconfig.py
--rw-r--r--   0        0        0    26320 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/kconfig_options.py
--rw-r--r--   0        0        0    21459 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/kernel.py
--rw-r--r--   0        0        0    15255 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/location.py
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/output.py
--rw-r--r--   0        0        0     6131 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/signature.py
--rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/syscall.py
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/type_hints.py
--rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/utils.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/version.py
--rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/arch/__init__.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/arch/all.py
--rw-r--r--   0        0        0    10299 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/arch/arch_base.py
--rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/arch/arm.py
--rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/arch/arm64.py
--rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/arch/mips.py
--rw-r--r--   0        0        0     9665 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/arch/powerpc.py
--rw-r--r--   0        0        0    10348 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/arch/x86.py
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/templates/syscall_table.css
--rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/templates/syscall_table.html
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 systrack-0.3rc2/src/systrack/templates/syscall_table.js
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 systrack-0.3rc2/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 systrack-0.3rc2/LICENSE
--rw-r--r--   0        0        0     5862 2020-02-02 00:00:00.000000 systrack-0.3rc2/README.md
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 systrack-0.3rc2/pyproject.toml
--rw-r--r--   0        0        0    47672 2020-02-02 00:00:00.000000 systrack-0.3rc2/PKG-INFO
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 systrack-0.3rc3/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/__init__.py
+-rw-r--r--   0        0        0    11563 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/__main__.py
+-rw-r--r--   0        0        0     5263 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/elf.py
+-rw-r--r--   0        0        0     3371 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/kconfig.py
+-rw-r--r--   0        0        0    26320 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/kconfig_options.py
+-rw-r--r--   0        0        0    21459 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/kernel.py
+-rw-r--r--   0        0        0    15450 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/location.py
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/output.py
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/signature.py
+-rw-r--r--   0        0        0     2038 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/syscall.py
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/type_hints.py
+-rw-r--r--   0        0        0     9623 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/utils.py
+-rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/version.py
+-rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/arch/__init__.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/arch/all.py
+-rw-r--r--   0        0        0    10931 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/arch/arch_base.py
+-rw-r--r--   0        0        0     5738 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/arch/arm.py
+-rw-r--r--   0        0        0     2312 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/arch/arm64.py
+-rw-r--r--   0        0        0     3903 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/arch/mips.py
+-rw-r--r--   0        0        0     9917 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/arch/powerpc.py
+-rw-r--r--   0        0        0    10348 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/arch/x86.py
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/templates/syscall_table.css
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/templates/syscall_table.html
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 systrack-0.3rc3/src/systrack/templates/syscall_table.js
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 systrack-0.3rc3/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 systrack-0.3rc3/LICENSE
+-rw-r--r--   0        0        0     5862 2020-02-02 00:00:00.000000 systrack-0.3rc3/README.md
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 systrack-0.3rc3/pyproject.toml
+-rw-r--r--   0        0        0    47672 2020-02-02 00:00:00.000000 systrack-0.3rc3/PKG-INFO
```

### Comparing `systrack-0.3rc2/CHANGELOG.md` & `systrack-0.3rc3/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc2/src/systrack/__main__.py` & `systrack-0.3rc3/src/systrack/__main__.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc2/src/systrack/elf.py` & `systrack-0.3rc3/src/systrack/elf.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc2/src/systrack/kconfig.py` & `systrack-0.3rc3/src/systrack/kconfig.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc2/src/systrack/kconfig_options.py` & `systrack-0.3rc3/src/systrack/kconfig_options.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc2/src/systrack/kernel.py` & `systrack-0.3rc3/src/systrack/kernel.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc2/src/systrack/location.py` & `systrack-0.3rc3/src/systrack/location.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,19 +65,23 @@
 		if path.is_file() and path.match('*.c'):
 			yield from grep_file(root, exp, path)
 		elif path.is_dir() and path.resolve() not in exclude:
 			yield from grep_recursive(root, exp, exclude, path)
 
 def grep_kernel_sources(kdir: Path, arch: Arch, syscalls: List[Syscall]) -> Iterator[Tuple[Syscall,Path,int]]:
 	if arch.compat:
-		exp = rb'\b(COMPAT_)?SYSCALL(32)?_DEFINE\d\s*\(\s*\w+'
+		base_exp = r'\b(COMPAT_)?SYSCALL(32)?_DEFINE\d\s*\('
 	elif arch.bits32:
-		exp = rb'\bSYSCALL(32)?_DEFINE\d\s*\(\s*\w+'
+		base_exp = r'\bSYSCALL(32)?_DEFINE\d\s*\('
 	else:
-		exp = rb'\bSYSCALL_DEFINE\d\s*\(\s*\w+'
+		base_exp = r'\bSYSCALL_DEFINE\d\s*\('
+
+	oddstyle = arch.syscall_def_regexp()
+	if oddstyle is not None:
+		base_exp = f'(({base_exp})|({oddstyle}))'
 
 	if not command_available('rg'):
 		logging.debug('No ripgrep available :( falling back to slow python implementation')
 
 		exclude = {
 			(kdir / 'Documentation').resolve(),
 			(kdir / 'drivers').resolve(),
@@ -85,37 +89,36 @@
 			(kdir / 'tools').resolve(),
 		}
 
 		for path in (kdir / 'arch').iterdir():
 			if not path.match(arch.name):
 				exclude.add(path.resolve())
 
-		out = list(grep_recursive(kdir, re.compile(exp), exclude))
+		out = list(grep_recursive(kdir, re.compile(base_exp + r'\s*\w+'), exclude))
 	else:
 		out = ensure_command((
 			'rg', '--line-number',
 			'--glob', '!Documentation/*',
 			'--glob', '!drivers/*',
 			'--glob', '!samples/*',
 			'--glob', '!tools/*',
 			'--glob', '!arch/*',           # ignore other architectures (important)
 			'--glob', f'arch/{arch.name}', # include the correct one
 			'--glob', '*.c',
-			exp
+			base_exp + r'\s*\w+'
 		), cwd=kdir).splitlines()
 
+	exps = {s: re.compile(rf':{base_exp}{s.origname}[,)]') for s in syscalls}
+
 	if arch.compat:
-		exps = {s: re.compile(rf':(COMPAT_)?SYSCALL(32)?_DEFINE\d\({s.origname}[,)]') for s in syscalls}
-		key  = lambda l: (l.startswith('arch'), ('COMPAT' in l) + ('SYSCALL32' in l))
+		key = lambda l: (l.startswith('arch'), ('COMPAT' in l) + ('SYSCALL32' in l))
 	elif arch.bits32:
-		exps = {s: re.compile(rf':SYSCALL(32)?_DEFINE\d\({s.origname}[,)]') for s in syscalls}
-		key  = lambda l: (l.startswith('arch'), 'SYSCALL32' in l)
+		key = lambda l: (l.startswith('arch'), 'SYSCALL32' in l)
 	else:
-		exps = {s: re.compile(rf':SYSCALL_DEFINE\d\({s.origname}[,)]') for s in syscalls}
-		key  = lambda l: l.startswith('arch')
+		key = lambda l: l.startswith('arch')
 
 	# Prioritize files under arch/ and prefer compat/32bit syscalls if needed
 	out.sort(key=key, reverse=True)
 
 	for line in out:
 		for sc, exp in tuple(exps.items()):
 			if exp.search(line):
@@ -138,15 +141,22 @@
 
 		definition = f.readline().decode()
 
 	# There are a lot of legacy/weird syscall definitions and some symbols can
 	# therefore point (addr2line output) to old-style `asmlinkage` functions
 	newstyle = ('^(COMPAT_)?' if arch.compat else '^') + rf'SYSCALL(32)?_DEFINE\d\({name}'
 	oldstyle = rf'^asmlinkage \w+' + (rf' sys(32)?_{name}\(' if name else '')
-	return re.match(f'{oldstyle}|{newstyle}', definition) is not None
+
+	if re.match(f'{oldstyle}|{newstyle}', definition) is not None:
+		return True
+
+	# Some archs use weirdly named SYSCALL_DEFINEn macros, e.g. PPC32 ABI on
+	# PowerPC 64-bit with its "PPC32_SYSCALL_DEFINEn".
+	oddstyle = arch.syscall_def_regexp(name)
+	return oddstyle is not None and re.match(oddstyle, definition) is not None
 
 def adjust_line(file: Path, line: int) -> int:
 	try:
 		with file.open('rb') as f:
 			lines = f.readlines()
 	except FileNotFoundError:
 		# This will happen if we mismatch vmlinux and kernel sources. There's no
```

### Comparing `systrack-0.3rc2/src/systrack/output.py` & `systrack-0.3rc3/src/systrack/output.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc2/src/systrack/signature.py` & `systrack-0.3rc3/src/systrack/signature.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,17 @@
 			sig += f.readline().strip()
 
 	# We only handle two scenarios here:
 	#
 	#     SYSCALL_DEFINEx(name, type1, arg1, type2, arg2, ...)
 	#     asmlinkage xxx sys_xxx(type1 arg1, type2 arg2, ...)
 
-	newsig = noprefix(sig, 'SYSCALL_DEFINE', 'SYSCALL32_DEFINE', 'COMPAT_SYSCALL_DEFINE', 'COMPAT_SYSCALL32_DEFINE')
+	newsig = noprefix(sig, 'SYSCALL_DEFINE', 'SYSCALL32_DEFINE',
+		'COMPAT_SYSCALL_DEFINE', 'COMPAT_SYSCALL32_DEFINE',
+		'PPC32_SYSCALL_DEFINE')
 
 	if sig != newsig:
 		sig = newsig
 		start = sig.find(',') + 1
 		nargs = int(sig[0])
 		assert nargs <= 6, f'SYSCALL_DEFINE{nargs}? {file}:{line}'
```

### Comparing `systrack-0.3rc2/src/systrack/syscall.py` & `systrack-0.3rc3/src/systrack/syscall.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc2/src/systrack/utils.py` & `systrack-0.3rc3/src/systrack/utils.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc2/src/systrack/arch/__init__.py` & `systrack-0.3rc3/src/systrack/arch/__init__.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc2/src/systrack/arch/arch_base.py` & `systrack-0.3rc3/src/systrack/arch/arch_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -264,7 +264,21 @@
 		The returned value is a list of tuples of the form: (number, name,
 		symbol_name, signature, kconfig_opts).
 
 		NOTE: the symbol_name that is returned needs to exist in the given
 		vmlinux.
 		'''
 		return []
+
+	def syscall_def_regexp(self, syscall_name: Optional[str]=None) -> Optional[str]:
+		'''Return a regexp capable of matching syscall definitions using
+		arch-specific SYSCALL_DEFINEx macros with weird names. If syscall_name
+		is given, return a regexp to match this syscall definition exactly,
+		otherwise just a generic one.
+
+		With syscall_name: the returned regexp should match a macro call up to
+		and including the syscall name, e.g., "SYSCALL_DEFINE3(name".
+
+		Without syscall_name: the returned regexp should match the macro call up
+		to and including the first open parenthesis, e.g., "SYSCALL_DEFINE3(".
+		'''
+		return None
```

### Comparing `systrack-0.3rc2/src/systrack/arch/arm.py` & `systrack-0.3rc3/src/systrack/arch/arm.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc2/src/systrack/arch/arm64.py` & `systrack-0.3rc3/src/systrack/arch/arm64.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc2/src/systrack/arch/mips.py` & `systrack-0.3rc3/src/systrack/arch/mips.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc2/src/systrack/arch/powerpc.py` & `systrack-0.3rc3/src/systrack/arch/powerpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -230,7 +230,15 @@
 
 			if len(insns) < 2 or (insns[1] & 0xffff0000) != 0x41c20000: # beq- xxx
 				return []
 
 		# We have the syscall
 		kconf = 'PPC_FAST_ENDIAN_SWITCH' if self.kernel_version >= (4,15) else None
 		return [(0x1ebe, 'switch_endian', exc.name, (), kconf)]
+
+	def syscall_def_regexp(self, syscall_name: Optional[str]=None) -> Optional[str]:
+		if self.abi != 'ppc32':
+			return None
+
+		if syscall_name is not None:
+			return rf'^PPC32_SYSCALL_DEFINE\d\({syscall_name}'
+		return r'\bPPC32_SYSCALL_DEFINE\d\s*\('
```

### Comparing `systrack-0.3rc2/src/systrack/arch/x86.py` & `systrack-0.3rc3/src/systrack/arch/x86.py`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc2/src/systrack/templates/syscall_table.css` & `systrack-0.3rc3/src/systrack/templates/syscall_table.css`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc2/src/systrack/templates/syscall_table.html` & `systrack-0.3rc3/src/systrack/templates/syscall_table.html`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc2/src/systrack/templates/syscall_table.js` & `systrack-0.3rc3/src/systrack/templates/syscall_table.js`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc2/LICENSE` & `systrack-0.3rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc2/README.md` & `systrack-0.3rc3/README.md`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc2/pyproject.toml` & `systrack-0.3rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `systrack-0.3rc2/PKG-INFO` & `systrack-0.3rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systrack
-Version: 0.3rc2
+Version: 0.3rc3
 Summary: Linux kernel syscall implementation tracker
 Project-URL: homepage, https://github.com/mebeim/systrack
 Project-URL: repository, https://github.com/mebeim/systrack.git
 Author-email: Marco Bonelli <marco@mebeim.net>
 Maintainer-email: Marco Bonelli <marco@mebeim.net>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

