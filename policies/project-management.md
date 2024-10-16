---
cover: >-
  https://www.shutterstock.com/image-photo/kanban-project-management-software-on-260nw-2129755877.jpg
coverY: 0
layout:
  cover:
    visible: true
    size: hero
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
---

# 🛠️ Project management

To understand the status of projects and figure out what needs to happen next, we use Trello. For scheduling events, we use Google Calendar. For data management, analysis, and writing we use a variety of software platforms.

## Calendars

As part of the onboarding process at The DaRL Lab, a lab manager will share a google calendar with you. It is your responsibility to keep this up to date to reflect your scheduled work hours.

## Data management

Our data, stim, videos, papers, and so on are our most valuable products! As such, we have a carefully designed system for ensuring that we never lose anything, while also making sure that each file we use is version-controlled and redundantly backed up.

All Music Lab files are stored in at least one of two places: on GitHub or Google Drive. These three locations are for three separate things, as follows:

Most of your day-to-day work will involve files on GitHub and Google Drive.

{% hint style="danger" %}
A word of warning: **most of GoogleDrive is editable**, even by new lab members. We trust you to be careful and ensure you don't delete things or check off items unintentionally.
{% endhint %}

### Version control and redundant backups

Every project has its own GitHub repository. This is where we store all of our files, **with two exceptions**: (1) large and/or high-security files, which live on personal google drive folders, and (2) Google Docs, which can't be git-controlled, and so they live on the shared Google Drive. All GitHub repos are managed via our GitHub Organization account ([http://github.com/themusiclab](http://github.com/themusiclab)). For example, the code for this Handbook is tracked at [http://github.com/themusiclab/handbook](http://github.com/themusiclab/TML\_handbook).

Project repos have a standardized directory structure, to keep things simple across scripts for different projects:

1. `admin` contains any administrative documents, like IRB-related material, flyers for recruitment, study protocols, etc.
2. `data` contains raw data.
3. `analysis` contains analysis scripts.
4. `results` contains processed data, that is, the results of analysis scripts.
5. `writing` contains all manuscripts, posters, etc.

Any projects that have large files, such as corpus projects with thousands of temp files, or tunning logs, should have a `.gitignore` file that prevents large files from uploading to GitHub; instead, these large files will only be stored on Google Drive.&#x20;

For the vast majority of projects that you'll be involved with, you will need to get comfortable with the basics of git: cloning repositories, making changes, and pushing your changes.

{% hint style="info" %}
If you've cloned one of our project repos and are having trouble pushing changes to master, most likely the issue is that your clone doesn't have an origin url set up properly. In Terminal, use `cd` to navigate to your local copy of the repo and then type `git remote set-url origin http://USER:PASSWORD@github.com/themusiclab/REPO.git`where `USER` and `PASSWORD` correspond to your GitHub credentials, and `REPO` is the name of the GitHub repository you're working in.
{% endhint %}

All lab computers are set up such that our local copies of project repositories will live in the path `~/git`. If this folder doesn't exist (i.e. you are on a non-lab machine), make this folder in your home directory to store all project related local repositories. More details on how to use git can be found easily online.

GitHub repositories that have large files (e.g., datasets over 100MB) require you to install `git lfs`. Ask a lab manager for help with this.

### Shared Google Drive

Google Documents have built-in version control, so they don't need to be stored in a git repo. Instead, **we store all Google Documents in our shared Google Drive, `darlshareddrive`**. This can get a bit confusing because often Google Documents are created on the fly by different people.

{% hint style="danger" %}
To ensure that we never lose access to a document we need, when you create a Google Doc (or sheet, form, etc), immediately move it to the `musiclabgdrive` Shared Google Drive. This will automatically enable access for everybody in the lab.
{% endhint %}

If you see a lab Google Document that is **not** in **`darlshareddrive`**, let a lab manager know so that we can fix it!

We also want to be sure that our lab-wide documents are not accessible to people outside the lab. For this reason, **please do not use link-based editing or viewing** in Google Docs. Instead, invite the specific people who need access to each document, and manage their permissions directly (usually giving commenting rights to everyone, so that they can type suggestions in the document, but not make direct edits).

### General data management principles

When you manage your personal files on your laptop or phone, you are the only person who needs to understand how they're organized, so it's no big deal if they are organized idiosyncratically.

In a scientific organization, we manage our files so that any new person on a project can immediately understand what they're looking at without needing to be instructed — but also so that if we go back to our files months, years, or decades after a project is complete, it will be obvious how they are organized.

Here are some simple principles for organizing files that you should \*always\* follow:

