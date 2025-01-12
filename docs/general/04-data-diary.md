---
title: Replication and the data diary
parent: General topics
nav_order: 6
---

<!-- Add Irena's documentation for the wildfire story. -->

# The data diary
{: .no_toc}


At the Associated Press, data reporters issue a simple command when beginning a project, which sets up a standardized set of files and folders. From there, reporters' work is centrally stored and documented in standard locations, making it easy for any one on the team to dip in and out of the project.

All of the unit's work, including its story memos, are done using standardized tools that allow for replication at any point in the project and ensure that any communication with all members of the reporting and graphics teams are looking at the same, up-to-date results.

"We have the one-person bus rule," said Meghan Hoyer, the team's manager. If someone is hit by a bus, someone else should be able to pick up the project without wasting any time.

One concession Hoyer made was to standardize the team around the R programming language. She doesn't regret it. "It was a big lift at the time," she said. "But now I could never go back" to overseeing projects done using less formal structure and documentation. (Note to students: AP data journalism interns are required to come with some facility in R, another good reason to learn it.)

## Replication and the data diary
It doesn't matter where you come down on the esoteric debate on replication. Your data, its analysis and the way it's characterized in publication must be demonstrably accurate. That means understanding exactly what you did, why, where it all is and how it should be communicated to a general audience.

The formal processes used by AP might not work for smaller endeavors, but anyone can put the underlying ideas to work. At the Center for Public Integrity, [Talia Buford kept a simple Word document]({{site.baseurl}}/assets/docs/TB_Data_Diary.pdf) with her questions and code annotated to help her repeat her work.

Enter the data diary.

Think of the data work the same way you think about interview notes or transcripts and any other research for a story. You wouldn't quote a court case without reading it and probably talking to some of the participants. You'd make sure you know where the documents are, and what people say about them. All data work should be documented in at least the same detail. Ideally, someone reading through your notes would be able to repeat your work and understand what it means.

 This is a note to your future self. Things happen in newsrooms. Stopping work halfway through a story and picking it up again six months later happens all the time. You should be able to pick up where you left off after briefly refreshing yourself on your work.

In this module you'll learn:

* The kinds of information you need to record in a data diary or in your documentation
* The questions you'll need to be able to answer before you publish
* A format for recording your work.

(There are disagreements among reporters about how much to try to make our work replicable in the same way scientists do. [Matt Waite's rant](https://github.com/datajtext/DataJournalismTextbook/blob/master/Modules/Replication/introduction.md) on the subject prompted me to [write a rebuttal](https://github.com/datajtext/DataJournalismTextbook/blob/master/Modules/Replication/response.md).)

## Getting started

Before you even start work on a new dataset, open up a new document and just start writing down what you do. For a quick daily story, you might be able to keep your work in one short document. For a longer project, you may find it easier to break your documents apart into logical pieces.

In many cases, you can link to a Jupyter notebook or R markdown program that is self-documenting.  In others, you'll need several documents to maintain a log of where you got data, who you spoke with and interviewed, what alternatives you looked at and what you decided along the way.

Here are some sections that are worth considering whenever you start a story or project.

### Data sourcing

* Where did you get the data? How do you know it's authentic?

* A description of who originally collects the data and why it exists.

* List of other stories that have used this or similar data -- links, advice, warnings and findings.

* Academic work that has relied on the data. Names, contact information for those sources.

* Alternative sources for this and similar or related datasets or documents.

### Data documentation and  flaws

You can keep editing this section as you work on the problems in the data.

If you found some 10-year-old children with drunk driving records, you either imported or converted the data badly or there is a mistake in how it was recorded or transmitted to you. Once you've found out why and fixed it, you can nix that from your diary. But if it's a flaw in the underlying data, you'll describe how you tried to resolve it and what you decided to do about it.

* List each step you took to look for flaws. For example, "Filtered on each field and looked for missing data." -- then what you found.

* What integrity checks did you make? How were they reconciled? Do your totals match reports generated by an agency? Why not? Are there 10-year-old children with drunk driving convictions? How did that happen and how will you resolve it?

* Links or copies of any original documentation such as a record layout, data dictionary or manual. If there isn't one, consider making a data dictionary with what you've learned.

* Questions about the meaning of fields or the scope of the data.

* Decisions you've made about the scope or method of your analysis. For example, if you want to look at "serious" crimes, describe how and why you categorized each crime as "serious" or "not serious." Some of these should be vetted by experts or should be verified by documenting industry standards.

* A list of interviews conducted / questions asked of officials and what they said.

### Processing notes

Some projects require many steps to get to a dataset that can be analyzed. You may have had to scrape the data, combine it with other sources or fix some entries. Some common elements you should document:

* Hand-made corrections. Try to list every one, but it's ok if you describe HOW you did it, such as clustering and hand-entering using OpenRefine. Link to any spreadsheet, document or program you used.

* Geocoding. Note how many were correct, how many missing, and what you did about it.

* A description of how you got messy data into a tabular form or a form suitable for analysis. For example, you may have had to strip headings or flip a spreadsheet on its head. Make sure to write down how you did that.

### The good part: Your analysis

 * Each question you asked of your data, and the steps you took to answer it. If you use programming notebooks, write it out in plain language before or after the query or statements.

 * Vetting of your answers: who has looked them over, commented on them

 * Why they might be wrong.

## Examples of documentation

[A published Jupyter notebook for an analysis of FEC enforcement](http://nbviewer.jupyter.org/github/datadesk/ferc-enforcement-analysis/blob/master/02_analyze.ipynb) actions from the Los Angeles Times' data desk.  Ben Welsh, the author of that notebook, says that there are previous versions with unpublishable work.

[An example of a data diary kept by Talia Buford]({{site.baseurl}}/assets/docs/TB_Data_Diary.pdf), a ProPublica reporter, when she was working at the Center for Public Integrity. She's nicely annotated the document to show why she structures it the way she does.

[A 2018 Buzzfeed News repo with start-to-finish documentation](https://github.com/BuzzFeedNews/2018-05-fentanyl-and-cocaine-overdose-deaths) of an opioid deaths story.


## Data smells: looking for flaws in data

We'll have a  module on data cleaning, but for now, here are a couple of readings that talk about dirty data.

[An email exchange between Sarah Cohen and Craig Silverman]({{site.baseurl}}/assets/docs/bulletproof), now at Buzzfeed, about the process she used at The New York Times in reporting and fact-checking. This isn't the same as a process for replication, but it discusses the kinds of things that should be in it.

[Ensuring Accuracy in Data Journalism, or *Data Smells*](https://github.com/nikeiubel/data-smells/wiki/Ensuring-Accuracy-in-Data-Journalism), by Nikolas Iubel

> -- Sarah Cohen, 2018
