# Paper writing tips in DaRL Lab

TJ and Hua discussed specific writing revisions on their papers. Below are section-specific suggestions/guidelines.



## Rule of Thumb about figures and tables

Pictures and tables are the most critical components of an article and often the first things people look at. All tables, images, and their corresponding captions should ensure that readers can understand the conclusions by looking at them alone.&#x20;

1. The captions should describe what the figure is about:
   1. If this figure is about an example, explain where this example is about,  what can be observed, and what is the conclusion. &#x20;
   2. If this figure is about our method overview, explain the overall flow of this method, the texts in the figure should be easily found in the Method section.&#x20;
   3. If the figure/table is about experiment results, explain the goal of the experiment, the evaluation metrics (higher, the better? or lower the better?), and describe the observations.
2. **5 figures and 3 tables in the main body of your paper (visually pleasing to most reviewers in AI)**.&#x20;
   * The best results (sometimes top 2 results) in Tables should be highlighted.
   * Figure colors should be consistent and text in figures should be easily found in the main body of the paper.

## Section 1. Introduction&#x20;

Introduction is a longer version of the abstract, i.e. of the entire paper and it is the most creative part of your paper writing, it requires storytelling skills that might need years to develop. But if you don't know how to tell a story about your research, the following structure is a baseline:

1. What is the problem? \[What are we trying to do and why is it relevant?]
2. Why is it interesting and important?
3. Why is it hard? (e.g., why do naive approaches fail?) \[Can use example]
4. Why hasn't it been solved before? (Or, what's wrong with previous proposed solutions? How does mine differ?)
5. How do we solve it (i.e. our contribution!) -> which part corresponds to which challenge. What are the key components of my approach and results?&#x20;
6. How do we verify that we solved it (e.g. Experiments and results)
7. New trend: specifically list your contributions as bullet points
8. Extra space? Future work and any specific limitations.

## Section 2. Related Work/Preliminaries

This should correspond to your introduction, introduce related works solving the similar problem - and most importantly, your differences with their methods.&#x20;

Depending on your content, related work could be put in the later sections before the Conclusion.&#x20;

When should I put the Related work later?

* When explaining the differences, if you have mathematical definitions involved, it might be a good idea to have a **Preliminaries/Background** section instead of a text-mainly related work section.&#x20;

## Section 3. Method&#x20;

The Method Section should be written in a detailed way to explain the motivation and how you implement things. Below is a general structure of Method Section.

### Section 3.1 Overview.

Usually, it will begin with an overview picture/subsection, to tell the readers what will be introduced and how they are organized.

### Section 3.2 Subsection 1 \[subsection titles should be easily found in the overview and pictures]

1. The first paragraph of each subsection is an introductory paragraph, connecting the previous subsection to the following subsubsections. It should describe the motivation/target of this section and should be aligned with Introduction.
2. Each subsubsections should also start with motivation - "In order to XXX".

### Section 3.3 Subsection 2

### Section 3.X ....



## Section 4. Experiments

Experiment section is the easiest section for a beginner to write once you conducted your experiments. Below is a general structure of Experiments Section.

The first paragraph should describe your motivation for experiments and what research questions you would like to answer. For example:

> We conduct comprehensive experiments to validate our method's ability to decouple explanation robustness from classification robustness. Our evaluation addresses three key research questions:
>
> • RQ1: Does MD-UQ have better quantify uncertainties?&#x20;
>
> • RQ2: How do different ensemble methods and information from both dimensions help?
>
> • RQ3: Is MD-UQ robust to different settings?

### Section 4.1 Experimental Settings

Introduce the dataset, baseline methods, metrics, hyperparameters etc..

### Section 4.2 RQ1: \[Shortened phrases for the RQ1]

This is the subsection where you have tables and figures to show your results.&#x20;

1.  The first part: you should start by explaining why need to do this experiment or the goal of this experiment.

    1. If this is an experiment related to an ablation study, please use one sentence to state why we need to care about this change or this parameter, and how it might influence the results. You should link to our methods part.

    > Example: In this section, we use more experiments to prove the necessity of using information from both semantic and knowledge dimensions as well as using tensor decomposition.
2.  The second part:  you should write how we conduct the experiments, i.e. the setup for this experiment.

    > Example: We conduct experiments on CoQA and NQ\_open using llama2-7b and llama3.1 as the knowledge extracted models.
3.  The third part:  tell readers where they could find the results. Using my caption to identify the tables or figures.

    > Example: We show the results in Fig. 6.


4.  Describe your observation and conclusion by starting with 'We have the following observation:' and analyze the results from different aspects using bullet points if possible.&#x20;

    1. When writing the analysis of the results, you must first state the observation with terms people can find in the tables and figures.
    2. &#x20;Then have a conclusion that is linked to the goal of experiments/research questions.

    > Example: We have the following observations:
    >
    > * \[Observation:] Compared with all baseline methods, MD-UQ achieves the best performance overall. Especially when we consider AUROC. For AUARC, MD-UQ achieves the best performance for NQ\_Open while MD-UQ also achieves the comparable performance for CoQA in most scenarios.  \[Conclusion: ] These results demonstrate that MD-UQ has better quantify uncertainties overall.
    > * \[Observation: Among all datasets, MD-UQ achieves the highest performance improvement on NQ\_Open, which is the most difficult dataset among all datasets.] \[Conclusion: This indicates MD-UQ could perform even better when the task is harder, where uncertainty quantification is more important.]

### Section 4.2 RQ2: \[Shortened phrases for the RQ2]

### Section 4.3 RQ3: \[Shortened phrases for the RQ3]

### Section 4.4 More notable results/case studies you wanted to share



## Section 4. Conclusion

The conclusion should:

* Start with a shorter vision of part of the introduction that starts with one summary sentence on "How do we solve it (i.e. our contribution!)" and "How do we verify that we solved it (e.g. Experiments and results)"
* Discussion on limitations and future work.



<figure><img src="../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>
