# Comparing `tmp/prompt_toolkit-3.0.8.tar.gz` & `tmp/prompt_toolkit-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/prompt_toolkit-3.0.8.tar", last modified: Mon Oct 12 14:58:14 2020, max compression
+gzip compressed data, was "dist/prompt_toolkit-3.0.9.tar", last modified: Tue Jan  5 09:05:13 2021, max compression
```

## Comparing `prompt_toolkit-3.0.8.tar` & `prompt_toolkit-3.0.9.tar`

### file list

```diff
@@ -1,400 +1,400 @@
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:14.004594 prompt_toolkit-3.0.8/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       13 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/.codecov.yml
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      423 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/.gitignore
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      773 2020-09-23 19:10:55.000000 prompt_toolkit-3.0.8/.travis.yml
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      148 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/AUTHORS.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    66169 2020-10-12 14:54:36.000000 prompt_toolkit-3.0.8/CHANGELOG
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1493 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/LICENSE
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      133 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/MANIFEST.in
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8164 2020-10-12 14:58:14.004594 prompt_toolkit-3.0.8/PKG-INFO
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4453 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/PROJECTS.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6034 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.8/README.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      997 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/appveyor.yml
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.524595 prompt_toolkit-3.0.8/docs/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6794 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/Makefile
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8581 2020-10-12 14:55:29.000000 prompt_toolkit-3.0.8/docs/conf.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.588595 prompt_toolkit-3.0.8/docs/images/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    72983 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/auto-suggestion.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    77372 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/bottom-toolbar.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    94994 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/colored-prompt.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    95099 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/colorful-completions.png
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.616595 prompt_toolkit-3.0.8/docs/images/dialogs/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   134890 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/dialogs/button.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   135405 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/dialogs/confirm.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   140141 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/dialogs/inputbox.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   139732 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/dialogs/messagebox.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   144850 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/dialogs/styled.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   105790 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/hello-world-prompt.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    92781 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/html-completion.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   116804 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/html-input.png
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)    56254 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/logo_400px.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    85296 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/multiline-input.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    81683 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/number-validator.png
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.632595 prompt_toolkit-3.0.8/docs/images/progress-bars/
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     5411 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/progress-bars/apt-get.png
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     8575 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/progress-bars/colored-title-and-label.png
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     8191 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/progress-bars/custom-key-bindings.png
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)    13218 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/progress-bars/simple-progress-bar.png
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     9723 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/progress-bars/two-tasks.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   133464 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/ptpython-2.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   103337 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/ptpython-history-help.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    60225 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/ptpython-menu.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    28700 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/ptpython.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   205809 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/pymux.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   150054 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/pyvim.png
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.656595 prompt_toolkit-3.0.8/docs/images/repl/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   125880 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/repl/sqlite-1.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   171192 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/repl/sqlite-2.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   126517 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/repl/sqlite-3.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   190998 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/repl/sqlite-4.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   182631 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/repl/sqlite-5.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   200352 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/repl/sqlite-6.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    79787 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/images/rprompt.png
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2716 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.8/docs/index.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6699 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/make.bat
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.676595 prompt_toolkit-3.0.8/docs/pages/
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.696595 prompt_toolkit-3.0.8/docs/pages/advanced_topics/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5484 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/pages/advanced_topics/architecture.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      794 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/docs/pages/advanced_topics/asyncio.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5714 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/pages/advanced_topics/filters.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      255 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.8/docs/pages/advanced_topics/index.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1455 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.8/docs/pages/advanced_topics/input_hooks.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12639 2020-07-30 11:15:49.000000 prompt_toolkit-3.0.8/docs/pages/advanced_topics/key_bindings.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3712 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/pages/advanced_topics/rendering_flow.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7337 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/pages/advanced_topics/rendering_pipeline.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10561 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/pages/advanced_topics/styling.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    32545 2020-09-14 23:38:45.000000 prompt_toolkit-3.0.8/docs/pages/asking_for_input.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9356 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.8/docs/pages/dialogs.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    18142 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.8/docs/pages/full_screen_apps.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      588 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/pages/gallery.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2848 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/docs/pages/getting_started.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9210 2020-10-12 13:56:12.000000 prompt_toolkit-3.0.8/docs/pages/printing_text.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7394 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/docs/pages/progress_bars.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5793 2020-07-30 11:15:49.000000 prompt_toolkit-3.0.8/docs/pages/reference.rst
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.700595 prompt_toolkit-3.0.8/docs/pages/tutorials/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      101 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/docs/pages/tutorials/index.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12329 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/docs/pages/tutorials/repl.rst
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.704594 prompt_toolkit-3.0.8/docs/pages/upgrading/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9591 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/docs/pages/upgrading/2.0.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3577 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/docs/pages/upgrading/3.0.rst
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      108 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/docs/pages/upgrading/index.rst
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.704594 prompt_toolkit-3.0.8/examples/
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.716595 prompt_toolkit-3.0.8/examples/dialogs/
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      386 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/examples/dialogs/button_dialog.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1055 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/dialogs/checkbox_dialog.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      314 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/dialogs/input_dialog.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      303 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/dialogs/messagebox.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      358 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/dialogs/password_dialog.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1158 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/dialogs/progress_dialog.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1080 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/dialogs/radio_dialog.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      931 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/dialogs/styled_messagebox.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      334 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/dialogs/yes_no_dialog.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.728594 prompt_toolkit-3.0.8/examples/full-screen/
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2389 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/full-screen/buttons.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2819 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/full-screen/calculator.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      159 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/examples/full-screen/dummy-app.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     5605 2020-09-14 23:38:45.000000 prompt_toolkit-3.0.8/examples/full-screen/full-screen-demo.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      938 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/examples/full-screen/hello-world.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      155 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/examples/full-screen/no-layout.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2500 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/examples/full-screen/pager.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.744594 prompt_toolkit-3.0.8/examples/full-screen/simple-demos/
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1959 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/full-screen/simple-demos/alignment.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2139 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/full-screen/simple-demos/autocompletion.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1869 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/full-screen/simple-demos/colorcolumn.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1870 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/full-screen/simple-demos/cursorcolumn-cursorline.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2743 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/full-screen/simple-demos/float-transparency.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     3429 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/full-screen/simple-demos/floats.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2775 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/full-screen/simple-demos/focus.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     7320 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/full-screen/simple-demos/horizontal-align.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      949 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/full-screen/simple-demos/horizontal-split.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     3146 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/full-screen/simple-demos/line-prefixes.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2184 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/full-screen/simple-demos/margins.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     5530 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/full-screen/simple-demos/vertical-align.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      944 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/full-screen/simple-demos/vertical-split.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     5144 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/full-screen/split-screen.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     9221 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/examples/full-screen/text-editor.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      686 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/examples/gevent-get-input.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.756595 prompt_toolkit-3.0.8/examples/print-text/
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     3083 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/print-text/ansi-colors.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1187 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/print-text/ansi.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1330 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/print-text/html.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      883 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/print-text/named-colors.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1097 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/examples/print-text/print-formatted-text.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      331 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/examples/print-text/print-frame.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1230 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/print-text/pygments-tokens.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1024 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/print-text/true-color-demo.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.776594 prompt_toolkit-3.0.8/examples/progress-bar/
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1903 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/progress-bar/a-lot-of-parallel-tasks.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      537 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/progress-bar/colored-title-and-label.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1211 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/progress-bar/custom-key-bindings.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1591 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/progress-bar/many-parallel-tasks.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      601 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/progress-bar/nested-progress-bars.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      532 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/progress-bar/scrolling-task-name.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      325 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/progress-bar/simple-progress-bar.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      862 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/progress-bar/styled-1.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1347 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/progress-bar/styled-2.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      941 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/progress-bar/styled-apt-get-install.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      932 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/progress-bar/styled-rainbow.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1108 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/examples/progress-bar/styled-tqdm-1.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1034 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/examples/progress-bar/styled-tqdm-2.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      929 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/progress-bar/two-tasks.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      516 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/progress-bar/unknown-length.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.824594 prompt_toolkit-3.0.8/examples/prompts/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      467 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/accept-default.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1957 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/asyncio-prompt.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.844594 prompt_toolkit-3.0.8/examples/prompts/auto-completion/
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1410 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/auto-completion/autocomplete-with-control-space.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1122 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/auto-completion/autocompletion-like-readline.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1198 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/auto-completion/autocompletion.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     3758 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/auto-completion/colored-completions-with-formatted-text.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1937 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/auto-completion/colored-completions.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1400 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/auto-completion/combine-multiple-completers.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1425 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/auto-completion/fuzzy-custom-completer.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1194 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/auto-completion/fuzzy-word-completer.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1212 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/auto-completion/multi-column-autocompletion-with-meta.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1093 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/auto-completion/multi-column-autocompletion.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      469 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/auto-completion/nested-autocompletion.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2650 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/auto-completion/slow-completions.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1453 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/auto-suggestion.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1096 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/autocorrection.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2339 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/bottom-toolbar.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      568 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/clock-input.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1858 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/colored-prompt.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      215 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/confirmation-prompt.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1840 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/custom-key-binding.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      734 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/custom-lexer.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2178 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/custom-vi-operator-and-text-object.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2046 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.8/examples/prompts/fancy-zsh-prompt.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1320 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/finalterm-shell-integration.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      275 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/get-input-vi-mode.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      338 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/get-input-with-default.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      203 2020-09-14 20:06:46.000000 prompt_toolkit-3.0.8/examples/prompts/get-input.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1007 2020-05-07 15:14:27.000000 prompt_toolkit-3.0.8/examples/prompts/get-multiline-input.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      770 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/get-password-with-toggle-display-shortcut.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      175 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/get-password.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.848594 prompt_toolkit-3.0.8/examples/prompts/history/
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      729 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/history/persistent-history.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1373 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/history/slow-history.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      407 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/html-input.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      753 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/input-validation.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2497 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/examples/prompts/inputhook.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      380 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/mouse-support.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      290 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/multiline-prompt.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      197 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/no-wrapping.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      404 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/operate-and-get-next.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      922 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/patch-stdout.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      388 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/examples/prompts/placeholder-text.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     3158 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/regular-language.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1524 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/rprompt.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2018 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/swap-light-and-dark-colors.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1033 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/switch-between-vi-emacs.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      610 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/system-clipboard-integration.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      747 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/system-prompt.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      273 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/terminal-title.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1217 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/prompts/up-arrow-partial-string-matching.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.848594 prompt_toolkit-3.0.8/examples/ssh/
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     3240 2020-07-01 16:08:21.000000 prompt_toolkit-3.0.8/examples/ssh/asyncssh-server.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.856594 prompt_toolkit-3.0.8/examples/telnet/
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2521 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/telnet/chat-app.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      741 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/telnet/dialog.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      980 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/telnet/hello-world.py
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1148 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/telnet/toolbar.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.860594 prompt_toolkit-3.0.8/examples/tutorial/
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)       85 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/examples/tutorial/README.md
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     3600 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/examples/tutorial/sqlite-cli.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      128 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/mypy.ini
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.880594 prompt_toolkit-3.0.8/prompt_toolkit/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      926 2020-10-12 14:55:20.000000 prompt_toolkit-3.0.8/prompt_toolkit/__init__.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.892594 prompt_toolkit-3.0.8/prompt_toolkit/application/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      553 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.8/prompt_toolkit/application/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    46086 2020-10-12 13:59:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/application/application.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5208 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/application/current.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1358 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/application/dummy.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3706 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/application/run_in_terminal.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5922 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/auto_suggest.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    70340 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/buffer.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3768 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/cache.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.896594 prompt_toolkit-3.0.8/prompt_toolkit/clipboard/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      403 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/clipboard/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2492 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/clipboard/base.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1077 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/clipboard/in_memory.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1151 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/clipboard/pyperclip.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.900594 prompt_toolkit-3.0.8/prompt_toolkit/completion/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      810 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/completion/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    11514 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/completion/base.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3838 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/completion/filesystem.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6954 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/completion/fuzzy_completer.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3894 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/completion/nested.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3036 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.8/prompt_toolkit/completion/word_completer.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.904594 prompt_toolkit-3.0.8/prompt_toolkit/contrib/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/prompt_toolkit/contrib/__init__.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.904594 prompt_toolkit-3.0.8/prompt_toolkit/contrib/completers/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       67 2020-07-01 16:08:21.000000 prompt_toolkit-3.0.8/prompt_toolkit/contrib/completers/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2021 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/contrib/completers/system.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.908594 prompt_toolkit-3.0.8/prompt_toolkit/contrib/regular_languages/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3243 2020-07-01 16:08:21.000000 prompt_toolkit-3.0.8/prompt_toolkit/contrib/regular_languages/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    21889 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/contrib/regular_languages/compiler.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3245 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/contrib/regular_languages/completion.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3398 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/contrib/regular_languages/lexer.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7827 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/contrib/regular_languages/regex_parser.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2048 2020-07-01 16:08:21.000000 prompt_toolkit-3.0.8/prompt_toolkit/contrib/regular_languages/validation.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.912594 prompt_toolkit-3.0.8/prompt_toolkit/contrib/ssh/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      144 2020-07-01 16:08:21.000000 prompt_toolkit-3.0.8/prompt_toolkit/contrib/ssh/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5096 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.8/prompt_toolkit/contrib/ssh/server.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.916594 prompt_toolkit-3.0.8/prompt_toolkit/contrib/telnet/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       68 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/contrib/telnet/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      130 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/contrib/telnet/log.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5561 2020-07-01 16:08:21.000000 prompt_toolkit-3.0.8/prompt_toolkit/contrib/telnet/protocol.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10487 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.8/prompt_toolkit/contrib/telnet/server.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      187 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/data_structures.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    40664 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.8/prompt_toolkit/document.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      322 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/enums.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.924594 prompt_toolkit-3.0.8/prompt_toolkit/eventloop/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      636 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/eventloop/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4126 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/eventloop/async_context_manager.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1711 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/eventloop/async_generator.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1117 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/eventloop/dummy_contextvars.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5517 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/eventloop/inputhook.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3251 2020-03-06 06:18:12.000000 prompt_toolkit-3.0.8/prompt_toolkit/eventloop/utils.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2011 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/eventloop/win32.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.928594 prompt_toolkit-3.0.8/prompt_toolkit/filters/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1028 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/filters/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9814 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/filters/app.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5737 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/filters/base.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1830 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/filters/cli.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      848 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/filters/utils.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.928594 prompt_toolkit-3.0.8/prompt_toolkit/formatted_text/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1378 2020-10-12 13:56:12.000000 prompt_toolkit-3.0.8/prompt_toolkit/formatted_text/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8095 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/formatted_text/ansi.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4960 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.8/prompt_toolkit/formatted_text/base.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4328 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/formatted_text/html.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      759 2020-10-12 13:56:12.000000 prompt_toolkit-3.0.8/prompt_toolkit/formatted_text/pygments.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2750 2020-10-12 13:56:12.000000 prompt_toolkit-3.0.8/prompt_toolkit/formatted_text/utils.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7131 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/history.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.944594 prompt_toolkit-3.0.8/prompt_toolkit/input/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      209 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/input/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    13116 2020-09-30 08:18:46.000000 prompt_toolkit-3.0.8/prompt_toolkit/input/ansi_escape_sequences.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3386 2020-09-16 15:06:28.000000 prompt_toolkit-3.0.8/prompt_toolkit/input/base.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1540 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/input/defaults.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1831 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/input/posix_pipe.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3937 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.8/prompt_toolkit/input/posix_utils.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2538 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/input/typeahead.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10109 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.8/prompt_toolkit/input/vt100.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8402 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/input/vt100_parser.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    22325 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.8/prompt_toolkit/input/win32.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4078 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/input/win32_pipe.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.948594 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      411 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/__init__.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.964594 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1808 2020-10-05 00:39:31.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/auto_suggest.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7191 2020-09-29 07:33:53.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/basic.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6876 2020-10-05 00:39:31.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/completion.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      750 2020-10-05 00:39:31.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/cpr.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    19593 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/emacs.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      471 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/focus.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4967 2020-10-05 00:39:31.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/mouse.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    18381 2020-07-01 16:08:21.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/named_commands.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1319 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/open_in_editor.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2355 2020-10-05 00:39:31.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/page_navigation.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5576 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/scroll.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2595 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/search.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    75531 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/vi.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1938 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/defaults.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    32798 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/digraphs.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      895 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/emacs_state.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    19399 2020-10-05 00:39:31.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/key_bindings.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    17655 2020-10-05 00:39:31.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/key_processor.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3364 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/key_binding/vi_state.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4885 2020-03-06 06:42:35.000000 prompt_toolkit-3.0.8/prompt_toolkit/keys.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.976594 prompt_toolkit-3.0.8/prompt_toolkit/layout/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3500 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.8/prompt_toolkit/layout/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    97597 2020-10-06 16:47:07.000000 prompt_toolkit-3.0.8/prompt_toolkit/layout/containers.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    35376 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/layout/controls.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6948 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.8/prompt_toolkit/layout/dimension.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1010 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/layout/dummy.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    14111 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.8/prompt_toolkit/layout/layout.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10382 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/layout/margins.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    25397 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.8/prompt_toolkit/layout/menus.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1046 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/layout/mouse_handlers.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    34176 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/layout/processors.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9754 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/layout/screen.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2262 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/layout/utils.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.980594 prompt_toolkit-3.0.8/prompt_toolkit/lexers/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      372 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/lexers/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2328 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/lexers/base.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    11958 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/lexers/pygments.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      116 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/log.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1339 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/mouse_events.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.984594 prompt_toolkit-3.0.8/prompt_toolkit/output/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      244 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/output/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7650 2020-10-05 00:39:31.000000 prompt_toolkit-3.0.8/prompt_toolkit/output/base.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1387 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/output/color_depth.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1816 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/output/conemu.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2477 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/output/defaults.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    22962 2020-09-23 19:10:55.000000 prompt_toolkit-3.0.8/prompt_toolkit/output/vt100.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    21973 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/output/win32.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3168 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/output/windows10.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5155 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/patch_stdout.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.8/prompt_toolkit/py.typed
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    28027 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/renderer.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7012 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/search.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1289 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/selection.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.984594 prompt_toolkit-3.0.8/prompt_toolkit/shortcuts/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      913 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.8/prompt_toolkit/shortcuts/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8826 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.8/prompt_toolkit/shortcuts/dialogs.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.988594 prompt_toolkit-3.0.8/prompt_toolkit/shortcuts/progress_bar/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      504 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.8/prompt_toolkit/shortcuts/progress_bar/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    14243 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/shortcuts/progress_bar/base.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    11782 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/shortcuts/progress_bar/formatters.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    58386 2020-10-12 13:59:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/shortcuts/prompt.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5752 2020-07-01 16:08:21.000000 prompt_toolkit-3.0.8/prompt_toolkit/shortcuts/utils.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.992594 prompt_toolkit-3.0.8/prompt_toolkit/styles/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1603 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/styles/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5062 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/styles/base.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8412 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/styles/defaults.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4355 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/styles/named_colors.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1955 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/styles/pygments.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    13026 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/styles/style.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12449 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/styles/style_transformation.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       85 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/token.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8180 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/prompt_toolkit/utils.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5840 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/validation.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.996594 prompt_toolkit-3.0.8/prompt_toolkit/widgets/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1181 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/widgets/__init__.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    29413 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.8/prompt_toolkit/widgets/base.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3370 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/widgets/dialogs.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12769 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/widgets/menus.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12238 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/widgets/toolbars.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4138 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/prompt_toolkit/win32_types.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:13.884594 prompt_toolkit-3.0.8/prompt_toolkit.egg-info/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8164 2020-10-12 14:58:13.000000 prompt_toolkit-3.0.8/prompt_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12667 2020-10-12 14:58:13.000000 prompt_toolkit-3.0.8/prompt_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        1 2020-10-12 14:58:13.000000 prompt_toolkit-3.0.8/prompt_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        8 2020-10-12 14:58:13.000000 prompt_toolkit-3.0.8/prompt_toolkit.egg-info/requires.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       15 2020-10-12 14:58:13.000000 prompt_toolkit-3.0.8/prompt_toolkit.egg-info/top_level.txt
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      296 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/pyproject.toml
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      358 2020-10-12 14:58:14.004594 prompt_toolkit-3.0.8/setup.cfg
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2194 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/setup.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:14.000594 prompt_toolkit-3.0.8/tests/
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      665 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/tests/test_async_generator.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2623 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/tests/test_buffer.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    28084 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/tests/test_cli.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    14392 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.8/tests/test_completion.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1626 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/tests/test_document.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1248 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/tests/test_filter.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5524 2020-10-12 13:56:12.000000 prompt_toolkit-3.0.8/tests/test_formatted_text.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4032 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/tests/test_inputstream.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5878 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/tests/test_key_binding.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1500 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/tests/test_layout.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2492 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/tests/test_print_formatted_text.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3124 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/tests/test_regular_languages.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1702 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/tests/test_shortcuts.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6451 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.8/tests/test_style.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1485 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/tests/test_style_transformation.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1588 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/tests/test_utils.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      657 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/tests/test_vt100_output.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2045 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.8/tests/test_yank_nth_arg.py
-drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2020-10-12 14:58:14.000594 prompt_toolkit-3.0.8/tools/
--rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      642 2020-09-14 23:38:45.000000 prompt_toolkit-3.0.8/tools/debug_vt100_input.py
--rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      352 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.8/tox.ini
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.669957 prompt_toolkit-3.0.9/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       13 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/.codecov.yml
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      423 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/.gitignore
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      773 2020-09-23 19:10:55.000000 prompt_toolkit-3.0.9/.travis.yml
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      148 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/AUTHORS.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    66498 2021-01-05 09:04:09.000000 prompt_toolkit-3.0.9/CHANGELOG
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1493 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/LICENSE
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      133 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/MANIFEST.in
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8164 2021-01-05 09:05:13.669957 prompt_toolkit-3.0.9/PKG-INFO
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4453 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/PROJECTS.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6034 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.9/README.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      997 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/appveyor.yml
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.277967 prompt_toolkit-3.0.9/docs/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6794 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/Makefile
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8581 2021-01-05 09:04:34.000000 prompt_toolkit-3.0.9/docs/conf.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.333966 prompt_toolkit-3.0.9/docs/images/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    72983 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/auto-suggestion.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    77372 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/bottom-toolbar.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    94994 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/colored-prompt.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    95099 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/colorful-completions.png
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.349965 prompt_toolkit-3.0.9/docs/images/dialogs/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   134890 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/dialogs/button.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   135405 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/dialogs/confirm.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   140141 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/dialogs/inputbox.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   139732 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/dialogs/messagebox.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   144850 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/dialogs/styled.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   105790 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/hello-world-prompt.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    92781 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/html-completion.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   116804 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/html-input.png
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)    56254 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/logo_400px.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    85296 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/multiline-input.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    81683 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/number-validator.png
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.357965 prompt_toolkit-3.0.9/docs/images/progress-bars/
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     5411 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/progress-bars/apt-get.png
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     8575 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/progress-bars/colored-title-and-label.png
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     8191 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/progress-bars/custom-key-bindings.png
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)    13218 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/progress-bars/simple-progress-bar.png
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     9723 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/progress-bars/two-tasks.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   133464 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/ptpython-2.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   103337 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/ptpython-history-help.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    60225 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/ptpython-menu.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    28700 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/ptpython.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   205809 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/pymux.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   150054 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/pyvim.png
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.373965 prompt_toolkit-3.0.9/docs/images/repl/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   125880 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/repl/sqlite-1.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   171192 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/repl/sqlite-2.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   126517 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/repl/sqlite-3.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   190998 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/repl/sqlite-4.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   182631 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/repl/sqlite-5.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)   200352 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/repl/sqlite-6.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    79787 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/images/rprompt.png
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2712 2021-01-05 08:58:30.000000 prompt_toolkit-3.0.9/docs/index.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6699 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/make.bat
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.385964 prompt_toolkit-3.0.9/docs/pages/
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.401964 prompt_toolkit-3.0.9/docs/pages/advanced_topics/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5484 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/pages/advanced_topics/architecture.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      794 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/docs/pages/advanced_topics/asyncio.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5714 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/pages/advanced_topics/filters.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      255 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.9/docs/pages/advanced_topics/index.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1455 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.9/docs/pages/advanced_topics/input_hooks.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12642 2021-01-05 08:58:30.000000 prompt_toolkit-3.0.9/docs/pages/advanced_topics/key_bindings.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3712 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/pages/advanced_topics/rendering_flow.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7337 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/pages/advanced_topics/rendering_pipeline.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10560 2021-01-05 08:58:30.000000 prompt_toolkit-3.0.9/docs/pages/advanced_topics/styling.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    32545 2020-09-14 23:38:45.000000 prompt_toolkit-3.0.9/docs/pages/asking_for_input.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9356 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.9/docs/pages/dialogs.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    18442 2021-01-05 08:58:30.000000 prompt_toolkit-3.0.9/docs/pages/full_screen_apps.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      588 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/pages/gallery.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2833 2021-01-05 08:58:30.000000 prompt_toolkit-3.0.9/docs/pages/getting_started.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9210 2020-10-12 13:56:12.000000 prompt_toolkit-3.0.9/docs/pages/printing_text.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7426 2021-01-05 08:58:30.000000 prompt_toolkit-3.0.9/docs/pages/progress_bars.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5793 2020-07-30 11:15:49.000000 prompt_toolkit-3.0.9/docs/pages/reference.rst
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.405964 prompt_toolkit-3.0.9/docs/pages/tutorials/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      101 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/docs/pages/tutorials/index.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12327 2021-01-05 08:58:30.000000 prompt_toolkit-3.0.9/docs/pages/tutorials/repl.rst
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.409964 prompt_toolkit-3.0.9/docs/pages/upgrading/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9591 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/docs/pages/upgrading/2.0.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3577 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/docs/pages/upgrading/3.0.rst
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      108 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/docs/pages/upgrading/index.rst
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.413964 prompt_toolkit-3.0.9/examples/
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.429963 prompt_toolkit-3.0.9/examples/dialogs/
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      386 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/examples/dialogs/button_dialog.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1055 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/dialogs/checkbox_dialog.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      314 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/dialogs/input_dialog.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      303 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/dialogs/messagebox.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      358 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/dialogs/password_dialog.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1158 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/dialogs/progress_dialog.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1080 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/dialogs/radio_dialog.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      931 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/dialogs/styled_messagebox.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      334 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/dialogs/yes_no_dialog.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.445963 prompt_toolkit-3.0.9/examples/full-screen/
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2389 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/full-screen/buttons.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2819 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/full-screen/calculator.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      159 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/examples/full-screen/dummy-app.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     5605 2020-09-14 23:38:45.000000 prompt_toolkit-3.0.9/examples/full-screen/full-screen-demo.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      938 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/examples/full-screen/hello-world.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      155 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/examples/full-screen/no-layout.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2500 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/examples/full-screen/pager.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.465963 prompt_toolkit-3.0.9/examples/full-screen/simple-demos/
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1959 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/full-screen/simple-demos/alignment.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2139 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/full-screen/simple-demos/autocompletion.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1869 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/full-screen/simple-demos/colorcolumn.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1870 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/full-screen/simple-demos/cursorcolumn-cursorline.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2743 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/full-screen/simple-demos/float-transparency.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     3429 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/full-screen/simple-demos/floats.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2775 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/full-screen/simple-demos/focus.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     7320 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/full-screen/simple-demos/horizontal-align.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      949 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/full-screen/simple-demos/horizontal-split.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     3146 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/full-screen/simple-demos/line-prefixes.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2184 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/full-screen/simple-demos/margins.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     5530 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/full-screen/simple-demos/vertical-align.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      944 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/full-screen/simple-demos/vertical-split.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     5144 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/full-screen/split-screen.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     9221 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/examples/full-screen/text-editor.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      686 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/examples/gevent-get-input.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.481962 prompt_toolkit-3.0.9/examples/print-text/
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     3083 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/print-text/ansi-colors.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1187 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/print-text/ansi.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1330 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/print-text/html.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      883 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/print-text/named-colors.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1097 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/examples/print-text/print-formatted-text.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      331 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/examples/print-text/print-frame.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1230 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/print-text/pygments-tokens.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1024 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/print-text/true-color-demo.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.509961 prompt_toolkit-3.0.9/examples/progress-bar/
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1903 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/progress-bar/a-lot-of-parallel-tasks.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      537 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/progress-bar/colored-title-and-label.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1211 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/progress-bar/custom-key-bindings.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1591 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/progress-bar/many-parallel-tasks.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      601 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/progress-bar/nested-progress-bars.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      532 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/progress-bar/scrolling-task-name.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      325 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/progress-bar/simple-progress-bar.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      862 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/progress-bar/styled-1.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1347 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/progress-bar/styled-2.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      941 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/progress-bar/styled-apt-get-install.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      932 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/progress-bar/styled-rainbow.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1108 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/examples/progress-bar/styled-tqdm-1.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1034 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/examples/progress-bar/styled-tqdm-2.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      929 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/progress-bar/two-tasks.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      516 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/progress-bar/unknown-length.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.573960 prompt_toolkit-3.0.9/examples/prompts/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      467 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/accept-default.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1957 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/asyncio-prompt.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.593959 prompt_toolkit-3.0.9/examples/prompts/auto-completion/
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1410 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/auto-completion/autocomplete-with-control-space.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1122 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/auto-completion/autocompletion-like-readline.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1198 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/auto-completion/autocompletion.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     3758 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/auto-completion/colored-completions-with-formatted-text.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1937 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/auto-completion/colored-completions.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1400 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/auto-completion/combine-multiple-completers.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1425 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/auto-completion/fuzzy-custom-completer.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1194 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/auto-completion/fuzzy-word-completer.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1212 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/auto-completion/multi-column-autocompletion-with-meta.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1093 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/auto-completion/multi-column-autocompletion.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      469 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/auto-completion/nested-autocompletion.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2650 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/auto-completion/slow-completions.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1453 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/auto-suggestion.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1096 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/autocorrection.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2339 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/bottom-toolbar.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      568 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/clock-input.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1858 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/colored-prompt.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      215 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/confirmation-prompt.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1840 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/custom-key-binding.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      734 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/custom-lexer.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2178 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/custom-vi-operator-and-text-object.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2046 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.9/examples/prompts/fancy-zsh-prompt.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1320 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/finalterm-shell-integration.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      275 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/get-input-vi-mode.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      338 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/get-input-with-default.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      203 2020-09-14 20:06:46.000000 prompt_toolkit-3.0.9/examples/prompts/get-input.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1007 2020-05-07 15:14:27.000000 prompt_toolkit-3.0.9/examples/prompts/get-multiline-input.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      770 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/get-password-with-toggle-display-shortcut.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      175 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/get-password.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.593959 prompt_toolkit-3.0.9/examples/prompts/history/
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      729 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/history/persistent-history.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1373 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/history/slow-history.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      407 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/html-input.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      753 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/input-validation.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2497 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/examples/prompts/inputhook.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      380 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/mouse-support.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      290 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/multiline-prompt.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      197 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/no-wrapping.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      404 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/operate-and-get-next.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      922 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/patch-stdout.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      388 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/examples/prompts/placeholder-text.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     3158 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/regular-language.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1524 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/rprompt.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2018 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/swap-light-and-dark-colors.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1033 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/switch-between-vi-emacs.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      610 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/system-clipboard-integration.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      747 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/system-prompt.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      273 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/terminal-title.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1217 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/prompts/up-arrow-partial-string-matching.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.597959 prompt_toolkit-3.0.9/examples/ssh/
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     3240 2020-07-01 16:08:21.000000 prompt_toolkit-3.0.9/examples/ssh/asyncssh-server.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.601959 prompt_toolkit-3.0.9/examples/telnet/
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2521 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/telnet/chat-app.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      741 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/telnet/dialog.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      980 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/telnet/hello-world.py
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     1148 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/telnet/toolbar.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.605959 prompt_toolkit-3.0.9/examples/tutorial/
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)       85 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/examples/tutorial/README.md
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     3600 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/examples/tutorial/sqlite-cli.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      128 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/mypy.ini
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.621959 prompt_toolkit-3.0.9/prompt_toolkit/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      926 2021-01-05 09:04:20.000000 prompt_toolkit-3.0.9/prompt_toolkit/__init__.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.629958 prompt_toolkit-3.0.9/prompt_toolkit/application/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      553 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.9/prompt_toolkit/application/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    46086 2021-01-05 09:00:33.000000 prompt_toolkit-3.0.9/prompt_toolkit/application/application.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5208 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/application/current.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1358 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/application/dummy.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3706 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/application/run_in_terminal.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5922 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/auto_suggest.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    70340 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/buffer.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3768 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/cache.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.629958 prompt_toolkit-3.0.9/prompt_toolkit/clipboard/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      403 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/clipboard/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2492 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/clipboard/base.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1077 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/clipboard/in_memory.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1151 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/clipboard/pyperclip.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.629958 prompt_toolkit-3.0.9/prompt_toolkit/completion/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      810 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/completion/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    11514 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/completion/base.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3838 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/completion/filesystem.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6954 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/completion/fuzzy_completer.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3894 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/completion/nested.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3036 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.9/prompt_toolkit/completion/word_completer.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.629958 prompt_toolkit-3.0.9/prompt_toolkit/contrib/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/prompt_toolkit/contrib/__init__.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.629958 prompt_toolkit-3.0.9/prompt_toolkit/contrib/completers/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       67 2020-07-01 16:08:21.000000 prompt_toolkit-3.0.9/prompt_toolkit/contrib/completers/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2021 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/contrib/completers/system.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.633958 prompt_toolkit-3.0.9/prompt_toolkit/contrib/regular_languages/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3243 2020-07-01 16:08:21.000000 prompt_toolkit-3.0.9/prompt_toolkit/contrib/regular_languages/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    21889 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/contrib/regular_languages/compiler.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3245 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/contrib/regular_languages/completion.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3398 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/contrib/regular_languages/lexer.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7827 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/contrib/regular_languages/regex_parser.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2048 2020-07-01 16:08:21.000000 prompt_toolkit-3.0.9/prompt_toolkit/contrib/regular_languages/validation.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.633958 prompt_toolkit-3.0.9/prompt_toolkit/contrib/ssh/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      144 2020-07-01 16:08:21.000000 prompt_toolkit-3.0.9/prompt_toolkit/contrib/ssh/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5096 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.9/prompt_toolkit/contrib/ssh/server.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.633958 prompt_toolkit-3.0.9/prompt_toolkit/contrib/telnet/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       68 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/contrib/telnet/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      130 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/contrib/telnet/log.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5561 2020-07-01 16:08:21.000000 prompt_toolkit-3.0.9/prompt_toolkit/contrib/telnet/protocol.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10487 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.9/prompt_toolkit/contrib/telnet/server.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      187 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/data_structures.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    40664 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.9/prompt_toolkit/document.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      322 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/enums.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.633958 prompt_toolkit-3.0.9/prompt_toolkit/eventloop/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      636 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/eventloop/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4126 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/eventloop/async_context_manager.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1711 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/eventloop/async_generator.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1117 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/eventloop/dummy_contextvars.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5517 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/eventloop/inputhook.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3251 2020-03-06 06:18:12.000000 prompt_toolkit-3.0.9/prompt_toolkit/eventloop/utils.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2011 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/eventloop/win32.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.633958 prompt_toolkit-3.0.9/prompt_toolkit/filters/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1028 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/filters/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9814 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/filters/app.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5737 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/filters/base.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1830 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/filters/cli.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      848 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/filters/utils.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.637958 prompt_toolkit-3.0.9/prompt_toolkit/formatted_text/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1378 2020-10-12 13:56:12.000000 prompt_toolkit-3.0.9/prompt_toolkit/formatted_text/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8095 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/formatted_text/ansi.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4960 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.9/prompt_toolkit/formatted_text/base.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4328 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/formatted_text/html.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      759 2020-10-12 13:56:12.000000 prompt_toolkit-3.0.9/prompt_toolkit/formatted_text/pygments.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2750 2020-10-12 13:56:12.000000 prompt_toolkit-3.0.9/prompt_toolkit/formatted_text/utils.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7143 2021-01-05 08:58:30.000000 prompt_toolkit-3.0.9/prompt_toolkit/history.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.637958 prompt_toolkit-3.0.9/prompt_toolkit/input/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      209 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/input/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    13163 2021-01-05 08:58:30.000000 prompt_toolkit-3.0.9/prompt_toolkit/input/ansi_escape_sequences.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3386 2020-09-16 15:06:28.000000 prompt_toolkit-3.0.9/prompt_toolkit/input/base.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1540 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/input/defaults.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1831 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/input/posix_pipe.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3937 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.9/prompt_toolkit/input/posix_utils.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2538 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/input/typeahead.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10109 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.9/prompt_toolkit/input/vt100.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8402 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/input/vt100_parser.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    22325 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.9/prompt_toolkit/input/win32.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4078 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/input/win32_pipe.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.637958 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      411 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/__init__.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.641958 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1808 2020-10-05 00:39:31.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/auto_suggest.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7191 2020-09-29 07:33:53.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/basic.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6876 2020-10-05 00:39:31.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/completion.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      750 2020-10-05 00:39:31.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/cpr.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    19593 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/emacs.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      471 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/focus.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4967 2020-10-05 00:39:31.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/mouse.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    18381 2020-07-01 16:08:21.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/named_commands.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1319 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/open_in_editor.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2355 2020-10-05 00:39:31.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/page_navigation.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5576 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/scroll.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2595 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/search.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    75531 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/vi.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1938 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/defaults.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    32798 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/digraphs.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      895 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/emacs_state.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    19399 2020-10-05 00:39:31.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/key_bindings.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    17655 2020-10-05 00:39:31.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/key_processor.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3364 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/key_binding/vi_state.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4885 2020-03-06 06:42:35.000000 prompt_toolkit-3.0.9/prompt_toolkit/keys.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.641958 prompt_toolkit-3.0.9/prompt_toolkit/layout/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3500 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.9/prompt_toolkit/layout/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    97597 2020-10-06 16:47:07.000000 prompt_toolkit-3.0.9/prompt_toolkit/layout/containers.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    35376 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/layout/controls.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6948 2020-11-25 09:51:25.000000 prompt_toolkit-3.0.9/prompt_toolkit/layout/dimension.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1010 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/layout/dummy.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    14111 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.9/prompt_toolkit/layout/layout.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    10382 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/layout/margins.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    25397 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.9/prompt_toolkit/layout/menus.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1046 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/layout/mouse_handlers.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    34183 2021-01-05 08:58:30.000000 prompt_toolkit-3.0.9/prompt_toolkit/layout/processors.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     9754 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/layout/screen.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2262 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/layout/utils.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.641958 prompt_toolkit-3.0.9/prompt_toolkit/lexers/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      372 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/lexers/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2328 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/lexers/base.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    11958 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/lexers/pygments.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      116 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/log.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1339 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/mouse_events.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.645958 prompt_toolkit-3.0.9/prompt_toolkit/output/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      244 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/output/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7650 2020-10-05 00:39:31.000000 prompt_toolkit-3.0.9/prompt_toolkit/output/base.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1387 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/output/color_depth.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1816 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/output/conemu.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2477 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/output/defaults.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    22962 2020-10-13 12:56:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/output/vt100.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    21973 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/output/win32.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3168 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/output/windows10.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5155 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/patch_stdout.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        0 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.9/prompt_toolkit/py.typed
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    28230 2021-01-05 08:58:30.000000 prompt_toolkit-3.0.9/prompt_toolkit/renderer.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     7012 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/search.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1289 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/selection.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.645958 prompt_toolkit-3.0.9/prompt_toolkit/shortcuts/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      913 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.9/prompt_toolkit/shortcuts/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8826 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.9/prompt_toolkit/shortcuts/dialogs.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.645958 prompt_toolkit-3.0.9/prompt_toolkit/shortcuts/progress_bar/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      504 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.9/prompt_toolkit/shortcuts/progress_bar/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    14243 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/shortcuts/progress_bar/base.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    11782 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/shortcuts/progress_bar/formatters.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    58386 2021-01-05 09:00:33.000000 prompt_toolkit-3.0.9/prompt_toolkit/shortcuts/prompt.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5752 2020-07-01 16:08:21.000000 prompt_toolkit-3.0.9/prompt_toolkit/shortcuts/utils.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.645958 prompt_toolkit-3.0.9/prompt_toolkit/styles/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1603 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/styles/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5062 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/styles/base.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8412 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/styles/defaults.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4355 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/styles/named_colors.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1955 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/styles/pygments.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    13026 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/styles/style.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12449 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/styles/style_transformation.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       85 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/token.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8180 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/prompt_toolkit/utils.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5840 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/validation.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.645958 prompt_toolkit-3.0.9/prompt_toolkit/widgets/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1181 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/widgets/__init__.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    29413 2020-10-12 13:56:14.000000 prompt_toolkit-3.0.9/prompt_toolkit/widgets/base.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3370 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/widgets/dialogs.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12769 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/widgets/menus.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12238 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/widgets/toolbars.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4138 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/prompt_toolkit/win32_types.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.625959 prompt_toolkit-3.0.9/prompt_toolkit.egg-info/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     8164 2021-01-05 09:05:13.000000 prompt_toolkit-3.0.9/prompt_toolkit.egg-info/PKG-INFO
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    12667 2021-01-05 09:05:13.000000 prompt_toolkit-3.0.9/prompt_toolkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        1 2021-01-05 09:05:13.000000 prompt_toolkit-3.0.9/prompt_toolkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)        8 2021-01-05 09:05:13.000000 prompt_toolkit-3.0.9/prompt_toolkit.egg-info/requires.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)       15 2021-01-05 09:05:13.000000 prompt_toolkit-3.0.9/prompt_toolkit.egg-info/top_level.txt
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      296 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/pyproject.toml
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      358 2021-01-05 09:05:13.669957 prompt_toolkit-3.0.9/setup.cfg
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)     2194 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/setup.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.669957 prompt_toolkit-3.0.9/tests/
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      665 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/tests/test_async_generator.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2623 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/tests/test_buffer.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    28084 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/tests/test_cli.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)    14392 2020-05-07 15:14:31.000000 prompt_toolkit-3.0.9/tests/test_completion.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1626 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/tests/test_document.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1248 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/tests/test_filter.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5524 2020-10-12 13:56:12.000000 prompt_toolkit-3.0.9/tests/test_formatted_text.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     4032 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/tests/test_inputstream.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     5878 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/tests/test_key_binding.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1500 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/tests/test_layout.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2492 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/tests/test_print_formatted_text.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     3124 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/tests/test_regular_languages.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1702 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/tests/test_shortcuts.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     6451 2020-09-09 15:49:45.000000 prompt_toolkit-3.0.9/tests/test_style.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1485 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/tests/test_style_transformation.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     1588 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/tests/test_utils.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      657 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/tests/test_vt100_output.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)     2045 2020-03-06 06:18:08.000000 prompt_toolkit-3.0.9/tests/test_yank_nth_arg.py
+drwxrwxr-x   0 jonathan  (1000) jonathan  (1000)        0 2021-01-05 09:05:13.669957 prompt_toolkit-3.0.9/tools/
+-rwxrwxr-x   0 jonathan  (1000) jonathan  (1000)      642 2020-09-14 23:38:45.000000 prompt_toolkit-3.0.9/tools/debug_vt100_input.py
+-rw-rw-r--   0 jonathan  (1000) jonathan  (1000)      352 2020-01-12 17:01:43.000000 prompt_toolkit-3.0.9/tox.ini
```

### Comparing `prompt_toolkit-3.0.8/.travis.yml` & `prompt_toolkit-3.0.9/.travis.yml`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/CHANGELOG` & `prompt_toolkit-3.0.9/CHANGELOG`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 CHANGELOG
 =========
 
