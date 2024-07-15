---
author: amanda-visconti
date: 2019-08-12
layout: post
slug: github-jekyll-glossary
title: "Running a collaborative blog: A glossary for GitHub & Jekyll"
crosspost:
  - title: Amanda's blog
    url: https://literaturegeek.com/2019/08/12/github-jekyll-glossary
---
[Brandon Walsh](https://scholarslab.lib.virginia.edu/people/brandon-walsh/) and I are writing a _[Programming Historian](https://programminghistorian.org/)_ lesson on how to run a collaborative research blog, picking up from [my previous _Programming Historian_ lesson](https://programminghistorian.org/en/lessons/building-static-sites-with-jekyll-github-pages) on setting up a scholarly blog using Jekyll and GitHub Pages. We're building on documentation written, tested, and improved by the Scholars' Lab community (staff and students) for use with this ScholarsLab.org website, which we [recently migrated](https://scholarslab.lib.virginia.edu/blog/site-relaunch/) from WordPress to Jekyll. In this post, I'll share our glossary for some commonly used terms when using GitHub to publish blog posts and other webpages.

## Commonly used terms
- **Git** is a versioning system (track changes made by one or more authors to the same piece of text/code over time), **GitHub** is a website (GitHub.com) and software (GitHub Desktop) based around git, and **GitHub Pages** is a web hosting solution offered by GitHub (place that stores and serves the files that make up your website to people who visit it).  
- **Repo** (aka repository): A collection (aka set) of code. The repo of code that makes up this website you're reading my post on is the place on GitHub.com where we store all the files that make up the ScholarsLab.org website (GitHub.com/ScholarsLab/ScholarsLab.org)
- **Branch:** A copy of the website files where you can make changes without affecting the live website or other folks' development or authoring work
- **Master** (aka master branch): The branch from which our live website gets it data
- **Merging:** Taking two sets of code (that already have some shared code/text between them, e.g. our master branch and a duplicated-then-altered branch we created), and combining these into one set of updated code. 
- **Pull request, aka PR:** Asking that the changes you've made in your branch be "pulled" (moved) into another branch (usually master). 
- **Review:** For our repo, making a pull request notifies other Scholars' Lab folks that someone's making a change to our website, allowing the opportunity for feedback on your work. You can set things up so pull requests do or do not require review before merging changes to the repo
- **Checks** aka **tests**: Our pull request process runs two tools over code you're hoping to merge: *Travis* makes sure your changes don't break anything on the main website, and *Netlify* lets you take a peek at how your changes will look on the website, before we actually publish those changes for the world to see.  
- **Conflicts**: Errors that git isn't sure how to resolve. While trying to merge your code, git ran into something it doesn't know how to solve (e.g. Line X in File Y says a different thing in each branch, and git doesn't know which one to keep), requiring human intervention  
- **Development** vs. **production** (e.g. dev vs. production website): Not currently set up for this website, but this is the standard practice of having one website the public sees (production), and one non-public version of the site where we make and test changes (development)
- **Markdown**: Markdown is a very lightweight way of marking up text to format it; the goal is commands that are easy to remember, easy to type, and easy to transform into other markup languages. For example, where HTML uses `<strong>bagels</strong>` to bold the word bagels, markdown uses the simpler `**bagels**` (italics: `*bagels*`). The file format for Markdown is .md (e.g. events.md).
- **Front matter** aka **YAML**: Metadata about a post or page, appearing at the top of a file. Also sometimes referred to as YAML ("yeah-mole"), which seriously stands for Yet Another Markup Language (the language the front matter uses). Metadata such as publication date and author helps the site do stuff like sorting and filtering content (e.g. "display all blog posts by current or former student affiliates on this page").  
- **Issue** (aka ticket): This is how GitHub lets us make a note about a bug we've identified and need to fix, a feature request, ideas for future site features, and similar tasks. We try to keep these to single tasks when possible (one task per issue), include enough info so anyone on the team can address the issue, and add a few pieces of metadata to each issue: ID if a specific person needs to address the issue, label what kind of work it requires (e.g. fixing a bug, content writing/editing, design/development work, documentation writing), and attach the issue to a "milestone" to signal when it needs to get done (way of gathering multiple issues and setting a deadline on addressing them, e.g. "Stuff to fix before annoucing the new website", "Stuff to get done during Spring 2019", and "Rainy Day" for stuff that isn't urgent).  
