# Applying Etter's Modern Technical Writing principles

<br />

# Purpose
The purpose of this text is to document the steps of how to format and host a resume online. Further, each step in both for-mating and hosting can be traced back to a principle that Andrew Etter describes in their book *Modern Technical Writing* 

<br />

# Prerequisites
## FirstName LastName
Address \
Phone: \
Email:

---

### Education
**Level of Education completed** \
StartDate - EndDate \
Institution

---

### Projects
[**Project Name**](Link to Project)
* Details about the projecy

---

### Work Experience
**Work** \
Work location \
Work duration


---

### Extra Curricular Activities
**Activity** \
Date

<br />

# Instructions
## Use detailed version control
Etter (2016) argues that using distributed version control is important for technical writers because developers prefer using it over centralized systems. Hence as a technical writer, it is important to know how to share and host documents on a distributed version control system.

For my distributed version control system, I chose Github Here are the steps I performed in order to create this repository
1. Sign in or create an account in github.com
2. Go to https://github.com/dashboard
3. Press the green button that says new
4. Choose an appropriate repository name
5. Set the repository to public
6. Press the Create repository button

There are various ways of cloning a repository directly to your machine, but since I am using Visual Studio Code as a part of my stack, I will be demonstrating how I cloned the repository with Visual Studio Code
1. Go to the repository you want to clone
2. Click the green button that says Code
3. Copy the HTTPS link on the drop down
4. Open Visual Studio Code
5. Click on the Source Control button on the list of buttons on the left side of the screen
6. Click the Clone Repository Button
7. Paste the HTTPS link in the text box provided
8. Press Clone from URL
9. Select a directory in your computer to store the repository
10. Click open once a popup window appears

## Use Lightweight markup

Etter (2016) suggests using a lightweight markup language for documentation because not only is it free, but it also has better longevity due to its compatibility with version control as opposed to creating PDFs with text editors like Microsoft Word. One of the most popular languages being Markdown.

To create and edit my markdown file, I used Visual Studio Code. 
1. Click File, then open
2. Open the folder containing your cloned repository from the previous step
3. Right click on the Explorer tab
4. Press New file...
5. Name this new file index.md

index.md is where you would write your resume using the markdown language.

Upon completing your resume in index.md, you would need to push these changes online to Github.
1. Click the source control button
2. In the Message text box, write a message detailing what you did
3. Press the Commit button
   
## Make Static Websites

Upon recreating my portfolio using Markdown, we now need to be able to display it such that potential employers can easily access it. We will accomplish this by building and hosting a static website. Etter (2016) recommended making static websites because it can easily be hosted anywhere due to static websites not requiring many dependencies. Further, there are plenty of generators that automatically create the static website for you. Etter suggested various hosts and generators, but the ones that I found most appealing to my current setup is GitHub Pages and Jekyll.

Here are the steps to creating a static website with Github Pages and Jekyll
1. Go to the repository you want to clone
2. Go to the Settings tabs
3. On Code and automation, click Pages
4. Set Source to GitHub Actions
5. Click the configure button on the Jekyll box
6. Press the green commit changes button
7. Press the green commit changes button again on the popup
8. Go to the Actions tab
9. Click the workflow run that corresponds to the commit
10.  Click on the link in the deploy bubble

Upon clicking the link, you should be redirected to a website containing your portfolio. It should look like this
![](https://github.com/BenedictAg/3040-A2/blob/main/demo.gif)


# Authors and Acknowledgements
The structure of the resume is inspired by the resumes found in Appendix D from the [Resume Book](https://www.umanitoba.ca/career-services/sites/career-services/files/2021-05/Online_Resume_Book.pdf) made by University of Manitoba Career Services

<br />

## Source
Andrew, E. (2016). Modern Technical Writing: An Introduction to Software Documentation. 

<br />

# More Resources
[**The Only Markdown Crash Course You Will Ever Need**](https://www.youtube.com/watch?v=_PPWWRV6gbA) \
When learning a new skill, I found that videos are often the best way to introduce a topic, as such I would recommend this  mark down tutorial by Web Dev Simplified. The video provides a good introduction to Markdown and as well as provides the essential information about Markdown such as how to create Headers and lists. 

<br />

[**How to Add GIFs on README .md File in a GitHub Repository?**](https://www.geeksforgeeks.org/how-to-add-gifs-on-readme-md-file-in-a-github-repository/) \
This website provides information on how to add gifs to your markdown file; which can be useful in README files.

<br />

# FAQs
## Why is Markdown better than a word processor?
For the purpose of documentation, using Markdown is superior to using a word processor. Etter (2016) makes a point in how a word processor file format does not work in version control. Meaning that, you can't make documentation for your Github repositories using a word processor. As such, for technical writing, always choose a lightweight markup language over a word processor.

## Why is my resume not showing up?
Upon completing the steps in instructions, your resume not showing up could be a result of two reason.

The first reason is that your resume is not stored in the correct .md file. Your resume should be stored under the index.md file for it to be displayed in the static website.

The other reason is that Github has not finished deploying the website. You could easily check if this is the case by going to the actions tab, and checking if the most recent workflow run has a green checkmark in it.