+3.0.9: 2021-01-05
+-----------------
+
+New features:
+- Handle c-tab for TERM=linux.
+
+Fixes:
+- Improve rendering speed of `print_formatted_text`. (Don't render styling
+  attributes to output between fragments that have identical styling.)
+- Gracefully handle `FileHistory` decoding errors.
+- Prevent asyncio deprecation warnings.
+
+
 3.0.8: 2020-10-12
 -----------------
 
 New features:
 - Added `validator` parameter to `input_dialog`.
 
 Fixes:
```

### Comparing `prompt_toolkit-3.0.8/LICENSE` & `prompt_toolkit-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/PKG-INFO` & `prompt_toolkit-3.0.9/prompt_toolkit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: prompt_toolkit
-Version: 3.0.8
+Name: prompt-toolkit
+Version: 3.0.9
 Summary: Library for building powerful interactive command lines in Python
 Home-page: https://github.com/prompt-toolkit/python-prompt-toolkit
 Author: Jonathan Slenders
 License: UNKNOWN
 Description: Python Prompt Toolkit
         =====================
```

### Comparing `prompt_toolkit-3.0.8/PROJECTS.rst` & `prompt_toolkit-3.0.9/PROJECTS.rst`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/README.rst` & `prompt_toolkit-3.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/appveyor.yml` & `prompt_toolkit-3.0.9/appveyor.yml`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/Makefile` & `prompt_toolkit-3.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/conf.py` & `prompt_toolkit-3.0.9/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,17 +47,17 @@
 copyright = u'2014-2020, Jonathan Slenders'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
