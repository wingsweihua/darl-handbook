# Writing Tips for Top Conference Papers (Part 2): Refining to enhance "readability"



This is a translation from [a blog in Chinese](https://zhuanlan.zhihu.com/p/639732057).

In "[Writing Tips for Top Conference Papers (Part 1): Macro Structure and Avoiding 'Hard to Follow'"](https://app.gitbook.com/o/Ibg8yymG2pI4tEIIo6eY/s/Yupq30GiLbkqhpxAt5B1/\~/changes/1/resources/paper-tips/writing-tips-for-top-conference-papers-part-1-macro-structure-and-avoiding-hard-to-follow), we discussed how to design the overall structure of a paper at a macro level to present one's core contributions in a way that is appealing to most readers.

In this part, we will focus on the level of language organization and provide practical advice and techniques to enhance the readability of the article. The goal is to allow readers to smoothly and effortlessly read through the paper and enable reviewers to objectively and painlessly evaluate the paper's value.

It should be noted that our discussions assume that the paper is grammatically correct, and we won't address basic issues that can be automatically handled by tools like Grammarly or ChatGPT.

As mentioned in the previous part, most papers can be written in the format of presenting a problem, abstracting the underlying principles, and proposing a solution (commonly known as storytelling). This part's macro structure will also follow this approach and serve as a specific implementation of the macro writing principles discussed in the previous part.

Assuming this article is indeed a paper, let's skip the clichéd phrases about the importance of writing and how writing has become an important research field. Also, let's skip the long list of references to prior work on writing (the author might not have even read them, but they're cited because others did). With that said, our story now begins.

In this article, we propose using the following concepts to measure the readability of a paper: **logical coherence, defensive resilience, confusion time, and information density**. Based on these concepts, we provide practical advice and techniques to improve the readability of articles.

### :jigsaw: Logical Coherence&#x20;

In any academic writing, logical coherence is far more important than using fancy words. In the previous part, we introduced some macro-level techniques for logical design. At the micro-level, it's essential to remember that logical coherence lies in the logic itself, not in transitional words (e.g., "to this end," "in contrast," "specifically," etc.).

In other words, **transitional words should be used to embellish the language and make it more fluent, not to forcefully construct logic for sentences lacking it**. For example, when moving from general to specific descriptions, use "Specifically, …"; when there is a contrast between two sentences, use "In contrast, …".

However, it's important not to do the reverse! Just using "In contrast" doesn't automatically create a contrasting relationship between the two sentences. The mismatch between transitional words and real logic can confuse readers and significantly reduce the paper's readability.

_**For every transitional word used, consider: Does it reflect a real logical relationship between the preceding and following sentences? Is it contextually correct? Could we do without it?**_

#### Example 1: Transitional words must be contextually correct and withstand scrutiny.

> "We argue that problem A is critical. To this end, we propose method B."&#x20;

The author might have intended to use a transitional word to introduce method B after mentioning problem A, but the context isn't clear. The phrase "to this end" refers to what "end"? Was there any previous mention of an "end" (i.e., what should be done or achieved)? The previous text only presents a viewpoint without stating any actions, so the transitional word's presence is incorrect.

#### Example 2: Transitional words should not impose logical relationships.

> "The system comprises three modules. First of all, Module A is.... Second, Module B is.... Last but not least, Module C is...."&#x20;

The author's intention might be to describe three parallel modules, but the transitional words impose a specific order on them. Instead, consider splitting the sentences and introducing each module separately: "The system comprises three modules: Module A..., Module B..., Module C...."

#### Example 3: Transitional words should accurately reflect real logical relationships.

> "The baseline model is… On top of that, model A employs an extra attention module. In contrast, we propose a novel objective function."&#x20;

The sentence in question is confusing as it leaves room for two different interpretations regarding whether our model uses the "extra attention module" along with the "novel objective function."

To address this ambiguity, if a comparison is necessary (for example, when dealing with a reviewer who may not fully understand but insists on a comparison), we should discuss the comparison separately from both the structural and loss perspectives to eliminate any misunderstandings and highlight our advantages:

> From a structural perspective, model A introduces an extra attention module, while we maintain the same model structure as the baseline. Regarding the objective function, method A adopts the vanilla XXX loss, which suffers from ..., whereas our model incorporates the new proposed objective function, resulting in ...

This approach ensures a clear logical flow, indicating that we intend to compare the two models from two different aspects, and avoids relying solely on transitional phrases like "In contrast" to establish the comparison, which could lead to misunderstandings.



### :shell: Defensive Resilience&#x20;

When writing, **we must anticipate potential challenges from reviewers and defend our statements accordingly**. "Defensive resilience" refers to the frequency of doubts raised by reviewers and the ability to resist scrutiny.

Just as we practice "defensive programming" when coding, we should adopt "defensive writing" and consider potential weaknesses in our statements.

#### Example 4: Providing solid evidence.

When stating, "Problem A is a critical issue in the field and remains unsolved," anticipate questions such as, "Why is it considered critical? What are the consequences, and how significant is the impact on performance?" Provide supporting evidence:

> "It is reported that problem A results in... \[1, 2, 3] and... \[4, 5], which are critical to... because... \[6, 7, 8]."

Rich and appropriate citations can create the illusion of the author's extensive knowledge and deep understanding of the field, even if they have only read the abstracts of those articles.

#### Example 5: Balance of explanations.

After presenting experimental results, we often need to explain why our method works. Over-asserting without direct evidence may invite challenges like, "How can you prove that? Is there any theoretical basis?" Balance the explanations:

* We observe an improvement in performance, attributed to XXX's ability to... (present direct evidence).
* If we don't have direct evidence, but some visualizations or indirect evidence, we can say, 'The performance improves, which may be explained by XXX's ability to... (present indirect evidence).'
* If we only have a feeling that our method should work, but it aligns with our motivation, we can say, 'The performance improves, suggesting that XXX can... (mention the motivation).'

#### Example 6: Avoid using self-defeating subjective vocabulary.

> In Table 1, it is obviously exhibited that …

In academic writing, using subjective words like "obviously" has no benefit. If the readers can recognize the results are good, there's no need to emphasize it with "obviously." If the readers can't understand, emphasizing will lead to even more confusion. So, avoid using words like "obviously" that may lead to more questions: "Where exactly is it good? Let me scrutinize it carefully, and, by the way, I might label it as an overclaim. How will you deal with that?"

### :confused: Confusion Time&#x20;

"Confusion time" refers to the time readers spend going from "What is this?" to "Oh, now I get it" while reading the paper. People's patience is limited, and the shorter the total confusion time of a paper, the higher its readability, and the reviewers will be more at ease.

#### Example 7: Immediate explanations after introducing a concept.

In the field of deep learning, a simple structure in a complex model may be named as XXX Perceiver, XXX Perceptron, XXX Recognizer, XXX Gating Function, etc., based on its function (and storytelling needs).

It is advisable to explain the essence immediately after introducing the name (e.g., "We propose XXX, implemented with a two-layer MLP"). Otherwise, readers will be left with confusion about what this "mysterious" concept is, leading to a negative reading experience.

#### Example 8: Clearly and unambiguously referential objects.

> "We update structure A to solve the problem caused by model B, which is widely used in the literature."&#x20;

Is "widely used" referring to A or B? If the sentence's structure doesn't allow for unambiguous reference, consider splitting it into shorter sentences. There's no need to showcase complex sentences to prove English proficiency; clear communication is more important than showcasing intricate language.

#### Example 9: Avoid multiple references to content several pages away.

While it's reasonable to mention the paper's results in the introduction and add some references to the figures or tables for context, it's not ideal to do this frequently, especially when it requires readers' focused attention (e.g., while passionately presenting your core story for them to judge its validity). During the time it takes for readers to find the referenced content, their train of thought may be interrupted, affecting their overall comprehension. Remember that a paper is a linear narrative, and maintaining readers' cognitive continuity is essential.



### :ocean:Information Density&#x20;

Information density is not a new concept; it refers to the amount of relevant information that readers can extract from a unit length of text. Articles with low information density may cause readers to lose focus and doubt the author's expertise.

#### Example 10: Avoid Lengthy Filler Phrases

We all know that every paper contains sentences that no one will seriously read, often found at the beginning of each chapter, with a high proportion of phrases like "in recent years." While these sentences might still be necessary, here are some suggestions:

* Keep them concise; if they are too long, no one will read them. Once, I reviewed a paper on model compression, and the introduction went on from LeNet to ViT until halfway through the second page before defining "model compression."
* Avoid irrelevant content. If your paper is about ViT and does not involve low-level operations, there's no need to mention how convolutional networks use sliding windows.
* Avoid writing a history book. After reviewing so many papers, I now suffer from PTSD when thinking about the history from the discovery of animal visual cortex principles to LeNet, AlexNet, and ResNet.
* Stay relevant to the main topic and quickly move on to the main content. For example, if you propose a new hierarchical ViT, you can divide ViTs into two categories based on their hierarchical nature in the first sentence of the main text (recently, ViTs have flourished, including two types…), and then proceed to the main points in the second sentence.

#### Example 11: Use Concise Language

Non-native English speakers often write less concisely than native speakers, and beginners may write longer texts because they fear imprecise language. For instance:

> "The image classification performance on ImageNet is 79.99%."&#x20;
>
> Change to: "The ImageNet top-1 accuracy is 79.99%."

> "As can be observed in Table 1, A outperforms B."&#x20;
>
> Change to: "Table 1 shows that A outperforms B."

> "Table 1 shows that the accuracy of model A is 81.0% and the accuracy of model B is 80.0%, so we conclude that model A outperforms model B."&#x20;
>
> Change to: "Table 1 shows that model A outperforms model B by 1.0% in accuracy (81.0% v.s. 80.0%)."

Using concise language to express ideas accurately is a challenging skill. It is advisable to read papers and other texts written by native English speakers, especially those written by young experts with rich teaching experience (e.g., Andrej Karpathy, who taught Stanford's CS231N).

#### Example 12: Increase Information Density Around Figures and Tables

* If abbreviations are used in figures or tables, it's best to explain them in the corresponding titles.&#x20;
* If you want to emphasize a particular result in Table 5, the sentences analyzing that result should be placed on the same page as Table 5, and it's helpful to include "Table 5" in those sentences. This is because readers may not read your text carefully but may directly look at the figures and tables and then search for related text using the PDF reader's search function. When they see an impressive result in Table 5 and become curious, they will likely search for "Table 5."&#x20;
* Do not expect readers to figure out the necessary comparisons from complex tables on their own. We should present the content that needs comparison together. If designing such tables is challenging, it's acceptable to repeat certain results (typically a baseline that needs to be compared with several other results) a few times. No one will reject your paper because of less elegant table design, but if readers can't understand the table and their blood pressure rises, it's a real issue for reviewers.
