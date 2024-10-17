---
description: There are some small things you might need to know about writing with Latex
---

# Latex Writing: Something to know

{% hint style="info" %}
Additional readings with examples:&#x20;

* Paper Writing Tips by MLNLP-World: [https://github.com/MLNLP-World/Paper-Writing-Tips](https://github.com/MLNLP-World/Paper-Writing-Tips)
{% endhint %}

Something that speeds up your writing:

* [ ] Latex  Equation tool：[https://www.mathjax.org/#demo](https://www.mathjax.org/#demo)
* [ ] Make your Tables beautiful:
  * [ ] Latex Table tool (Latex/Markdown/Excel/HTML): [basic table converter,](https://www.tablesgenerator.com/) [fancy tables tool ](https://www.latex-tables.com)&#x20;
  * [ ] Take a look at [the guide](https://people.inf.ethz.ch/markusp/teaching/guides/guide-tables.pdf), basically, it's:
    * [ ] Avoid vertical lines
    * [ ] Avoid “boxing up” cells, usually 3 horizontal lines are enough: above, below, and after the heading (see examples in this guide)
    * [ ] Avoid double horizontal lines
    * [ ] Enough space between rows
    * [ ] If in doubt, align left
  * [ ] Try `\toprule`, `\midrule`, `\bottomrule`
* [ ] [Latex fonts](latex-fonts.md) gallery
* [ ] Latex Math Equation gallery: [中文版](https://www.jianshu.com/p/97ec8a3739f6),  [English version](https://tilburgsciencehub.com/building-blocks/collaborate-and-share-your-work/write-your-paper/amsmath-latex-cheatsheet/)
* [ ] Make full use of the Macro definition (宏定义), which could be super helpful to refer to the frequently used terms, like the name of your proposed method, your dataset name, or baseline method.
  * [ ] You could use [the command file](predefined-latex-commands.md) directly as a starter.
  *   [ ] Define your method as `\ours` and directly use it in the main body of the paper - this will help you change the method name quickly until you finalize it in later stages of paper writing. For example, it could be:

      &#x20;

      `\newcommand{\datasetFont}{\text}`&#x20;

      `\newcommand{\ours}{\datasetFont{MixupExplainer}\xspace}`
* [ ] Latex Debug tip: If you run into an error in Latex, sometimes it's hard to locate directly what causes the error - Just delete part of your latex to narrow down the candidate location (but remember to put it in a copy).