-version = '3.0.8'
+version = '3.0.9'
 # The full version, including alpha/beta/rc tags.
-release = '3.0.8'
+release = '3.0.9'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #language = None
 
 # There are two options for replacing |today|: either, you set today to some
 # non-false value, then it is used:
```

### Comparing `prompt_toolkit-3.0.8/docs/images/auto-suggestion.png` & `prompt_toolkit-3.0.9/docs/images/auto-suggestion.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/bottom-toolbar.png` & `prompt_toolkit-3.0.9/docs/images/bottom-toolbar.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/colored-prompt.png` & `prompt_toolkit-3.0.9/docs/images/colored-prompt.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/colorful-completions.png` & `prompt_toolkit-3.0.9/docs/images/colorful-completions.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/dialogs/button.png` & `prompt_toolkit-3.0.9/docs/images/dialogs/button.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/dialogs/confirm.png` & `prompt_toolkit-3.0.9/docs/images/dialogs/confirm.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/dialogs/inputbox.png` & `prompt_toolkit-3.0.9/docs/images/dialogs/inputbox.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/dialogs/messagebox.png` & `prompt_toolkit-3.0.9/docs/images/dialogs/messagebox.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/dialogs/styled.png` & `prompt_toolkit-3.0.9/docs/images/dialogs/styled.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/hello-world-prompt.png` & `prompt_toolkit-3.0.9/docs/images/hello-world-prompt.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/html-completion.png` & `prompt_toolkit-3.0.9/docs/images/html-completion.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/html-input.png` & `prompt_toolkit-3.0.9/docs/images/html-input.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/logo_400px.png` & `prompt_toolkit-3.0.9/docs/images/logo_400px.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/multiline-input.png` & `prompt_toolkit-3.0.9/docs/images/multiline-input.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/number-validator.png` & `prompt_toolkit-3.0.9/docs/images/number-validator.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/progress-bars/apt-get.png` & `prompt_toolkit-3.0.9/docs/images/progress-bars/apt-get.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/progress-bars/colored-title-and-label.png` & `prompt_toolkit-3.0.9/docs/images/progress-bars/colored-title-and-label.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/progress-bars/custom-key-bindings.png` & `prompt_toolkit-3.0.9/docs/images/progress-bars/custom-key-bindings.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/progress-bars/simple-progress-bar.png` & `prompt_toolkit-3.0.9/docs/images/progress-bars/simple-progress-bar.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/progress-bars/two-tasks.png` & `prompt_toolkit-3.0.9/docs/images/progress-bars/two-tasks.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/ptpython-2.png` & `prompt_toolkit-3.0.9/docs/images/ptpython-2.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/ptpython-history-help.png` & `prompt_toolkit-3.0.9/docs/images/ptpython-history-help.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/ptpython-menu.png` & `prompt_toolkit-3.0.9/docs/images/ptpython-menu.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/ptpython.png` & `prompt_toolkit-3.0.9/docs/images/ptpython.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/pymux.png` & `prompt_toolkit-3.0.9/docs/images/pymux.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/pyvim.png` & `prompt_toolkit-3.0.9/docs/images/pyvim.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/repl/sqlite-1.png` & `prompt_toolkit-3.0.9/docs/images/repl/sqlite-1.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/repl/sqlite-2.png` & `prompt_toolkit-3.0.9/docs/images/repl/sqlite-2.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/repl/sqlite-3.png` & `prompt_toolkit-3.0.9/docs/images/repl/sqlite-3.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/repl/sqlite-4.png` & `prompt_toolkit-3.0.9/docs/images/repl/sqlite-4.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/repl/sqlite-5.png` & `prompt_toolkit-3.0.9/docs/images/repl/sqlite-5.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/repl/sqlite-6.png` & `prompt_toolkit-3.0.9/docs/images/repl/sqlite-6.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/images/rprompt.png` & `prompt_toolkit-3.0.9/docs/images/rprompt.png`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/index.rst` & `prompt_toolkit-3.0.9/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 Go to :ref:`getting started <getting_started>` and build your first prompt.
 
 
 Thanks to:
 ----------
 
 A special thanks to `all the contributors