1. For projects that include human subjects run in lab, **use a** **single set of subject numbers** (usually `1000` thru `9999`), where the subject number is informative. For example, in IPL, subjects in the `1000`-`1999` range were pilot subjects, while subjects in the `8000` -`8999` range were in the final cohort.
2. Always **choose filenames that are intelligible** regardless of where they are stored (e.g., `/IPL/datadrop/IPL8006_codingBlink.csv`, not `/IPL/datadrop/coding/blink/8006.csv` — get the difference?)
3. Whenever possible, **don't create sub-subdirectories**. It's hard enough to remember what belongs in what folder for a single project, let alone multiple projects.
4. For in-lab human subjects projects, always **use an automatically-generated studylog**. We usually do this with a Google Form, which generates a log of all subjects run and organizes their details in a machine-readable csv. That file then becomes the starting point for all analyses. **All notes you take on participants should be part of the studylog**; otherwise, we risk losing them or doing analysis without knowing that they exist.

Remember, these apply to all files, whether they're stored on GitHub, `musiclabnas`, or `musiclabgdrive`.

## Analysis and writing

Because the process of scientific research is idiosyncratic and because your personal preferences may not be the same as those of Hua or your labmates, we do not dictate much in terms of lab-wide policies for how to handle data, do analyses, or write up projects — except for just a few things. This section lays out what **does** need to be the same across all projects.

Anything not covered here is up to the people leading a project. In general, before you decide to use a particular software package or implement a particular analysis, you should discuss it with Hua.

### Working diary

While you are not required to use any particular analysis package, you are required to log your working process and do your analyses in a reproducible fashion. This means that for every value that ends up in a research product, there needs to be a "research trail".  This would help you trace back, summarize, and retrospect your work easily. In general, this should be a commented analysis with screenshots and notes.&#x20;

Location: Google Drive - your individual directory created by the lab

Updated frequency: Daily

### Individual/Project meeting slides

With working diaries, you could easily prepare your slides for meetings, and meeting slides are required to share with Hua or involved group members. This should be one file for each semester of your work, with newer updates in the front.&#x20;

Location: Google Drive - your individual directory created by the lab

Updated frequency: Weekly before meeting for summary, and updated meeting summary after meeting

### Group meeting notes

Group meetings will be mainly paper sharing. See [Recurring activities](../resources/recurring-activities.md) for more detail.

Location: Google Drive - shared lab directory

Updated frequency: Weekly before meeting



### Writing

Like our approach to data analysis, we feel there is not any one "right way" to write a manuscript. That said, we often begin with a Google Doc so that we can jot down ideas and do unstructured collaborative editing all at once. Then, as the manuscript begins to take shape, we move to Markdown or Word and edit documents directly, one editor at a time, tracking changes via git.

If you're collaborating on a Word manuscript, preserve an intelligible filename, usually with the project name, the journal it will be submitted to, and the version number (e.g., `NHS_sci_2b.docx`). Append your initials to the filename after you've edited so that it's easy to tell who's version is whose (e.g., `NHS_sci_2b_sm.docx`).&#x20;

If you're working on a Markdown manuscript, then we generally won't change the filename as editing progresses, since GitHub will take care of comparing versions automatically so long as the filename stays the same. So you should just title the manuscript with the project name and the journal it will be submitted to (e.g., `IPL_nhb.md`).



## ~~Deprecated: Status (Trello)~~ now with Slack

~~We keep track of all our projects on Trello, a project management platform that basically is a bunch of nested lists. While Trello has a variety of features, including commenting and communication, **we only use it for management, not for communication**. This means that if you want to talk to someone about a card or checklist item, **always do so in Slack, not in the built-in commenting system.** This is a firm rule — just as email is redundant with Slack, so is communication in Trello.~~

~~Instead, we use Trello to keep track of the status of projects and shepherd them from the ideas stage thru experimental design, data collection, analysis, write-up, and publication. To facilitate discussion of events recorded on Trello (e.g., "a new checklist item was created for TML"), some Slack channels have Trello bots that automatically post updates, which can then be replied to in threads.~~

{% hint style="info" %}
~~The most important board on Trello is **darllab-status**. This is the overview board for all Music Lab projects: each card on the board represents a project, and has a master checklist of the big things happening next (like "draft the methods section of the paper!"). **darllab-status** is also the home of the ever-important **Who's Doing What** list (which hosts to-do lists for all lab members).~~
{% endhint %}

~~In general, there is no standardized way that we use Trello across different projects. This is intentional: different projects have vastly different project management needs.~~&#x20;

~~As you get involved in a project, you'll get the hang of what parts of that project's presence on Trello you need to pay attention to. At the very least, you'll need to use darllab-status to know what's happening next on your projects; however, in most cases, you'll use the full project board to organize your work.~~
