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
macmini:Markdown Preview ozuma$ diff --unified=10 markdown.css.org markdown.css
--- markdown.css.org 2016-02-21 23:52:59.000000000 +0900
+++ markdown.css  2016-03-10 16:01:09.000000000 +0900
@@ -133,21 +133,21 @@
 }
 
 .markdown-body .codehilitetable pre,
 .markdown-body .codehilitetable div.codehilite {
   margin: 0;
 }
 
 .markdown-body .linenos,
 .markdown-body .code,
 .markdown-body .codehilitetable td {
-  border: 0;
+  border: 1px;
   padding: 0;
 }
 
 .markdown-body td:not(.linenos) .linenodiv {
   padding: 0 !important;
 }
 
 .markdown-body .code {
   width: 100%;
 }
@@ -374,35 +374,43 @@
 .markdown-body h2:hover .headeranchor-link .headeranchor,
 .markdown-body h3:hover .headeranchor-link .headeranchor,
 .markdown-body h4:hover .headeranchor-link .headeranchor,
 .markdown-body h5:hover .headeranchor-link .headeranchor,
 .markdown-body h6:hover .headeranchor-link .headeranchor {
   display: inline-block;
 }
 
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
   font-size: 1.25em;
 }
 
 .markdown-body h5 {
   font-size: 1em;
 }
 
@@ -462,20 +470,22 @@
 
 .markdown-body dl dd {
   padding: 0 16px;
   margin-bottom: 16px;
 }
 
 .markdown-body blockquote {
   padding: 0 15px;
   color: #777;
   border-left: 4px solid #ddd;
+  margin-left: 2em;
+  font-size: 0.8em;
 }
 
 .markdown-body blockquote>:first-child {
   margin-top: 0;
 }
 
 .markdown-body blockquote>:last-child {
   margin-bottom: 0;
 }
 
@@ -514,20 +524,21 @@
 
 .markdown-body code,
 .markdown-body samp {
   padding: 0;
   padding-top: 0.2em;
   padding-bottom: 0.2em;
   margin: 0;
   font-size: 85%;
   background-color: rgba(0,0,0,0.04);
   border-radius: 3px;
+  border: 1px solid #000000;
 }
 
 .markdown-body code:before,
 .markdown-body code:after {
   letter-spacing: -0.2em;
   content: "\00a0";
 }
 
 .markdown-body pre>code {
   padding: 0;
macmini:Markdown Preview ozuma$ 
```

# install "IMESupport"

inline typing for Japanese Input method.

- `Ctrl + Shift + p`
- "Package Control: Install Package"
- "IMESupport"