-<https://github.com/jonathanslenders/python-prompt-toolkit/graphs/contributors>`_
+<https://github.com/prompt_toolkit/python-prompt-toolkit/graphs/contributors>`_
 for making prompt_toolkit possible.
 
 Also, a special thanks to the `Pygments <http://pygments.org/>`_ and `wcwidth
 <https://github.com/jquast/wcwidth>`_ libraries.
 
 
 Table of contents
@@ -86,8 +86,8 @@
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
 
 Prompt_toolkit was created by `Jonathan Slenders
-<http://github.com/jonathanslenders/>`_.
+<http://github.com/prompt_toolkit/>`_.
```

### Comparing `prompt_toolkit-3.0.8/docs/make.bat` & `prompt_toolkit-3.0.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/pages/advanced_topics/architecture.rst` & `prompt_toolkit-3.0.9/docs/pages/advanced_topics/architecture.rst`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/pages/advanced_topics/asyncio.rst` & `prompt_toolkit-3.0.9/docs/pages/advanced_topics/asyncio.rst`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/pages/advanced_topics/filters.rst` & `prompt_toolkit-3.0.9/docs/pages/advanced_topics/filters.rst`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/pages/advanced_topics/input_hooks.rst` & `prompt_toolkit-3.0.9/docs/pages/advanced_topics/input_hooks.rst`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/pages/advanced_topics/key_bindings.rst` & `prompt_toolkit-3.0.9/docs/pages/advanced_topics/key_bindings.rst`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     :kbd:`c-q` (control-q) and :kbd:`c-s` (control-s) are often captured by the
     terminal, because they were used traditionally for software flow control.
     When this is enabled, the application will automatically freeze when
     :kbd:`c-s` is pressed, until :kbd:`c-q` is pressed. It won't be possible to
     bind these keys.
 
-    In order to disable this, execute type the following in your shell, or even
+    In order to disable this, execute the following command in your shell, or even
     add it to your `.bashrc`.
 
     .. code::
 
         stty -ixon
 
 Key bindings can even consist of a sequence of multiple keys. The binding is
```

