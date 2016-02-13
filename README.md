My settings of Sublime Text2.

# install "Package Control"

- https://packagecontrol.io/installation#st2
    - Type `Ctrl + \``, [Paste], [Enter].
- Restart.
- Check [Preferences]-[Package Control].
- `Ctrl + Shift + p`

# install "Markdown Preview"

- `Ctrl + Shift + p`
- "Package Control: Install Package"
- type "Markdown Preview", install.

## use Markdown Preview..

- `Ctrl + Shift + p`
- "Markdown Preview: Preview in browser"-"markdown"

## Customize CSS

Draw a line around codeblocks.

### File Path

```
C:\Users\{USER}\AppData\Roaming\Sublime Text 2\Packages\Markdown Preview\markdown.css
```

replace a file with `Packages/Markdown Preview/markdown.css` or diff:

```
[ozuma@cent6 sublime2config]$ diff -u markdown.css Packages/Markdown\ Preview/markdown.css
--- markdown.css        2016-02-13 17:31:30.000000000 +0900
+++ Packages/Markdown Preview/markdown.css      2016-02-14 02:10:26.953737618 +0900
@@ -140,7 +140,7 @@
 .markdown-body .linenos,
 .markdown-body .code,
 .markdown-body .codehilitetable td {
-  border: 0;
+  border: 1px;
   padding: 0;
 }

@@ -381,21 +381,29 @@

 .markdown-body h1 {
   padding-bottom: 0.3em;
-  font-size: 2.25em;
+  padding-left: 0.2em;
+  font-size: 2em;
   line-height: 1.2;
-  border-bottom: 1px solid #eee;
+  background-color: #dddddd;
+  border-left: 3px solid #000;
+  border-right: 3px solid #000;
+  border-bottom: 2px solid #000;
+  border-top: 2px solid #000;
 }

 .markdown-body h2 {
   padding-bottom: 0.3em;
+  padding-left: 0.1em;
   font-size: 1.75em;
   line-height: 1.225;
-  border-bottom: 1px solid #eee;
+  border-left: 3px solid #000;
+  border-bottom: 1px solid #000;
 }

 .markdown-body h3 {
-  font-size: 1.5em;
+  font-size: 1.4em;
   line-height: 1.43;
+  border-bottom: 1px solid #666;
 }

 .markdown-body h4 {
@@ -469,6 +477,8 @@
   padding: 0 15px;
   color: #777;
   border-left: 4px solid #ddd;
+  margin-left: 2em;
+  font-size: 0.8em;
 }

 .markdown-body blockquote>:first-child {
@@ -521,6 +531,7 @@
   font-size: 85%;
   background-color: rgba(0,0,0,0.04);
   border-radius: 3px;
+  border: 1px solid #000000;
 }

 .markdown-body code:before,
[ozuma@cent6 sublime2config]$
```

# install "IMESupport"

inline typing for Japanese Input method.

- `Ctrl + Shift + p`
- "Package Control: Install Package"
- "IMESupport"
