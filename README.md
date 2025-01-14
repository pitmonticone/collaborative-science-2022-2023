 [![Creative Commons License](http://mirrors.creativecommons.org/presskit/logos/cc.logo.png)](http://creativecommons.org/licenses/by-nc-nd/4.0/)

# An introduction to modern tools for collaborative science 

## Best practices in co-developing and co-authoring

- Luca Heltai (<luca.heltai@sissa.it>)

All lectures are live in Room A-133, and on zoom on 

https://sissa-it.zoom.us/j/81471012769?pwd=QnNiZnVtbUxvNENybXlPNWVsT1hmQT09

Meeting ID: 814 7101 2769
Passcode: GitRules

The official course page, with the schedule and up-to-date information is 

https://www.math.sissa.it/course/phd-course/collaborative-science-2022-2023

## Course information

Collaboration (or *the action of working with someone to produce something*) is one of the fundamental pillars in Science.

While some types of collaborative efforts are done synchronously (either "in person", during coffee breaks, using blackboards, whiteboards, workshops, etc., or "remotely" via phone calls, skype/zoom/meets meetings, email exchanges, etc.), most of the time they require separate efforts from the various participants, which then need to be synchronized.

Let's take the action of writing a paper  (using LaTeX) with a co-author as an example. John and Jane have discussed a new and interesting topic on the black board, and now they want to write it down.

Jane starts up, and prepares a draft, with title, sections, and so on. John waits for Jane to be finished, then starts working on the same document. Wait. How do Jane and John exchange information (in this case, a LaTeX document)?

A workflow could look like the following:

1. Jane works on a document. Then sends it by email to John.
2. John receives the document. He changes it. John sends it back to Jane. Jane receives it and *replaces* the old document with the new one, or saves it as a new file (with a meaningful name, like `document_v2.txt`).
3. Repeat.

In a simple and linear world, this would work fine. However:

1. Working in parallel is difficult. With more than two authors, life becomes cumbersome, to say the least.
2. Overwriting the wrong file is always a risk, and agreeing on the right naming convention is often more difficult than it looks like.
3. We'll end up with our directories full of files like `document_final_final_2_really_final.tex`
4. Often we end up with files that don't compile, and we need to start "chasing for errors", before we can even start working on our task

In this short course I'll discuss modern tools used to automate the above process, and to introduce fail-safe habits that will make your life as a researcher much easier. In particular, the main topics of this course will be:

1. Minimal introduction to command line interfaces
   1. Introduction to Linux/Unix and bash
   2. bash scripting

2. Version control systems
   
   1. An historical overview (RCS -> CVS -> SVN -> GIT)
   2. Using GIT for single user projects
   3. Using GIT for small collaborative projects
   4. Using GIT for large collaborative projects
   5. Github examples

3. Testing systems
   
   1. Unit tests
   2. Functional tests
   3. Integration tests

4. Continuous integration systems
   
   1. Combining version control systems and test systems
   2. Github actions

5. Container systems
   
   1. Docker
   2. Singularity
   3. Integrating docker or singularity with github actions
   4. Integrating docker with Visual Studio Code

6. Putting it all together
   
   1. Create a working environment
   2. Cloning the working environment on github/gitlab actions
   3. Singularity aware usage of SISSA cluster 
   4. Cloning the working environment on SISSA cluster

At the end of the course, you will be able to setup a collaborative environment that will make your day-to-day work much safer, and much more effective, both if you work alone, or if you collaborate with hundreds of other people.

We'll work through some examples based on the LaTeX typesetting language, and on the python programming language. You will end up with two template repositories (one for a LaTeX paper, and one for a python project) that will allow you to bootstrap your day-to-day research with state-of-the-art tools for collaborative science development.

Particular attention will be dedicated to reproducibility, providing a safe way to share programming environments (containers) both with colleagues, with automated testing systems (github actions/travis CI/etc.), and with cluster programming environments (Ulysses) including ways to guarantee reproducibility of your results

## References and Text Books:

-   Pro Git, Scott Chacon, 
    [\[E-Book-ENG\]](https://github.com/progit/progit2/releases/download/2.1.331/progit.pdf)

-   Git Immersion [\[Interactive Site\]](https://gitimmersion.com/)

-   Learn git branching [\[Interactive Site\]](https://learngitbranching.js.org/)

## A final note

This repository contains assignments, workspaces, and other material for the course "An introduction to modern tools for collaborative science"

New material will be uploaded frequently,

Remember to set a second remote, either to our seed

	git remote add teacher https://github.com/luca-heltai/collaborative-science-2022-2023.git

or (if using ssh keys in your github account)

	git remote add teacher git@github.com:luca-heltai/collaborative-science-2022-2023.git

and to update before the lectures:

	git pull teacher main

**Please consider contributing pull requests to correct typos, or better document the material in this repository!**

# Licencing

The content of this repository is distributed with a Creative Common licence. See
the file LICENCE.md in this directory for more information.

# Attribution

Attributions of the various lectures will be added here.