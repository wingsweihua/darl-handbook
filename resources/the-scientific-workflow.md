---
cover: >-
  https://png.pngtree.com/thumb_back/fw800/background/20240618/pngtree-rocky-river-fast-flow-of-water-long-exposure-image_15797801.jpg
coverY: 0
---

# 💡 The Scientific Workflow

This is a guide for carrying out research in my lab. Keep this workflow in mind when you are planning, conducting, analyzing, and interpreting scientific work. You may notice two themes that seem to run throughout the plan: documenting and sharing. That’s the take-home message: Document everything you do and share your work for feedback (with the group, your peers, the field, and the public). Not every project will follow this outline, but most will. &#x20;

## Theory & Reading&#x20;

The first step is theory development and understanding the relationship of our work to the relevant literature. You should keep up with developments in the field using Google Scholar alerts and its recommendations. I check every week and I recommend that you do as well. \


We want to test the assumptions of the theories in computer science, understand what they predict, test their limitations and contrast with alternative accounts. We’re going to design experiments that help understand the theory, the models, and make refinements and/or reject some aspects of our theorization.\


* Use Google Scholar to find updates that are important for your research.
* Save papers in Mendeley or other bib software and annotate as needed.
* Document your work in Google Docs.
* Share interesting papers and preprints in the relevant channel in Slack.

\
Hypotheses Generation
---------------------

Hypotheses are generated to test assumptions and aspects of the theory and to test predictions of other theories. The hypothesis is a formal statement of something that can be tested experimentally and these often arise from more general “research questions” which are often broad statements about what you are interested in or trying to discover. You might arrive at a research question or an idea while reading a paper, at a conference, while thinking about an observation you made, or by brainstorming in an informal group or lab meeting. Notice that all of these assume that you put in some time and effort to understand the theory and then allow some time to work over ideas in your mind, on paper, or in a computer simulation.

* Work on hypothesis generation in lab meetings, our advisory meetings, and on your own.
* Document your work in Google Docs (or your own notes on paper, OneNote or Evernote).
* Share insights in lab meetings and in the relevant channel in Slack.

## Design the study/experiment

