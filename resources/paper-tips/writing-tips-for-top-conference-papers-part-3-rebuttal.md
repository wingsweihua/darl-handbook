# Writing Tips for Top Conference Papers (Part 3): Rebuttal

When it comes to rebuttal, let's consider the following postulates:

* Postulate 1: The ultimate goal of rebuttal is to persuade the Associate Chair (AC), while convincing the reviewers is just one of the means to achieve it。
* Postulate 2: Reviewers' expertise varies, and some may lack the qualifications to judge the quality of your work accurately.
* Postulate 3: Despite the existence of reviewers who might lack domain knowledge (e.g., "what is softmax"), we still believe that, on average, reviewers have a sense of responsibility and fairness above societal norms.

Based on these postulates, I have summarized the following four strategies for rebuttal:



### Be truthful and avoid feigning humility.

Some individuals believe that the key to successful rebuttal is admitting one's mistakes to please the reviewers. However, I consider this approach not to be the most optimal strategy. Reviewers may make various incorrect judgments due to mismatched research directions, time constraints, or even personal moods. In such cases, when a reviewer's comments are mistaken, it is crucial to point out the errors rather than blindly agreeing with them.

When faced with inappropriate negative evaluations, some students might adopt a strategy of partially admitting the shortcomings and then providing various reasons to mitigate the negative impact. For instance, if a reviewer states that "there are no experimental results on the XXX dataset," and this dataset is actually optional, some students might apologize and say, "we apologize ..., but ... is still acceptable," then proceed to add those results and thank the reviewer for improving the paper.

However, I believe a better strategy is to present references to several influential papers that did not include the requested experiment. For example, authors can say, "You requested this experiment, and although it has limited significance, we have conducted it as you asked. Here are some representative papers with similar impact that also didn't perform this experiment." (Inner thoughts: "As a reviewer, saying something uninformed like this, perhaps it's time for some self-reflection? AC, take a look, I respect them, but aren't they more reliable than this reviewer?")

From a reviewer's perspective, I believe that a rebuttal for a paper worth accepting should contain expressions like "we beg to differ," rather than being full of apologies. When I see authors firmly defending their work, regardless of whether I agree with their views, I at least feel they deserve respect, and I am more inclined to read their rebuttal carefully.



### Stop futile arguments and identify slackers.

Stopping the debate and pointing out who is "slacking off" is sometimes necessary when dealing with unreasonable reviewers. These reviewers might be in a bad mood, not paying attention, or simply participating as a joke. When encountering highly ridiculous comments, it is best to stop arguing and refrain from explaining basic concepts like "what is softmax." Instead, directly inform the AC (Area Chair) through the "AC message," which is not visible to the reviewers, to identify the problematic reviewer and ultimately have their opinion excluded. Of course, if there is extra space in your rebuttal, you can still respond to them briefly since the behavior of such reviewers is unpredictable, and there's a chance they might even elevate your paper to acceptance (as seen in personal experience).

We must believe that the average competence level of ACs is higher than that of the reviewers they assign. Your AC might not even hold the reviewer's opinion in high regard. If you can provide evidence truthfully and objectively to demonstrate the reviewer's incompetence, the AC might be inclined to ignore their feedback during the discussion phase, as it would be a waste of their time to deal with such reviewers.

For example, the following excerpt is from a small report I once submitted to the AC as part of the review process. The specific content cannot be disclosed, so I'll provide a general outline:

> "We feel it necessary to bring to your attention that some of the comments from Reviewer X confuse us a lot. It seems that the reviews lack some common knowledge of the deep learning literature.

* Reviewer X brought up a peculiar term, XX, and asked us to explain its relation to YY. XX has left us baffled, as YY is something anyone familiar with the field would know, and we can't see how it relates to XX.
* Although we have repeatedly stated that we implemented AAA, Reviewer X claimed in the summary that we used BBB.
* Reviewer X pointed out that there are numerous language errors, yet failed to provide any specific examples. This violates guideline X, section Y of the review criteria."

When delivering such reports, it's important to keep in mind:

1. Focus on the issues, not the person. Disagree with the comments, not the reviewer, to maintain professionalism.
2. Ensure that all accusations against the reviewer are based on solid evidence and straightforward logic. The comments should be clearly absurd to warrant such reporting. ACs are busy, and expecting them to spend several minutes contemplating the factual accuracy of a specific comment when they are not yet familiar with the paper might be unrealistic.
3. Avoid making the AC feel like you're instructing them on what to do. Instead, suggest that the AC takes the quality issues of the reviews into consideration during their decision-making process, rather than explicitly asking them to exclude the reviewer's score.



### Employ creative arguments to trigger internal discussions.

Using strategic tactics to initiate internal discussions among the reviewers can be beneficial when dealing with conflicting feedback due to their different expertise and preferences. Reviewer A might praise the writing but find the novelty lacking, while Reviewer B might have the opposite opinion. In such cases, you can selectively quote from one reviewer to counter the negative judgment of another, with the precondition of being truthful and objective.

For instance, you could start your rebuttal by saying: "We are glad that the Reviewers appreciate the novelty (Reviewer X), writing (Reviewer Y), and impressive experimental results (Reviewer Z)…"

When addressing each reviewer's comments individually, employ language skills to avoid being too direct (e.g., "How come Reviewer Y can see the innovation in our work, but you can't?"). Instead, subtly incorporate the positive evaluations of other reviewers to imply your point. For example:

> "We would like to note that XXX distinguishes our method from YYY and ZZZ, which is appreciated by Reviewer Y and Z."

This approach serves two purposes: it encourages reviewers to reevaluate their judgments more openly, and it may spark discussions among them. If the AC perceives the ensuing discussion as lively and valuable, they might find it rewarding and gain new insights. As the catalyst for such discussions, your paper may leave a positive impression on the AC and the reviewers.





### Make specific commitments, not empty promises.

Exactly, when you plan to make revisions based on the reviewer's feedback, it's essential to convey your willingness to implement the changes effectively. The reviewers and the AC might be concerned about uncontrollable modifications that could exceed the page limit, remove essential content, or introduce new errors. To address these concerns, avoid making empty promises in your rebuttal:

> "We will conduct the experiments you suggested."
>
> "We will modify Figure 2."
>
> "We will rewrite the second chapter."

Instead, be highly specific in your responses:

> "We have conducted experiments XX and YY, and we will include the results in Table 1."
>
> "We will add the legend for XX to Figure 2, adjusting the font size and color accordingly."

In one of my previous papers, a reviewer pointed out that the logic in the entire third chapter (the section describing the methods) was confusing, and they got lost. They requested a rewrite. In response, I dedicated a significant portion of my rebuttal to describing how I would reorganize that section:

> "We understand that the initial part of the third chapter focused on background information, and we will move it to the 'Related Work' section."
>
> "We will add a comprehensive opening paragraph to the third chapter, summarizing the entire methodology and outlining its main components, which will provide clarity and guide readers to subsequent detailed subsections. This paragraph will be as follows..."
>
> "The subsequent subsections will individually describe..."



In conclusion, I hope that readers can avoid using these strategies as much as possible during the submission and rebuttal process. However, if they find themselves in such situations, I wish everyone the best of luck.