### Comparing `prompt_toolkit-3.0.8/docs/pages/advanced_topics/rendering_flow.rst` & `prompt_toolkit-3.0.9/docs/pages/advanced_topics/rendering_flow.rst`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/pages/advanced_topics/rendering_pipeline.rst` & `prompt_toolkit-3.0.9/docs/pages/advanced_topics/rendering_pipeline.rst`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/pages/advanced_topics/styling.rst` & `prompt_toolkit-3.0.9/docs/pages/advanced_topics/styling.rst`

 * *Files 0% similar despite different names*

```diff
@@ -221,15 +221,15 @@
 
 `Pygments <http://pygments.org/>`_ has a slightly different notation for
 specifying styles, because it maps styling to Pygments "Tokens". A Pygments
 style can however be loaded and used as follows:
 
 .. code:: python
 
-    from prompt_toolkit.styles.from_pygments import style_from_pygments_cls
+    from prompt_toolkit.styles.pygments import style_from_pygments_cls
     from pygments.styles import get_style_by_name
 
     style = style_from_pygments_cls(get_style_by_name('monokai'))
 
 
 Merging styles together
 -----------------------
@@ -261,15 +261,15 @@
 | 8 bit  | 256 colors      | ``ColorDepth.DEPTH_8_BIT``  | ``ColorDepth.DEFAULT``          |
 +--------+-----------------+-----------------------------+---------------------------------+
 | 24 bit | True colors     | ``ColorDepth.DEPTH_24_BIT`` | ``ColorDepth.TRUE_COLOR``       |
 +--------+-----------------+-----------------------------+---------------------------------+
 
 By default, 256 colors are used, because this is what most terminals support
 these days. If the ``TERM`` enviroment variable is set to ``linux`` or
-``eterm-color``, then only ANSI colors are used, because of these terminals. 24
+``eterm-color``, then only ANSI colors are used, because of these terminals. The 24
 bit true color output needs to be enabled explicitely. When 4 bit color output
 is chosen, all colors will be mapped to the closest ANSI color.
 
 Setting the default color depth for any prompt_toolkit application can be done
 by setting the ``PROMPT_TOOLKIT_COLOR_DEPTH`` environment variable. You could
 for instance copy the following into your `.bashrc` file.
```

### Comparing `prompt_toolkit-3.0.8/docs/pages/asking_for_input.rst` & `prompt_toolkit-3.0.9/docs/pages/asking_for_input.rst`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/pages/dialogs.rst` & `prompt_toolkit-3.0.9/docs/pages/dialogs.rst`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/pages/full_screen_apps.rst` & `prompt_toolkit-3.0.9/docs/pages/full_screen_apps.rst`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
       abstraction of the output stream, and is called by the renderer.
 
 Both are optional and normally not needed to pass explicitly. Usually, the
 default works fine.
 
 There is a third I/O object which is also required by the application, but not
 passed inside. This is the event loop, an
-:class:`~prompt_toolkit.eventloop.EventLoop` instance. This is basically a
+:class:`~prompt_toolkit.eventloop` instance. This is basically a
 while-true loop that waits for user input, and when it receives something (like
 a key press), it will send that to the the appropriate handler, like for
 instance, a key binding.
 
 When :func:`~prompt_toolkit.application.Application.run()` is called, the event
 loop will run until the application is done. An application will quit when 
 :func:`~prompt_toolkit.application.Application.exit()` is called.
@@ -127,18 +127,17 @@
   Normally, it is never needed to create new
   :class:`~prompt_toolkit.layout.UIControl` or
   :class:`~prompt_toolkit.layout.Container` classes, but instead you would
   create the layout by composing instances of the existing built-ins.
 
 - A higher level abstraction of building a layout is by using "widgets". A
   widget is a reusable layout component that can contain multiple containers
-  and controls. It should have a ``__pt__container__`` function, which is
-  supposed to return the root container for this widget. Prompt_toolkit
-  contains a couple of widgets like
-  :class:`~prompt_toolkit.widgets.TextArea`,
+  and controls. Widgets have a ``__pt__container__`` function, which returns
+  the root container for this widget. Prompt_toolkit contains a couple of
+  widgets like :class:`~prompt_toolkit.widgets.TextArea`,
   :class:`~prompt_toolkit.widgets.Button`,
   :class:`~prompt_toolkit.widgets.Frame`,
   :class:`~prompt_toolkit.widgets.VerticalLine` and so on.
 
 - The highest level abstractions can be found in the ``shortcuts`` module.
   There we don't have to think about the layout, controls and containers at
   all. This is the simplest way to use prompt_toolkit, but is only meant for
@@ -230,15 +229,15 @@
 condition is satisfied, use a
 :class:`~prompt_toolkit.layout.ConditionalContainer`.
 
 
 Focusing windows
 ^^^^^^^^^^^^^^^^^
 
-Focussing something can be done by calling the
+Focusing something can be done by calling the
 :meth:`~prompt_toolkit.layout.Layout.focus` method. This method is very
 flexible and accepts a :class:`~prompt_toolkit.layout.Window`, a
 :class:`~prompt_toolkit.buffer.Buffer`, a
 :class:`~prompt_toolkit.layout.controls.UIControl` and more.
 
 In the following example, we use :func:`~prompt_toolkit.application.get_app`
 for getting the active application.
@@ -319,19 +318,26 @@
 
 :ref:`Read more about key bindings ...<key_bindings>`
 
 
 Modal containers
 ^^^^^^^^^^^^^^^^
 
-All container objects, like :class:`~prompt_toolkit.layout.VSplit` and
-:class:`~prompt_toolkit.layout.HSplit` take a ``modal`` argument.
+The following container objects take a ``modal`` argument
+:class:`~prompt_toolkit.layout.VSplit`,
+:class:`~prompt_toolkit.layout.HSplit`, and
+:class:`~prompt_toolkit.layout.FloatContainer`.
 
-If this flag has been set, then key bindings from the parent are not
-taken into account if one of the children windows has the focus.
+Setting ``modal=True`` makes what is called a **modal** container. Normally, a
+child container would inherit its parent key bindings. This does not apply to
+**modal** containers.
+
+Consider a **modal** container (e.g. :class:`~prompt_toolkit.layout.VSplit`)
+is child of another container, its parent. Any key bindings from the parent
+are not taken into account if the **modal** container (child) has the focus.
 
 This is useful in a complex layout, where many controls have their own key
 bindings, but you only want to enable the key bindings for a certain region of
 the layout.
 
 The global key bindings are always active.
```

### Comparing `prompt_toolkit-3.0.8/docs/pages/gallery.rst` & `prompt_toolkit-3.0.9/docs/pages/gallery.rst`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/pages/getting_started.rst` & `prompt_toolkit-3.0.9/docs/pages/getting_started.rst`

 * *Files 4% similar despite different names*

```diff
@@ -20,16 +20,16 @@
 Several use cases: prompts versus full screen terminal applications
 --------------------------------------------------------------------
 
 `prompt_toolkit` was in the first place meant to be a replacement for readline.
 However, when it became more mature, we realised that all the components for
 full screen applications are there and `prompt_toolkit` is very capable of
 handling many use situations. `Pyvim
