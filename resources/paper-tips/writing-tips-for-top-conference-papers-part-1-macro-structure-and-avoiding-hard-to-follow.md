# Writing Tips for Top Conference Papers (Part 1): Macro Structure and Avoiding 'Hard to Follow',"

This is a translation from [a blog in Chinese](https://zhuanlan.zhihu.com/p/593195527).

Over the past few years, I have been the lead author or made significant revisions to about 20 top conference papers. At first, I worked on these papers in the lab at Tsinghua University, struggling through numerous rejections before making progress. Eventually, during internships and work experiences, I found myself helping junior colleagues and interns improve their writing by addressing common issues. I want to summarize some advice for new writers of top conference papers. If my suggestions can help others avoid common mistakes, I will consider it an honor.

I will divide this advice into two parts, each focusing on avoiding a common pitfall that can lead to a fatal "reject" decision:

(1) This paper is hard to follow (macro-level, organization, optimizing structure, conveying core contributions).

(2) The readability can be greatly improved (micro-level, fine-tuning, avoiding common mistakes).

In this article, I will address the first pitfall - "hard to follow." Inexperienced writers who receive this type of feedback, combined with a "strong reject," can feel confused and frustrated. Therefore, I will begin by analyzing why reviewers may provide this feedback, and then offer two examples of how to improve your writing accordingly.

&#x20;

### The perspective of a reviewer

From the perspective of a reviewer, this feedback may indicate that there is a significant gap between the macro organization and content distribution of the paper and what the reviewer expected, which resulted in the reviewer being unable to understand what the author has done before running out of patience. What is the difference between what the reviewer thinks and what the author thinks about the same paper?

A student may be very satisfied with their just-completed paper because:

* During the study of an important problem, I encountered several complex sub-problems. I solved these problems one by one and ultimately obtained a clever solution. I recorded this wonderful process, and the reviewer should be convinced of the systematic and self-consistent nature of this solution.
* The problem I discussed may be a bit difficult to understand, but once you get past that hurdle and go through a series of thought-provoking games, you can transform the problem into another simple one, and the solution will come naturally. I used two pages to expound on this reasoning, gradually deriving the final conclusion, and the reviewer will certainly be inspired by it.
* I added essential innovation to someone else's work, turning it into something completely new, with excellent results, a true SOTA. As long as the reviewer can understand the experimental results, they should accept my paper.

How does the reviewer view this? **The reviewer simply does not care.**

The reviewer opens your paper and thinks to themselves:

* What problem is the author trying to solve? Why are there so many problems? Which one is the one they are trying to solve? Which method is common practice and which one did they propose?
* What is written on these two pages? There is no summary at the beginning or end, and in the middle, there are assumptions and inferences. What is the conclusion? It seems obvious. Why did they write two pages about it?
* Oh, I understand this. It's yet another AAA + BBB. I'll skip the middle four pages and just look at the results. What does this indicator in the table mean? It's only 0.2 higher than someone else's. Is that a significant difference?

What does the reviewer expect?

* The reviewer wants to quickly understand what new thing you have proposed, rather than listen to you explain in detail and follow along with you as you gradually discover the answer. The purpose of writing a paper is to introduce the final form of the work to the reader, not to document the research process. Some students may describe their journey from initial idea to final result in their paper, but this is usually irrelevant.
* The reviewer will not read the paper word for word. They want to be able to quickly find what they are looking for on any page, in a format that they are used to. Therefore, if the organization of your paper is not conventional, the reviewer may not bother to read it at all.
* Many reviewers are looking to learn something new. If you present some counterintuitive, interesting, or practical conclusions in an obvious place, they may find it rewarding. However, do not expect every reviewer to be willing to spend time deciphering your lengthy text or deciphering unclear charts to come to these conclusions themselves.

#### **Example 1: Don't fully restore the research process**

In order to solve an important known problem (problem A), I proposed solution A (which is significantly different from other methods), but found that it was not good enough. I investigated why, and discovered that solution A introduced another problem (problem B). I then studied how to solve problem B, and finally proposed an improved version of solution B (which only involved a small change, a trick). All problems were solved, and the trick also improved other methods. I proposed two solutions and also discovered a problem that others hadn't noticed. I think this paper is solid.

However, the reviewer is looking at this paper from a different perspective. They did not experience my research process firsthand, so they may not be able to see the main points as clearly as I do. They may ask:

* How do you prove that the fundamental reason why solution A is not effective is problem B?
* Solution A also has some effect, how do you prove that it is because problem A is solved?
* The difference between solution B and solution A is very small, so where is the novelty?
* You said that the improvement of solution B can also be applied to other methods, so why do we need solution A? Isn't solution A not better than other methods?

I feel very wronged: the final result of this paper is obviously solution B, which is an ingenious upgraded version of solution A. The difference is naturally small. But solution A was also proposed by me! Also, why are you so concerned about the relationship between solution A and problem A? Is it really that important?

If the reviewer could hear my complaints, they would say:

* You have been promoting solution B throughout the entire paper, and have not emphasized solution A. How do I know that it is also a major part of this paper?
* Even if solution A was proposed by you, it did not solve problem B, which you emphasized. Does it still count as a major contribution?
* Since solution A is not a major contribution, isn't the improvement you emphasized for solution B only a small change?

Arguing about the review comments is meaningless, and we can only try to avoid triggering such pointless debates when writing. If we change our writing approach slightly, the reviewers will find it easier to understand our work:

* I propose a novel method to solve an important problem.
* This method consists of a new framework and a general trick.
* Demonstrate the effectiveness of both: using the framework without the trick results in relatively worse performance due to an interesting problem (analysis provided); the trick can also improve other methods to some extent; the combination of both achieves the best performance.

Why do reviewers prefer this organizational structure? Because they can quickly see what we propose and what their respective roles are. They only need to judge the technical correctness and the significance of the proposed work.

#### Example 2: Avoid Using "Based on" and "A+B" Lightly

The phrase "based on AAA and BBB" is a common expression used in undergraduate thesis writing and is suitable for situations that require caution and safety but not much innovation. However, using this phrase in top conference papers may undermine the originality of your work. In most cases, it's best to avoid claiming that your work is "based on." Instead, you can state that you noticed an important problem, understood the underlying principles, came up with a solution, and proposed something new that naturally incorporates AAA and BBB. It's important to highlight that you didn't just modify someone else's work.

Imagine if the ResNet paper were written using the "based on" and "A+B" format, it would have undermined the innovation of the work.

"ResNet: Yet Another Simplified GoogLeNet" - We designed a model based on GoogLeNet and VGGNet that employs a large number of 3x3 convolutions (inspired by VGGNet) and parallel shortcuts (simplified from GoogleNet), surpassing both GoogLeNet and VGGNet. Why is the performance so good? Because VGGNet and GoogLeNet are brilliant, and Batch Norm is also very useful. We didn't think there was any theoretical innovation in this work, but we've provided a good baseline for future work.

**How much can readers learn from such articles?**

So how was ResNet actually written?

* As you all know, there is an important problem today: the deeper the model, the more it drops in accuracy.
* Our solution is surprisingly simple: we change the mapping form in the model from y = f(x) to y = f(x) + x, which is called "residual learning," and can solve this problem. This is because the model is easy to fit f(x) = 0, but not f(x) = x. Residual learning is easy to implement and very effective.

Identifying the problem, abstracting the underlying principles, proposing one's own solution and its specific implementation, and validating with experiments, this is a writing style that is more in line with human cognitive rules.

Some students feel that writing a paper with less contribution in this way is just "telling a story," but as long as it is truthful and the experimental evidence can support your story, this kind of story is not only beneficial for reviewers to give you high scores, but also for readers to learn new knowledge and for the dissemination of your views. It is a win-win situation.

### Summary and Other Suggestions

* The first point discussed above is actually related to ResNet: the real history of ResNet comes from the deconstruction of GoogLeNet, and ResNet was not developed by suddenly discovering the principle of "residual learning," but by Sun Jian's team thinking about the explanation after discovering that the shortcut structure of GoogLeNet is useful. The "poor version" writing style we imagined, while reflecting the real research process, is not conducive to digging deeper into the underlying principles and spreading the core ideas. This example just supports the point of this article: how to do research and how to write a paper are two different things.
* A paper is a tool for disseminating knowledge, a standardized way of communication that makes it easy for others to learn new things with time and effort saved. It is not a stage for personal expression. Reviewers (readers) are accustomed to reading what kind of papers, so we write what kind of papers. This is essentially the same as popular songs and popular novels - just trying to cater to the audience, nothing more.
* There is no need to seek innovation in the structure of the article. Most articles can be written in the form of Introduction + Related Work + Method + Experiment + Conclusion. If what you propose is not a single innovation point but a combination of small changes, you can learn how ShuffleNet v2 is written.
* Be explicit. What you don't emphasize, don't expect others to figure it out themselves.
* Describe what you propose in one place, don't scatter it around. Don't assume that a reader will have the patience to read 50% of the paper before understanding what you have done.
