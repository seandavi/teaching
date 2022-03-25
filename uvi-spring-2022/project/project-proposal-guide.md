---
title: Project Proposal Guide/Template
---

## Introduction

Give a narrative description of the problem you are addressing, and the
methods you will use to address it. Provide context:

1.  What is the question you are attempting to answer?
2.  Why is this question important? (Why should we care)
3.  How will you go about attempting to answer this question?

I'm less interested in the answer to the question than in you using R to describe the data, the variable, the relationships between them, and the interpretation of those findings.

## Data Sources

You have been provided with a list of COVID-19 data sets. You are to
select a dataset(s) that will be suitable for answering your proposed
question.

1.  What datasets will you use to answer your question?
2.  Who/What are the observations in the dataset?
3.  To what population do the observations belong?
4.  How many observations are there?
5.  Which variables will your analysis focus on?
    - Describe your variables.
    - Are the variables categorical or quantitative
    - Do you expect a possible association between any of your variables of interest?

## Data Visualization and Data Analysis

1.  Which graphs do you intend to generate based on your question and
    selected variables?
    - Consider adding a section on each variable where you give descriptive statistics, plots, or summaries.
    - For each variable, consider how it relates to other variables in the datasets and use plots or tables to show the relationship(s).
2.  What tools will you use throughout? (these can be tentative). For example:
    - dplyr (for manipulating dataframes)
    - ggplot2 (for plotting)
    - sars2pack
    - kable and kableExtras (for making tables)
    - summary statistics (mean, median, min, max, table, summary)
3.  Do you have a testable hypothesis and any expected outcomes for your
    proposed question?
    - You may not end up with testable hypotheses, but that is OK.
    - Using exploration and looking for relationships between variables is often the first step in data analysis.
4.  What statistics will you provide?
    - Note that a `statistic` is defined as "a fact or piece of data from a study of a large quantity of numerical data."
    - Descriptive statistics such as mean, median, standard deviation are all really useful.

## Submission

One member from each group can submit the proposal on behalf of thegroup. You are to also include how each group member contributed to the development of your project. You are creating a R MArkdown document. You should submit a PDF or HTML and the .rmd file to blackboard.

## Feedback

Dr. Davis (<sean.2.davis@cuanschutz.edu>) and Dr. Rogers
(<lavida.brooks@uvi.edu>) will provide students with feedback and guidance on their proposed projects.

## Ideas for dividing work

- If you are proposing to work with more than one dataset, have one person prepare a section of Rmarkdown on each dataset.
- Have each member of the group take responsibility for one set of figures or tables.
- Have one person responsible for keeping the "master" Rmarkdown and making sure that it always "knits" after adding new material.