Concurrent with hypothesis generation is [experimental design](https://opentextbc.ca/researchmethods/chapter/experimental-design/). We’re designing experiments to test hypotheses about category representation and category learning and/or the predictions of computational models. Avoid the temptation to put the cart before the horse and come up with experiments and studies that will produce an effect for its own sake. We want to test hypotheses generated from theories and also carry out exploratory work to help refine our theories. We don’t just want to generate effects.&#x20;

The design comes first and you need to consider the logic of your experiment, what you plan to manipulate, and what you want to measure. We also want to avoid the temptation to add in more measures than we need, just to see if there’s an effect. For example, do you need to add in 2-3 measures of working memory, mood, or some demographic information just to see if there’s an effect there? If it’s not fully justified, it may hurt more than help because you have non-theoretically driven measures to contend with. I’ve been guilty of this and it always comes back to haunt me.&#x20;

* Work on experiment generation in lab meetings, advisory meetings, on your own.
* Document your work and ideas in Google Docs or a note-taking app that you can share.&#x20;
* Test these experiment protocols often.
* Develop a script for research assistants who will be helping you carry out the study.
* Share insights in lab meetings and in the relevant channel in Slack.\


## Analysis Plan & Ethics Protocol

This is where we start to formalize things. An analysis plan will link together the hypothesis and the experimental design with the dependent variables and/outcome measures. In this plan, we’ll describe and document how the data will be collected, visualized, analyzed, stored and shared. This plan should describe how we will deal with outlier data, missing data, data from participants who did not complete the experiment correctly, experimenter error, malfunction, etc. This plan can include tentative predictions derived from a model and also a justification of how we intend to analyze and interpret the data. This plan can (and probably should) be pre-registered with [Papers with Code](https://paperswithcode.com/), which is where we’ll plan to share the data we collect with the scientific community. \


The analysis plan should describe exactly what we are doing and why and should provide enough information that someone else would be able to reproduce our experiments in their own lab. These will also provide an outline for your eventual method section (ethics protocol) and your results section (analysis plan)

* Document your analysis plan and ethics protocol work in Google Docs.&#x20;
* Link these documents to the project sheet for your project.
* Share in the relevant channel in Slack.

## Collect data (or obtain data from other sources)

Once the experiment is designed, the stimuli have been examined, we’re ready to collect data or to obtain data from a third party (which might be appropriate for model testing). Before you run your first subject, however, there are some things to consider. Take some time to run yourself through every condition several times and ask a lab maket to do the same. You can use this to make sure things are working exactly as you intend, to make sure the data are being saved on the computer, and to make sure the experiment takes as long as planned.&#x20;

When you are ready to collect data for your experiment:&#x20;

* Meet with all of your research volunteers to go over the procedure.&#x20;
* Book the experiment rooms on the Google Calendar.&#x20;
* Reserve a laptop or laptops on the Google Calendar.

While you are running your experiment:

* Document the study in Google Docs and/or Slack
* Make sure the raw data are labelled consistently and never altered.
* Be sure to follow the data storage procedures outlined in the ethics protocol.

## Data Management

Your data plan should specify where and how to store your data. While you are collecting data you should be working on a script in R (or Python) to extract and summarize the raw data according to your plan. When you reach the planned sample size, ensure that all of that data are secure and backed up and do an initial summary with your R script.&#x20;

As you work on summarizing and managing your data:

* Make notes in the project sheet about where the data are stored
* Document your steps in your working diary or a [Python Notebook](https://jupyter.org/).&#x20;

## Plots & Stats

This is the best part of science: seeing your data visualized for the first time. When you have completed your experiment and taken care of the data storage and basic processing, it’s time to have fun and see what you discovered. The analysis plan is your guide and your analysis plan describes how you want to analyze the data, what your dependent variables are, and how to conduct statistical tests with your data to test the hypothesis. But before you do any statistics, work on visualizing the data. Use your Python notebook to document everything and generate boxplots, scatter plots, or violin plots to see the means, medians, and distribution for the data.&#x20;

Because you are using Notebooks to do the analysis, you can write detailed descriptions of how you created the plot, what the plot is showing, and how we should interpret the plot.&#x20;

If you are fitting a model to your data, make sure you have the code for the model. Use Git to do version control with comments wisely. Make sure that you develop the version for your experiment and that the generic model is not modified.&#x20;

## Present and explain each iteration

While you are working on your analysis, you should present the work often in lab meetings for the rest of the group and we can discuss the work when we meet individually. The reason to present and discuss often is to keep the ideas and work fresh in your mind by reviewing manageable pieces of it often. If you try to do too much at once, you may miss something or forget to document a step. Go over your work, make sure it's documented, and then work on the new analyses, and repeat. You should be familiar with your data and your analysis so that you can explain it to yourself, to me, to your peers, and eventually anyone who reads your paper.\


Use the following guidelines for developing:&#x20;

* Make your best plots and figures.
* Be able to present these to the lab on a regular basis.&#x20;
* Use slides to share summary work instantly.
* Keep improving the analysis after each iteration.
* You should always have 8-10 slides that you can present to the group.
* Document your work in Python Notebooks, Google Docs, and Google Slides.

## Write papers around this flow

The final step is to write a paper that describes your research question, your experimental design, your analysis and your interpretation of what the analysis is. A scientific paper, in my opinion has two important features: \


1. The paper should be clear and complete. That means it describes exactly what you wanted to find out, how and why you designed your experiment, how you collected your data, how you analyzed your data, what you discovered, and what that means.  Clear and complete also means that it can be used by you or by others to reproduce your experiments.
2. The paper should be interesting. A scientific paper should be interesting to read. It needs to connect to a testable theory, some problem in the literature, an unexplained observation. It is just as long as it needs to be. \


I think the best way to generate a good paper is to make good figures. Try to tell the story of your theory, experiment, and results with figures. The paper is really just writing how you made the figues. You might have a theory or model that you can use a figure to explain. You can create clear figures for the experimental design, the task, and the stimuli. Your data figures, that you made according to your analysis plan, will frame the results section and a lot of what you write is telling the reader what they show, how you made them, and what they mean. A scientific paper is writing a narrative for your figures.

Good writing requires good thinking and good planning. But if you’ve been working on your experiment according to this plan, you’ve already done a lot of the thinking and planning work that you need to do to write things. You’ve already made notes about the literature and prior work for your introduction. You have notes from your experimental design phase to frame the experiment. You have an ethics protocol for your methods section and an analysis plan for your results. You’ll need to write the discussion section after you understand the results, but if you’ve been presenting your 8-10 slides in a lab meeting and talking about them you will have some good ideas and the writing should flow. Finally, if you’ve been keeping track of the papers in Mendeley, your reference section should be easy.

## Submit the paper

The final paper may have several experiments, each around the theme set out in the introduction. It’s a record of what we did, why we did it, and how. The peer reviewed journal article is the final stage, but before we submit the paper we have a few other steps to ensure that our work roughly conforms to the principles of[ Open Science](https://jpminda.com/2018/07/12/open-science-my-list-of-best-practices/), each of which should be straightforward if we’ve followed this plan.

* Create a publication-quality preprint. We’ll host this on [ArXiv](https://arxiv.org/) (unless submitting a blind ms.) &#x20;
* Create a file for all the stimuli or materials that we used and upload it to Github and link to [Papers with Code](https://paperswithcode.com/).&#x20;
* Create a data archive with all the raw, de-identified data and upload it to Github and link to  [Papers with Code](https://paperswithcode.com/).
* Upload a clean version of your Python Notebook that describes your analyses and upload it to Github and link to  [Papers with Code](https://paperswithcode.com/).

\
\
