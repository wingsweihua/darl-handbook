# Latex de facto

### In the main text

* [ ] All parentheses/literature citations/cross-references should have a space before them, created using the "\~" symbol in latex. (所有的括号/文献引用/图表交叉引用前面都要有空格，在Latex里符号生成空格)
  * [ ] Using `~` instead of a regular space can prevent awkward line breaks when cross-referencing or mentioning people's names. For example, "as shown in Fig.\~\ref{Fig1}" or "as A.\~Einstein said..."
* [ ] Avoid placing numbers at the beginning of a line.&#x20;
  * [ ] Using `~` instead of a regular space to avoid
* [ ] The usage of quotation marks should be combined with `` ` `` (located to the left of the number `1` on the keyboard, shared with the tilde `~`) and `'` (apostrophe, located to the right of the letter `L` on the keyboard, shared with the double quotation marks `"`). Latex 中的引号使用要结合\`（键盘数字1左边的键盘符号，和～共用）和‘（单引号，键盘字母L右侧两个，和双引号“共用）
* [ ] Remember, in formal writing, "can't" cannot be abbreviated; it should be written as "cannot" without a space between "can" and "not".  (Can't不能缩写，要写成cannot)
* [ ] Pictures and tables are the most critical components of an article and often the first things people look at. Review all tables, images, and their corresponding captions to ensure readers can understand the conclusions by looking at them alone. Suggest including the conclusions in the titles of experimental results. (图片和表格是文章最重要的部分，是很多人第一眼先看的东西。检查所有的表格、图片和对应标题，是不是可以使读者单看图片、表格和标题就可以看到结论。建议实验结果的标题里写上结论)
*   [ ] When inserting URLs into the main text, use `\url`

    ```latex
    \usepackage{hyperref}
    \url{http://stackoverflow.com/}
    ```

    * [ ] Make sure to escape characters that have special meaning: `# $ % & ~ _ ^ \ { }`
      *   [ ] So `http://stack_overflow.com/~foo%20bar#link` would

          be `http://stack\_overflow.com/\~foo\%20bar\#link`



### About common abbreviations

If you are not sure about it, then don't use it.

<table><thead><tr><th width="106.33333333333331"></th><th width="189"></th><th width="330"></th><th></th></tr></thead><tbody><tr><td>et al.</td><td><p></p><p>et al. is commonly used as an abbreviation when citing scholars' work or referencing sources in a paper. It is used to abbreviate a list of authors.</p></td><td><p>Do not add a period after et because it is not an abbreviation.</p><p></p><p>Add a period after al because it is an abbreviation.</p><p></p><p>If et al. appears at the end of a sentence, there is no need to repeat the period.</p><p></p><p>If followed by question marks, exclamation marks, or other punctuation, add a period after et al.</p><p></p><p>Do not use a comma before et al.</p></td><td>These results agree with the ones published by Pelon et al.</td></tr><tr><td>etc.</td><td>Generally, it is placed at the end of a list to indicate that the examples mentioned earlier are not exhaustive. </td><td><p>Use a comma before etc.</p><p></p><p>Similarly, if etc. appears at the end of a sentence, do not add an additional period.</p><p></p><p>Use "et al." in the context of people, and "etc." in the context of inanimate things or non-living entities.</p></td><td> I need to go to the store and buy some pie, milk, cheese, etc.</td></tr><tr><td>e.g.</td><td>It can be used in place of expressions like "for example," "for instance," or "such as." </td><td><p>Both e and g should have periods after them. A common mistake is forgetting the period after e.</p><p></p><p>It is best to place e.g. along with its example inside parentheses, such as: I like quiet activities (e.g., reading).</p><p></p><p>Avoid using etc. after e.g. in a list. </p><p></p><p>It is not recommended to use etc. after "including" in a list. This is because e.g. already implies a few examples, and adding etc. would be redundant.</p></td><td>Buy some vegetables, e.g., carrots.  </td></tr><tr><td>i.e.</td><td>It is used to provide further clarification or explanation of something that has been mentioned before.</td><td><p>The first period in i.e. is often overlooked.</p><p></p><p>There should be a comma after i.e.</p><p></p><p><del>Similar to e.g., it is best to place i.e. inside parentheses for clarity.</del> </p></td><td>There are three meals in the day, i.e., breakfast, lunch, and dinner.</td></tr></tbody></table>

### About math equations

* [ ] Mathematical formulas are a form of text. All punctuation rules applicable to regular text also apply to mathematical formulas.
* [ ] For numbers that cannot be expressed in one word and without mathematical significance, consider using words like "one," "two," or "three" instead.
* [ ] Use the math environment for numbers, even if it's just a 1 or 0. Whenever a number is involved, it's best to use the math environment. If you fail to follow this convention, mistakes like using "-" instead of a minus sign might occur.&#x20;
* [ ] For special mathematical functions like sin, cos, log, and exp, use \sin, \cos, \log, and \exp, respectively, to get the appropriate spacing and upright format.&#x20;
* [ ] Some inner product symbols in mathematics, as well as the bra-ket notation in quantum mechanics, are represented using \langle and \rangle, not the less than (<) and greater than (>) symbols.

| Yes                                                                                                                                                                                                | No                                                                                                                                                                                                                                     |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p>Now that we know </p><p><span class="math">A=B</span></p><p>and</p><p><span class="math">B=C</span>, </p><p>we can conclude that</p><p><span class="math">A=C</span></p><p>This is obvious.</p> | <p>Now that we know </p><p><span class="math">A=B</span></p><p>and</p><p><span class="math">B=C</span> <strong>(missing comma here)</strong></p><p>we can conclude that</p><p><span class="math">A=C</span></p><p>This is obvious.</p> |
| four datasets                                                                                                                                                                                      | 4 datasets or $$4$$ datasets                                                                                                                                                                                                           |
| $$21$$baseslines                                                                                                                                                                                   | Twenty-one baselines, 21 baselines                                                                                                                                                                                                     |
| it is $-1$  or it is $$-1$$                                                                                                                                                                        | it is -1                                                                                                                                                                                                                               |
| \sin $$\sin$$                                                                                                                                                                                      | sin $$sin$$                                                                                                                                                                                                                            |
| \exp $$\exp$$                                                                                                                                                                                      | exp $$exp$$                                                                                                                                                                                                                            |
| \argmax $$\argmax$$                                                                                                                                                                                | argmax $$argmax$$                                                                                                                                                                                                                      |
| \langle s,a, r,s' \rangle $$\langle s,a, r,s' \rangle$$                                                                                                                                            | $$<s,a, r,s' >$$                                                                                                                                                                                                                       |



### About Bibliography

* [ ] You could shorten your bibliography to shorten the total pages in a manuscript for submission, but you need to put full citations in camera ready.
* [ ] Use citations with published conferences/journals as references other than Arxiv when possible.
* [ ] After compiling, always check the reference list. Do not fully trust downloaded bib entries from the internet (google scholar or Mendeley). Sometimes they provide the wrong format for some European names and subtitles.
