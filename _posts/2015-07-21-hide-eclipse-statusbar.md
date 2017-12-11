---
layout: post
title: Hide status bar on Eclipse MARS
---

Steps to hide the status bar in Eclipse MARS

* Edit eclipse/plugins/org.eclipse.ui.themes_1.1.0.v20150511-0913/css/e4_basestyle.css
* Add the following lines to the end of the file

```sh
#org-eclipse-ui-trim-status,
#org-eclipse-ui-trim-vertical1,
#org-eclipse-ui-trim-vertical2 {
   visibility: hidden;
}
```