-<http://github.com/jonathanslenders/pyvim>`_ and `pymux
-<http://github.com/jonathanslenders/pymux>`_ are examples of full screen
+<http://github.com/prompt_toolkit/pyvim>`_ and `pymux
+<http://github.com/prompt_toolkit/pymux>`_ are examples of full screen
 applications.
 
 .. image:: ../images/pyvim.png
 
 Basically, at the core, `prompt_toolkit` has a layout engine, that supports
 horizontal and vertical splits as well as floats, where each "window" can
 display a user control. The API for user controls is simple yet powerful.
@@ -61,16 +61,16 @@
 
 
 Learning `prompt_toolkit`
 -------------------------
 
 In order to learn and understand `prompt_toolkit`, it is best to go through the
 all sections in the order below. Also don't forget to have a look at all the
-examples `examples
-<https://github.com/jonathanslenders/python-prompt-toolkit/tree/master/examples>`_
+`examples
+<https://github.com/prompt_toolkit/python-prompt-toolkit/tree/master/examples>`_
 in the repository.
 
 - First, :ref:`learn how to print text <printing_text>`. This is important,
   because it covers how to use "formatted text", which is something you'll use
   whenever you want to use colors anywhere.
 
 - Secondly, go through the :ref:`asking for input <asking_for_input>` section.
```

### Comparing `prompt_toolkit-3.0.8/docs/pages/printing_text.rst` & `prompt_toolkit-3.0.9/docs/pages/printing_text.rst`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/pages/progress_bars.rst` & `prompt_toolkit-3.0.9/docs/pages/progress_bars.rst`

 * *Files 1% similar despite different names*

```diff
@@ -197,15 +197,17 @@
 .. code:: python
 
     from prompt_toolkit import HTML
     from prompt_toolkit.key_binding import KeyBindings
     from prompt_toolkit.patch_stdout import patch_stdout
     from prompt_toolkit.shortcuts import ProgressBar
 
+    import os
     import time
+    import signal
 
     bottom_toolbar = HTML(' <b>[f]</b> Print "f" <b>[x]</b> Abort.')
 
     # Create custom key bindings first.
     kb = KeyBindings()
     cancel = [False]
```

### Comparing `prompt_toolkit-3.0.8/docs/pages/reference.rst` & `prompt_toolkit-3.0.9/docs/pages/reference.rst`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/pages/tutorials/repl.rst` & `prompt_toolkit-3.0.9/docs/pages/tutorials/repl.rst`

 * *Files 0% similar despite different names*

```diff
@@ -333,9 +333,9 @@
 .. image:: ../../images/repl/sqlite-6.png
 
 I hope that gives an idea of how to get started on building command line
 interfaces.
 
 The End.
 
-.. _prompt_toolkit: https://github.com/jonathanslenders/python-prompt-toolkit
+.. _prompt_toolkit: https://github.com/prompt_toolkit/python-prompt-toolkit
 .. _Pygments: http://pygments.org/
```

### Comparing `prompt_toolkit-3.0.8/docs/pages/upgrading/2.0.rst` & `prompt_toolkit-3.0.9/docs/pages/upgrading/2.0.rst`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/docs/pages/upgrading/3.0.rst` & `prompt_toolkit-3.0.9/docs/pages/upgrading/3.0.rst`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/dialogs/checkbox_dialog.py` & `prompt_toolkit-3.0.9/examples/dialogs/checkbox_dialog.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/dialogs/progress_dialog.py` & `prompt_toolkit-3.0.9/examples/dialogs/progress_dialog.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/dialogs/radio_dialog.py` & `prompt_toolkit-3.0.9/examples/dialogs/radio_dialog.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/dialogs/styled_messagebox.py` & `prompt_toolkit-3.0.9/examples/dialogs/styled_messagebox.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/full-screen/buttons.py` & `prompt_toolkit-3.0.9/examples/full-screen/buttons.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/full-screen/calculator.py` & `prompt_toolkit-3.0.9/examples/full-screen/calculator.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/full-screen/full-screen-demo.py` & `prompt_toolkit-3.0.9/examples/full-screen/full-screen-demo.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/full-screen/hello-world.py` & `prompt_toolkit-3.0.9/examples/full-screen/hello-world.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/full-screen/pager.py` & `prompt_toolkit-3.0.9/examples/full-screen/pager.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/full-screen/simple-demos/alignment.py` & `prompt_toolkit-3.0.9/examples/full-screen/simple-demos/alignment.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/full-screen/simple-demos/autocompletion.py` & `prompt_toolkit-3.0.9/examples/full-screen/simple-demos/autocompletion.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/full-screen/simple-demos/colorcolumn.py` & `prompt_toolkit-3.0.9/examples/full-screen/simple-demos/colorcolumn.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/full-screen/simple-demos/cursorcolumn-cursorline.py` & `prompt_toolkit-3.0.9/examples/full-screen/simple-demos/cursorcolumn-cursorline.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/full-screen/simple-demos/float-transparency.py` & `prompt_toolkit-3.0.9/examples/full-screen/simple-demos/float-transparency.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/full-screen/simple-demos/floats.py` & `prompt_toolkit-3.0.9/examples/full-screen/simple-demos/floats.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/full-screen/simple-demos/focus.py` & `prompt_toolkit-3.0.9/examples/full-screen/simple-demos/focus.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/full-screen/simple-demos/horizontal-align.py` & `prompt_toolkit-3.0.9/examples/full-screen/simple-demos/horizontal-align.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/full-screen/simple-demos/horizontal-split.py` & `prompt_toolkit-3.0.9/examples/full-screen/simple-demos/horizontal-split.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/full-screen/simple-demos/line-prefixes.py` & `prompt_toolkit-3.0.9/examples/full-screen/simple-demos/line-prefixes.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/full-screen/simple-demos/margins.py` & `prompt_toolkit-3.0.9/examples/full-screen/simple-demos/margins.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/full-screen/simple-demos/vertical-align.py` & `prompt_toolkit-3.0.9/examples/full-screen/simple-demos/vertical-align.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/full-screen/simple-demos/vertical-split.py` & `prompt_toolkit-3.0.9/examples/full-screen/simple-demos/vertical-split.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/full-screen/split-screen.py` & `prompt_toolkit-3.0.9/examples/full-screen/split-screen.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/full-screen/text-editor.py` & `prompt_toolkit-3.0.9/examples/full-screen/text-editor.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/gevent-get-input.py` & `prompt_toolkit-3.0.9/examples/gevent-get-input.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/print-text/ansi-colors.py` & `prompt_toolkit-3.0.9/examples/print-text/ansi-colors.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/print-text/ansi.py` & `prompt_toolkit-3.0.9/examples/print-text/ansi.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/print-text/html.py` & `prompt_toolkit-3.0.9/examples/print-text/html.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/print-text/named-colors.py` & `prompt_toolkit-3.0.9/examples/print-text/named-colors.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/print-text/print-formatted-text.py` & `prompt_toolkit-3.0.9/examples/print-text/print-formatted-text.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/print-text/pygments-tokens.py` & `prompt_toolkit-3.0.9/examples/print-text/pygments-tokens.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/print-text/true-color-demo.py` & `prompt_toolkit-3.0.9/examples/print-text/true-color-demo.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/progress-bar/a-lot-of-parallel-tasks.py` & `prompt_toolkit-3.0.9/examples/progress-bar/a-lot-of-parallel-tasks.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/progress-bar/colored-title-and-label.py` & `prompt_toolkit-3.0.9/examples/progress-bar/colored-title-and-label.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/progress-bar/custom-key-bindings.py` & `prompt_toolkit-3.0.9/examples/progress-bar/custom-key-bindings.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/progress-bar/many-parallel-tasks.py` & `prompt_toolkit-3.0.9/examples/progress-bar/many-parallel-tasks.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/progress-bar/nested-progress-bars.py` & `prompt_toolkit-3.0.9/examples/progress-bar/nested-progress-bars.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/progress-bar/scrolling-task-name.py` & `prompt_toolkit-3.0.9/examples/progress-bar/scrolling-task-name.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/progress-bar/styled-1.py` & `prompt_toolkit-3.0.9/examples/progress-bar/styled-1.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/progress-bar/styled-2.py` & `prompt_toolkit-3.0.9/examples/progress-bar/styled-2.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/progress-bar/styled-apt-get-install.py` & `prompt_toolkit-3.0.9/examples/progress-bar/styled-apt-get-install.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/progress-bar/styled-rainbow.py` & `prompt_toolkit-3.0.9/examples/progress-bar/styled-rainbow.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/progress-bar/styled-tqdm-1.py` & `prompt_toolkit-3.0.9/examples/progress-bar/styled-tqdm-1.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/progress-bar/styled-tqdm-2.py` & `prompt_toolkit-3.0.9/examples/progress-bar/styled-tqdm-2.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/progress-bar/two-tasks.py` & `prompt_toolkit-3.0.9/examples/progress-bar/two-tasks.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/progress-bar/unknown-length.py` & `prompt_toolkit-3.0.9/examples/progress-bar/unknown-length.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/asyncio-prompt.py` & `prompt_toolkit-3.0.9/examples/prompts/asyncio-prompt.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/auto-completion/autocomplete-with-control-space.py` & `prompt_toolkit-3.0.9/examples/prompts/auto-completion/autocomplete-with-control-space.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/auto-completion/autocompletion-like-readline.py` & `prompt_toolkit-3.0.9/examples/prompts/auto-completion/autocompletion-like-readline.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/auto-completion/autocompletion.py` & `prompt_toolkit-3.0.9/examples/prompts/auto-completion/autocompletion.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/auto-completion/colored-completions-with-formatted-text.py` & `prompt_toolkit-3.0.9/examples/prompts/auto-completion/colored-completions-with-formatted-text.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/auto-completion/colored-completions.py` & `prompt_toolkit-3.0.9/examples/prompts/auto-completion/colored-completions.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/auto-completion/combine-multiple-completers.py` & `prompt_toolkit-3.0.9/examples/prompts/auto-completion/combine-multiple-completers.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/auto-completion/fuzzy-custom-completer.py` & `prompt_toolkit-3.0.9/examples/prompts/auto-completion/fuzzy-custom-completer.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/auto-completion/fuzzy-word-completer.py` & `prompt_toolkit-3.0.9/examples/prompts/auto-completion/fuzzy-word-completer.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/auto-completion/multi-column-autocompletion-with-meta.py` & `prompt_toolkit-3.0.9/examples/prompts/auto-completion/multi-column-autocompletion-with-meta.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/auto-completion/multi-column-autocompletion.py` & `prompt_toolkit-3.0.9/examples/prompts/auto-completion/multi-column-autocompletion.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/auto-completion/slow-completions.py` & `prompt_toolkit-3.0.9/examples/prompts/auto-completion/slow-completions.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/auto-suggestion.py` & `prompt_toolkit-3.0.9/examples/prompts/auto-suggestion.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/autocorrection.py` & `prompt_toolkit-3.0.9/examples/prompts/autocorrection.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/bottom-toolbar.py` & `prompt_toolkit-3.0.9/examples/prompts/bottom-toolbar.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/clock-input.py` & `prompt_toolkit-3.0.9/examples/prompts/clock-input.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/colored-prompt.py` & `prompt_toolkit-3.0.9/examples/prompts/colored-prompt.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/custom-key-binding.py` & `prompt_toolkit-3.0.9/examples/prompts/custom-key-binding.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/custom-lexer.py` & `prompt_toolkit-3.0.9/examples/prompts/custom-lexer.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/custom-vi-operator-and-text-object.py` & `prompt_toolkit-3.0.9/examples/prompts/custom-vi-operator-and-text-object.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/fancy-zsh-prompt.py` & `prompt_toolkit-3.0.9/examples/prompts/fancy-zsh-prompt.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/finalterm-shell-integration.py` & `prompt_toolkit-3.0.9/examples/prompts/finalterm-shell-integration.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/get-multiline-input.py` & `prompt_toolkit-3.0.9/examples/prompts/get-multiline-input.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/get-password-with-toggle-display-shortcut.py` & `prompt_toolkit-3.0.9/examples/prompts/get-password-with-toggle-display-shortcut.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/history/persistent-history.py` & `prompt_toolkit-3.0.9/examples/prompts/history/persistent-history.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/history/slow-history.py` & `prompt_toolkit-3.0.9/examples/prompts/history/slow-history.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/input-validation.py` & `prompt_toolkit-3.0.9/examples/prompts/input-validation.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/inputhook.py` & `prompt_toolkit-3.0.9/examples/prompts/inputhook.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/patch-stdout.py` & `prompt_toolkit-3.0.9/examples/prompts/patch-stdout.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/regular-language.py` & `prompt_toolkit-3.0.9/examples/prompts/regular-language.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/rprompt.py` & `prompt_toolkit-3.0.9/examples/prompts/rprompt.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/swap-light-and-dark-colors.py` & `prompt_toolkit-3.0.9/examples/prompts/swap-light-and-dark-colors.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/switch-between-vi-emacs.py` & `prompt_toolkit-3.0.9/examples/prompts/switch-between-vi-emacs.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/system-clipboard-integration.py` & `prompt_toolkit-3.0.9/examples/prompts/system-clipboard-integration.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/system-prompt.py` & `prompt_toolkit-3.0.9/examples/prompts/system-prompt.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/prompts/up-arrow-partial-string-matching.py` & `prompt_toolkit-3.0.9/examples/prompts/up-arrow-partial-string-matching.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/ssh/asyncssh-server.py` & `prompt_toolkit-3.0.9/examples/ssh/asyncssh-server.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/telnet/chat-app.py` & `prompt_toolkit-3.0.9/examples/telnet/chat-app.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/telnet/dialog.py` & `prompt_toolkit-3.0.9/examples/telnet/dialog.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/telnet/hello-world.py` & `prompt_toolkit-3.0.9/examples/telnet/hello-world.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/telnet/toolbar.py` & `prompt_toolkit-3.0.9/examples/telnet/toolbar.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/examples/tutorial/sqlite-cli.py` & `prompt_toolkit-3.0.9/examples/tutorial/sqlite-cli.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/__init__.py` & `prompt_toolkit-3.0.9/prompt_toolkit/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 `prompt_toolkit.shortcuts.prompt`.
 """
 from .application import Application
 from .formatted_text import ANSI, HTML
 from .shortcuts import PromptSession, print_formatted_text, prompt
 
 # Don't forget to update in `docs/conf.py`!
-__version__ = "3.0.8"
+__version__ = "3.0.9"
 
 # Version tuple.
 VERSION = tuple(__version__.split("."))
 
 
 __all__ = [
     # Application.
```

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/application/__init__.py` & `prompt_toolkit-3.0.9/prompt_toolkit/application/__init__.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/application/application.py` & `prompt_toolkit-3.0.9/prompt_toolkit/application/application.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/application/current.py` & `prompt_toolkit-3.0.9/prompt_toolkit/application/current.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/application/dummy.py` & `prompt_toolkit-3.0.9/prompt_toolkit/application/dummy.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/application/run_in_terminal.py` & `prompt_toolkit-3.0.9/prompt_toolkit/application/run_in_terminal.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/auto_suggest.py` & `prompt_toolkit-3.0.9/prompt_toolkit/auto_suggest.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/buffer.py` & `prompt_toolkit-3.0.9/prompt_toolkit/buffer.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/cache.py` & `prompt_toolkit-3.0.9/prompt_toolkit/cache.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/clipboard/base.py` & `prompt_toolkit-3.0.9/prompt_toolkit/clipboard/base.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/clipboard/in_memory.py` & `prompt_toolkit-3.0.9/prompt_toolkit/clipboard/in_memory.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/clipboard/pyperclip.py` & `prompt_toolkit-3.0.9/prompt_toolkit/clipboard/pyperclip.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/completion/__init__.py` & `prompt_toolkit-3.0.9/prompt_toolkit/completion/__init__.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/completion/base.py` & `prompt_toolkit-3.0.9/prompt_toolkit/completion/base.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/completion/filesystem.py` & `prompt_toolkit-3.0.9/prompt_toolkit/completion/filesystem.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/completion/fuzzy_completer.py` & `prompt_toolkit-3.0.9/prompt_toolkit/completion/fuzzy_completer.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/completion/nested.py` & `prompt_toolkit-3.0.9/prompt_toolkit/completion/nested.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/completion/word_completer.py` & `prompt_toolkit-3.0.9/prompt_toolkit/completion/word_completer.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/contrib/completers/system.py` & `prompt_toolkit-3.0.9/prompt_toolkit/contrib/completers/system.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/contrib/regular_languages/__init__.py` & `prompt_toolkit-3.0.9/prompt_toolkit/contrib/regular_languages/__init__.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/contrib/regular_languages/compiler.py` & `prompt_toolkit-3.0.9/prompt_toolkit/contrib/regular_languages/compiler.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/contrib/regular_languages/completion.py` & `prompt_toolkit-3.0.9/prompt_toolkit/contrib/regular_languages/completion.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/contrib/regular_languages/lexer.py` & `prompt_toolkit-3.0.9/prompt_toolkit/contrib/regular_languages/lexer.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/contrib/regular_languages/regex_parser.py` & `prompt_toolkit-3.0.9/prompt_toolkit/contrib/regular_languages/regex_parser.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/contrib/regular_languages/validation.py` & `prompt_toolkit-3.0.9/prompt_toolkit/contrib/regular_languages/validation.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/contrib/ssh/server.py` & `prompt_toolkit-3.0.9/prompt_toolkit/contrib/ssh/server.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/contrib/telnet/protocol.py` & `prompt_toolkit-3.0.9/prompt_toolkit/contrib/telnet/protocol.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/contrib/telnet/server.py` & `prompt_toolkit-3.0.9/prompt_toolkit/contrib/telnet/server.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/document.py` & `prompt_toolkit-3.0.9/prompt_toolkit/document.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/eventloop/__init__.py` & `prompt_toolkit-3.0.9/prompt_toolkit/eventloop/__init__.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/eventloop/async_context_manager.py` & `prompt_toolkit-3.0.9/prompt_toolkit/eventloop/async_context_manager.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/eventloop/async_generator.py` & `prompt_toolkit-3.0.9/prompt_toolkit/eventloop/async_generator.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/eventloop/dummy_contextvars.py` & `prompt_toolkit-3.0.9/prompt_toolkit/eventloop/dummy_contextvars.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/eventloop/inputhook.py` & `prompt_toolkit-3.0.9/prompt_toolkit/eventloop/inputhook.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/eventloop/utils.py` & `prompt_toolkit-3.0.9/prompt_toolkit/eventloop/utils.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/eventloop/win32.py` & `prompt_toolkit-3.0.9/prompt_toolkit/eventloop/win32.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/filters/__init__.py` & `prompt_toolkit-3.0.9/prompt_toolkit/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/filters/app.py` & `prompt_toolkit-3.0.9/prompt_toolkit/filters/app.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/filters/base.py` & `prompt_toolkit-3.0.9/prompt_toolkit/filters/base.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/filters/cli.py` & `prompt_toolkit-3.0.9/prompt_toolkit/filters/cli.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/filters/utils.py` & `prompt_toolkit-3.0.9/prompt_toolkit/filters/utils.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/formatted_text/__init__.py` & `prompt_toolkit-3.0.9/prompt_toolkit/formatted_text/__init__.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/formatted_text/ansi.py` & `prompt_toolkit-3.0.9/prompt_toolkit/formatted_text/ansi.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/formatted_text/base.py` & `prompt_toolkit-3.0.9/prompt_toolkit/formatted_text/base.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/formatted_text/html.py` & `prompt_toolkit-3.0.9/prompt_toolkit/formatted_text/html.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/formatted_text/pygments.py` & `prompt_toolkit-3.0.9/prompt_toolkit/formatted_text/pygments.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/formatted_text/utils.py` & `prompt_toolkit-3.0.9/prompt_toolkit/formatted_text/utils.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/history.py` & `prompt_toolkit-3.0.9/prompt_toolkit/history.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Implementations for the history of a `Buffer`.
 
-NOTE: Notice that there is no `DynamicHistory`. This doesn't work well, because
-      the `Buffer` needs to be able to attach an event handler to the event
-      when a history entry is loaded. This loading can be done asynchronously
-      and making the history swappable would probably break this.
+NOTE: There is no `DynamicHistory`:
+      This doesn't work well, because the `Buffer` needs to be able to attach
+      an event handler to the event when a history entry is loaded. This
+      loading can be done asynchronously and making the history swappable would
+      probably break this.
 """
 import datetime
 import os
 from abc import ABCMeta, abstractmethod
 from threading import Thread
 from typing import Callable, Iterable, List, Optional
 
