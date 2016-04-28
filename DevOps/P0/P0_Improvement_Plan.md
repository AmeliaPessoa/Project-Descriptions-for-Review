# [DevOps P0] Improvement Plan: Project Description

## Introduction
In this project, you will create a document that describes the current situation in a company as seen from the perspective of either a software developer or a member of the IT operations team. The document should capture the typical processes by which software is built, tested, and put into production. The document should reflect both what processes are going well and what processes could be improved.

As you progress through the Nanodegree program, you will continuously update the document to reflect your new skills. This will serve not only to show what you have learned, but also as a source for inspiration for changes that you can bring to your organization using DevOps tools, techniques, and practices.

The goal of this project is to reinforce the core value of DevOps. DevOps is not just a set of technical tools; it is a way of rethinking business processes throughout the organization. The DevOps philosophy sees IT and software development as core components of the organization, working in collaboration with Marketing, Sales, Accounting, and other teams to advance the core function of the company. To understand the value of DevOps and the mindset of a DevOps engineer, it's necessary to look at the larger business context. This project is meant to help you place the DevOps tools you will learn throughout this Nanodegree program in that larger context.

In creating the document, if you are comfortable using your real-life experiences (from your current position or from previous jobs), feel free to do so. However, using real scenarios may be sensitive from both a business and a personal standpoint. If you wish to keep real-world information out of the project, or if you have not previously worked in a field related to DevOps, use the following resources to generate the document:

* Talk with friends who currently work in IT Ops or software development, asking about the software development and deployment process. What works well? What is difficult? 
* Search the web to get a sense of typical [processes](https://www.google.com/#hl=en&q=IT%20development%20typical%20processes) and [problems](https://www.google.com/#hl=en&q=IT+development+typical+processes+problems) around the software development lifecycle, and use them in your narrative.
* Take a look at the [sample project submission](P0_Sample_Submission.md) that has been provided as a guide.
* Using the suggestions above, add some detail to this [description of a fictional company](P0_Fictional_Company.md) and use it for your project.

Your project has two parts: first, a series of short, open-ended brief questions you must answer to provide an overview or **snapshot of your (real or fictional) organization**; second, a set of **quantitative ratings** you provide about the effectiveness of collaborative processes within the organization.

The assignment is meant to be a low-stakes way to get you started thinking like a DevOps engineer. Use these questions as a way of orienting yourself to the sort of issues DevOps engineers tackle. Don't worry about finding the perfect answers! It's okay if you don't know some of them right away. You will revisit the document and fill in the details later. Every time you add to the document, **put in the date** so that you have a record of how your answers change over time.

The project is intended to take about 1.5 to 2 hours to complete. 

## Organization Snapshot

Assume that you are either a software developer or an IT Operations employee at the chosen company. You will be asked to answer these questions that will provide an overview of the current state of the organization as you understand it today.

#### Provide a brief description of the company and your team's role in it.

Please address such questions as:

* What is the company's main business?
* How long has it been in existence?
* How many employees are in the company?
* What is the role of your team or organizational unit within the company? 
* How many employees are in your organizational unit or team?

The response should give a clear picture of the company as a whole and the team's role. 

#### What is the core function of your team? What is the core function of your company or organizational unit? Is the core function of your team well aligned with the function of the larger organizational unit or the company as a whole?

The *core function* of a team is the one clearly stated objective around which the team is organized. A team may have several different responsibilities. For example, an IT team might both provide end-user support and maintain infrastructure such as file servers. But the core function of the team might be something like "ensuring all employees have the IT tools and resources they need to do their jobs efficiently". 

Depending on how big your company is you might want to think about several levels of core business. For example, if you work at a company that sells shoes, these might be the core functions at various levels: 

* Team: developing the software to sell shoes online
* Organizational unit: handling all matters related to selling shoes online
* Company-wide: selling shoes

#### Who are your team's customers? Are they internal or external? What do they need?

To continue with the shoe selling example, the software development team has both external and internal customers. 

* External: the customer purchasing the shoes
* Internal: the warehouse staff who need to fulfill the orders and maintain inventory.

There might be other internal customers as well, such as the accounting department. Any stakeholder who needs some functionality from the software product counts as a customer. 

#### What is the current flow of software development and delivery in your team? List the main steps and whether they are manual or automated. 

Steps might include:

* Specifying desired functionality
* Assessing user requirements
* Coding the application

and so on. 

#### What are all the teams or people that are involved in a product release, from start to finish? 

You will likely include the product team, developers, testers, sysadmins, marketing, and others in this list. 

#### How is communication handled in your organization? 

Consider such questions as:

* Whom do you work with? For work purposes, do you only interact with your team members and manager, or also with people outside your team? Are those external interactions formal meetings, informal chats, or both? 
* Are both developers and operations involved when starting a new project? Do developers receive and act upon feedback from operations regarding how the software is performing?
* How do internal customers make their requirements known? Do they directly communicate with the developers?

## Quantitative Ratings

You will be asked to provide the ratings described below. If a given rating is lower than you would like, we recommend that you provide a short explanation of the issue and some suggestions about how to resolve it. 

#### How satisfied are you with how other teams work and support the work that you do? 

Rate on a scale from 1-10, with 1 being least and 10 being most satisfied. You may give an overall rating, or separate ratings for each other team. 

#### Do deployments go smoothly?
 
Rate on a scale from 1-10, with 1 being least and 10 being most smooth.

#### Do you have planned downtime for system upgrades or maintenance? 

If yes, please specify:

* What is the schedule according to which the system is taken offline? Specific days, specific times of day? 
* How long is the maintenance window?
* Is this downtime enough to complete the required upgrades satisfactorily?
* From a business perspective, is this downtime is too long or too frequent? Or is it acceptable?
* Ideally, how short would the downtime be, while still being sufficient to perform all the needed maintenance?

#### How much time does it take to set up the environment for a new project? 

Please provide your answers in time units, e.g. 5 hours or 2 days. If it takes longer than desired, what would your target be for this? 

#### How often do you deploy to production? 

Please provide your answer in deployments per time unit, e.g., a maintenance release every month and a full upgrade every six months. What do you think would be optimal? 

#### How long does it take to deploy a new feature or bugfix from "code checked in to repository" to "feature is live to customers"? 

Please provide your answers in time units, e.g. 5 hours or 2 days.

#### How easy is it to deploy a new feature or bugfix from "code checked in to repository" to "feature is live to customers"?  

Rate on a scale of 1-10, with 1 being most difficult and 10 being easiest.

#### How would you rate the quality of your software? 

Rate on a scale of 1-10, with 1 being worst and 10 being best. How do you measure quality? Please explain the reason for your rating. 

#### How easy it is to test your software?

Rate on a scale of 1-10, with 1 being most difficult and 10 being easiest. How do you measure ease of testing? Please explain the reason for your rating. 

#### How satisfied are your customers? 

Rate on a scale of 1-10, with 1 being least satisfied and 10 being most satisfied. How do you measure customer satisfaction? Please explain the reason for your rating. 

## Submission format

Your document must be submitted in **Markdown format**. Markdown uses a plaintext file and the `.md` file extension to generate a document that renders attractively in a web browser. This document is itself written in Markdown. If you don't know Markdown, rest assured that it's quite easy. A [handy online tutorial](http://www.markdowntutorial.com/) promises to teach you all you need to know about Markdown in ten minutes. 

You can download a [template](https://raw.githubusercontent.com/udacity/Project-Descriptions-for-Review/master/DevOps/P0/P0_Template.md) that you can use to create your Improvement Plan. The template is already in Markdown and has space for you to provide your answers. After downloading the template, please rename it to `P0_FirstName_LastName.md` with your first and last name, then edit it to include your answers.

Many text editors allow you to edit, save, and preview Markdown documents. For example:

* [BBEdit](http://www.barebones.com/products/bbedit/), a Mac-only application, does so natively
* [SublimeText](https://www.sublimetext.com/), for both Mac and Windows, has [extensions](https://www.macstories.net/roundups/sublime-text-2-and-markdown-tips-tricks-and-links/) that provide the preview functionality. 

You can find other Markdown editors on the web. Or you could use any text editor to edit the Markdown template, and any modern web browser to open the document for a preview. 

## Assessment and Submission Details

### How will the project be reviewed? 

Your submission will be reviewed using [this rubric](https://review.udacity.com/#!/projects/7709298823/rubric). Please go through the rubric carefully to ensure that you have addressed all the project requirements.

### What is the procedure to submit the project? 

When you are confident that your Improvement Plan meets all the requirements of the rubric, you can submit your `P0_FirstName_LastName.md` file at [this link](https://review.udacity.com/#!/projects/156/submit-file).
