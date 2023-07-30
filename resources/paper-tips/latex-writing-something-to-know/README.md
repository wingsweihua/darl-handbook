---
description: There are some small things you might need to know about writing with Latex
---

# Latex Writing: Something to know

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





Some small things you might neglect

* [ ] All parentheses/literature citations/cross-references should have a space before them, created using the "\~" symbol in latex. (所有的括号/文献引用/图表交叉引用前面都要有空格，在Latex里符号生成空格)
* [ ] The usage of quotation marks should be combined with \` (located to the left of the number 1 on the keyboard, shared with the tilde \~) and ' (apostrophe, located to the right of the letter L on the keyboard, shared with the double quotation marks "). Latex 中的引号使用要结合\`（键盘数字1左边的键盘符号，和～共用）和‘（单引号，键盘字母L右侧两个，和双引号“共用）
* [ ] Remember, in formal writing, "can't" cannot be abbreviated; it should be written as "cannot" without a space between "can" and "not".  (Can't不能缩写，要写成cannot)
* [ ] Pictures and tables are the most critical components of an article and often the first things people look at. Review all tables, images, and their corresponding captions to ensure readers can understand the conclusions by looking at them alone. Suggest including the conclusions in the titles of experimental results. (图片和表格是文章最重要的部分，是很多人第一眼先看的东西。检查所有的表格、图片和对应标题，是不是可以使读者单看图片、表格和标题就可以看到结论。建议实验结果的标题里写上结论)