@@ -203,15 +204,15 @@
                 string = "".join(lines)[:-1]
 
                 strings.append(string)
 
         if os.path.exists(self.filename):
             with open(self.filename, "rb") as f:
                 for line_bytes in f:
-                    line = line_bytes.decode("utf-8")
+                    line = line_bytes.decode("utf-8", errors="replace")
 
                     if line.startswith("+"):
                         lines.append(line[1:])
                     else:
                         add()
                         lines = []
```

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/input/ansi_escape_sequences.py` & `prompt_toolkit-3.0.9/prompt_toolkit/input/ansi_escape_sequences.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,15 @@
     "\x1b[3~": Keys.Delete,
     "\x1b[4~": Keys.End,  # tmux
     "\x1b[5~": Keys.PageUp,
     "\x1b[6~": Keys.PageDown,
     "\x1b[7~": Keys.Home,  # xrvt
     "\x1b[8~": Keys.End,  # xrvt
     "\x1b[Z": Keys.BackTab,  # shift + tab
+    "\x1b\x09": Keys.BackTab,  # Linux console
     # --
     # Function keys.
     "\x1bOP": Keys.F1,
     "\x1bOQ": Keys.F2,
     "\x1bOR": Keys.F3,
     "\x1bOS": Keys.F4,
     "\x1b[[A": Keys.F1,  # Linux console.
```

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/input/base.py` & `prompt_toolkit-3.0.9/prompt_toolkit/input/base.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/input/defaults.py` & `prompt_toolkit-3.0.9/prompt_toolkit/input/defaults.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/input/posix_pipe.py` & `prompt_toolkit-3.0.9/prompt_toolkit/input/posix_pipe.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/input/posix_utils.py` & `prompt_toolkit-3.0.9/prompt_toolkit/input/posix_utils.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/input/typeahead.py` & `prompt_toolkit-3.0.9/prompt_toolkit/input/typeahead.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/input/vt100.py` & `prompt_toolkit-3.0.9/prompt_toolkit/input/vt100.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/input/vt100_parser.py` & `prompt_toolkit-3.0.9/prompt_toolkit/input/vt100_parser.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/input/win32.py` & `prompt_toolkit-3.0.9/prompt_toolkit/input/win32.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/input/win32_pipe.py` & `prompt_toolkit-3.0.9/prompt_toolkit/input/win32_pipe.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/auto_suggest.py` & `prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/auto_suggest.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/basic.py` & `prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/basic.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/completion.py` & `prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/completion.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/cpr.py` & `prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/cpr.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/emacs.py` & `prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/emacs.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/mouse.py` & `prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/mouse.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/named_commands.py` & `prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/named_commands.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/open_in_editor.py` & `prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/open_in_editor.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/page_navigation.py` & `prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/page_navigation.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/scroll.py` & `prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/scroll.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/search.py` & `prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/search.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/key_binding/bindings/vi.py` & `prompt_toolkit-3.0.9/prompt_toolkit/key_binding/bindings/vi.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/key_binding/defaults.py` & `prompt_toolkit-3.0.9/prompt_toolkit/key_binding/defaults.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/key_binding/digraphs.py` & `prompt_toolkit-3.0.9/prompt_toolkit/key_binding/digraphs.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/key_binding/emacs_state.py` & `prompt_toolkit-3.0.9/prompt_toolkit/key_binding/emacs_state.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/key_binding/key_bindings.py` & `prompt_toolkit-3.0.9/prompt_toolkit/key_binding/key_bindings.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/key_binding/key_processor.py` & `prompt_toolkit-3.0.9/prompt_toolkit/key_binding/key_processor.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/key_binding/vi_state.py` & `prompt_toolkit-3.0.9/prompt_toolkit/key_binding/vi_state.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/keys.py` & `prompt_toolkit-3.0.9/prompt_toolkit/keys.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/layout/__init__.py` & `prompt_toolkit-3.0.9/prompt_toolkit/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/layout/containers.py` & `prompt_toolkit-3.0.9/prompt_toolkit/layout/containers.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/layout/controls.py` & `prompt_toolkit-3.0.9/prompt_toolkit/layout/controls.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/layout/dimension.py` & `prompt_toolkit-3.0.9/prompt_toolkit/layout/dimension.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/layout/dummy.py` & `prompt_toolkit-3.0.9/prompt_toolkit/layout/dummy.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/layout/layout.py` & `prompt_toolkit-3.0.9/prompt_toolkit/layout/layout.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/layout/margins.py` & `prompt_toolkit-3.0.9/prompt_toolkit/layout/margins.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/layout/menus.py` & `prompt_toolkit-3.0.9/prompt_toolkit/layout/menus.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/layout/mouse_handlers.py` & `prompt_toolkit-3.0.9/prompt_toolkit/layout/mouse_handlers.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/layout/processors.py` & `prompt_toolkit-3.0.9/prompt_toolkit/layout/processors.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 SourceToDisplay = Callable[[int], int]
 DisplayToSource = Callable[[int], int]
 
 
 class TransformationInput:
     """
-    :param control: :class:`.BufferControl` instance.
+    :param buffer_control: :class:`.BufferControl` instance.
     :param lineno: The number of the line to which we apply the processor.
     :param source_to_display: A function that returns the position in the
         `fragments` for any position in the source string. (This takes
         previous processors into account.)
     :param fragments: List of fragments that we can transform. (Received from the
         previous processor.)
     """
```

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/layout/screen.py` & `prompt_toolkit-3.0.9/prompt_toolkit/layout/screen.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/layout/utils.py` & `prompt_toolkit-3.0.9/prompt_toolkit/layout/utils.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/lexers/base.py` & `prompt_toolkit-3.0.9/prompt_toolkit/lexers/base.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/lexers/pygments.py` & `prompt_toolkit-3.0.9/prompt_toolkit/lexers/pygments.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/mouse_events.py` & `prompt_toolkit-3.0.9/prompt_toolkit/mouse_events.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/output/base.py` & `prompt_toolkit-3.0.9/prompt_toolkit/output/base.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/output/color_depth.py` & `prompt_toolkit-3.0.9/prompt_toolkit/output/color_depth.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/output/conemu.py` & `prompt_toolkit-3.0.9/prompt_toolkit/output/conemu.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/output/defaults.py` & `prompt_toolkit-3.0.9/prompt_toolkit/output/defaults.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/output/vt100.py` & `prompt_toolkit-3.0.9/prompt_toolkit/output/vt100.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/output/win32.py` & `prompt_toolkit-3.0.9/prompt_toolkit/output/win32.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/output/windows10.py` & `prompt_toolkit-3.0.9/prompt_toolkit/output/windows10.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/patch_stdout.py` & `prompt_toolkit-3.0.9/prompt_toolkit/patch_stdout.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/renderer.py` & `prompt_toolkit-3.0.9/prompt_toolkit/renderer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Renders the command line on the console.
 (Redraws parts of the input line that were changed.)
 """
-from asyncio import FIRST_COMPLETED, Future, sleep, wait
+from asyncio import FIRST_COMPLETED, Future, ensure_future, sleep, wait
 from collections import deque
 from enum import Enum
 from typing import TYPE_CHECKING, Any, Callable, Deque, Dict, Hashable, Optional, Tuple
 
 from prompt_toolkit.application.current import get_app
 from prompt_toolkit.data_structures import Point, Size
 from prompt_toolkit.filters import FilterOrBool, to_filter
@@ -562,19 +562,19 @@
             await sleep(timeout)
 
             # Got timeout, erase queue.
             for response_f in cpr_futures:
                 response_f.cancel()
             self._waiting_for_cpr_futures = deque()
 
-        coroutines = [
-            wait_for_responses(),
-            wait_for_timeout(),
-        ]
-        _, pending = await wait(coroutines, return_when=FIRST_COMPLETED)
+        tasks = {
+            ensure_future(wait_for_responses()),
+            ensure_future(wait_for_timeout()),
+        }
+        _, pending = await wait(tasks, return_when=FIRST_COMPLETED)
         for task in pending:
             task.cancel()
 
     def render(
         self, app: "Application[Any]", layout: "Layout", is_done: bool = False
     ) -> None:
         """
@@ -627,15 +627,15 @@
                 self._min_available_height,
                 last_height,
                 layout.container.preferred_height(size.columns, size.rows).preferred,
             )
 
         height = min(height, size.rows)
 
-        # When te size changes, don't consider the previous screen.
+        # When the size changes, don't consider the previous screen.
         if self._last_size != size:
             self._last_screen = None
 
         # When we render using another style or another color depth, do a full
         # repaint. (Forget about the previous rendered screen.)
         # (But note that we still use _last_screen to calculate the height.)
         if (
@@ -753,27 +753,31 @@
     fragments = to_formatted_text(formatted_text)
     style_transformation = style_transformation or DummyStyleTransformation()
     color_depth = color_depth or output.get_default_color_depth()
 
     # Reset first.
     output.reset_attributes()
     output.enable_autowrap()
+    last_attrs: Optional[Attrs] = None
 
     # Print all (style_str, text) tuples.
     attrs_for_style_string = _StyleStringToAttrsCache(
         style.get_attrs_for_style_str, style_transformation
     )
 
     for style_str, text, *_ in fragments:
         attrs = attrs_for_style_string[style_str]
 
-        if attrs:
-            output.set_attributes(attrs, color_depth)
-        else:
-            output.reset_attributes()
+        # Set style attributes if something changed.
+        if attrs != last_attrs:
+            if attrs:
+                output.set_attributes(attrs, color_depth)
+            else:
+                output.reset_attributes()
+        last_attrs = attrs
 
         # Eliminate carriage returns
         text = text.replace("\r", "")
 
         # Assume that the output is raw, and insert a carriage return before
         # every newline. (Also important when the front-end is a telnet client.)
         output.write(text.replace("\n", "\r\n"))
```

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/search.py` & `prompt_toolkit-3.0.9/prompt_toolkit/search.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/selection.py` & `prompt_toolkit-3.0.9/prompt_toolkit/selection.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/shortcuts/__init__.py` & `prompt_toolkit-3.0.9/prompt_toolkit/shortcuts/__init__.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/shortcuts/dialogs.py` & `prompt_toolkit-3.0.9/prompt_toolkit/shortcuts/dialogs.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/shortcuts/progress_bar/base.py` & `prompt_toolkit-3.0.9/prompt_toolkit/shortcuts/progress_bar/base.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/shortcuts/progress_bar/formatters.py` & `prompt_toolkit-3.0.9/prompt_toolkit/shortcuts/progress_bar/formatters.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/shortcuts/prompt.py` & `prompt_toolkit-3.0.9/prompt_toolkit/shortcuts/prompt.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/shortcuts/utils.py` & `prompt_toolkit-3.0.9/prompt_toolkit/shortcuts/utils.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/styles/__init__.py` & `prompt_toolkit-3.0.9/prompt_toolkit/styles/__init__.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/styles/base.py` & `prompt_toolkit-3.0.9/prompt_toolkit/styles/base.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/styles/defaults.py` & `prompt_toolkit-3.0.9/prompt_toolkit/styles/defaults.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/styles/named_colors.py` & `prompt_toolkit-3.0.9/prompt_toolkit/styles/named_colors.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/styles/pygments.py` & `prompt_toolkit-3.0.9/prompt_toolkit/styles/pygments.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/styles/style.py` & `prompt_toolkit-3.0.9/prompt_toolkit/styles/style.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/styles/style_transformation.py` & `prompt_toolkit-3.0.9/prompt_toolkit/styles/style_transformation.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/utils.py` & `prompt_toolkit-3.0.9/prompt_toolkit/utils.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/validation.py` & `prompt_toolkit-3.0.9/prompt_toolkit/validation.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/widgets/__init__.py` & `prompt_toolkit-3.0.9/prompt_toolkit/widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/widgets/base.py` & `prompt_toolkit-3.0.9/prompt_toolkit/widgets/base.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/widgets/dialogs.py` & `prompt_toolkit-3.0.9/prompt_toolkit/widgets/dialogs.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/widgets/menus.py` & `prompt_toolkit-3.0.9/prompt_toolkit/widgets/menus.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/widgets/toolbars.py` & `prompt_toolkit-3.0.9/prompt_toolkit/widgets/toolbars.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit/win32_types.py` & `prompt_toolkit-3.0.9/prompt_toolkit/win32_types.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit.egg-info/PKG-INFO` & `prompt_toolkit-3.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: prompt-toolkit
-Version: 3.0.8
+Name: prompt_toolkit
+Version: 3.0.9
 Summary: Library for building powerful interactive command lines in Python
 Home-page: https://github.com/prompt-toolkit/python-prompt-toolkit
 Author: Jonathan Slenders
 License: UNKNOWN
 Description: Python Prompt Toolkit
         =====================
```

### Comparing `prompt_toolkit-3.0.8/prompt_toolkit.egg-info/SOURCES.txt` & `prompt_toolkit-3.0.9/prompt_toolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/setup.py` & `prompt_toolkit-3.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/tests/test_async_generator.py` & `prompt_toolkit-3.0.9/tests/test_async_generator.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/tests/test_buffer.py` & `prompt_toolkit-3.0.9/tests/test_buffer.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/tests/test_cli.py` & `prompt_toolkit-3.0.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/tests/test_completion.py` & `prompt_toolkit-3.0.9/tests/test_completion.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/tests/test_document.py` & `prompt_toolkit-3.0.9/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/tests/test_filter.py` & `prompt_toolkit-3.0.9/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/tests/test_formatted_text.py` & `prompt_toolkit-3.0.9/tests/test_formatted_text.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/tests/test_inputstream.py` & `prompt_toolkit-3.0.9/tests/test_inputstream.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/tests/test_key_binding.py` & `prompt_toolkit-3.0.9/tests/test_key_binding.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/tests/test_layout.py` & `prompt_toolkit-3.0.9/tests/test_layout.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/tests/test_print_formatted_text.py` & `prompt_toolkit-3.0.9/tests/test_print_formatted_text.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/tests/test_regular_languages.py` & `prompt_toolkit-3.0.9/tests/test_regular_languages.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/tests/test_shortcuts.py` & `prompt_toolkit-3.0.9/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/tests/test_style.py` & `prompt_toolkit-3.0.9/tests/test_style.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/tests/test_style_transformation.py` & `prompt_toolkit-3.0.9/tests/test_style_transformation.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/tests/test_utils.py` & `prompt_toolkit-3.0.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/tests/test_vt100_output.py` & `prompt_toolkit-3.0.9/tests/test_vt100_output.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/tests/test_yank_nth_arg.py` & `prompt_toolkit-3.0.9/tests/test_yank_nth_arg.py`

 * *Files identical despite different names*

### Comparing `prompt_toolkit-3.0.8/tools/debug_vt100_input.py` & `prompt_toolkit-3.0.9/tools/debug_vt100_input.py`

 * *Files identical despite different names*

