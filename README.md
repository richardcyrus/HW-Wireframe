# HW-Wireframe

A web design skeleton build using HTML/CSS

## Specifications

* Create a project folder named `HW-Wireframe`.
* In the project folder create the following files:
    - `index.html`
    - `style.css`.
* The HTML document should contain each of the following sections:
    * Header (`<header />`)
    * Nav (`<nav />`)
    * Aside with heading (`<aside />`)
    * Section with heading (`<section />`)
    * Article with heading, contained within a section (`<article />`)
    * Headers contained within the article (`<h1 />` .. `<h6 />`)
    * Paragraph contained with the article (`<p />`)
* The CSS should have the following style elements:

~~~css
body {
    background: #777;
    color: #777;
    font-family: 'Arial', 'Helvetica Neue', Helvetica, sans-serif;
    font-size: 18px;
    width: 960px;
}

aside,
footer,
header,
nav,
section {
    background-color: #ebebeb;
}

article {
    color: #ebebeb;
    background: #777;
}

section {
    width: 496px;
}
~~~

# Scripted Project Setup

~~~bash
#! /usr/bin/env bash

# Define the Project Name and Folder Name.
PROJECT_NAME='HW-Wireframe'

# Define the parent location for the project files.
BASE_DIR="${HOME}/BootCampProjects/GitHub"

# Define the complete project location.
PROJECT_DIR="${BASE_DIR}/${PROJECT_NAME}"

# Make sure the parent project directory exists
mkdir -p "${BASE_DIR}"

# Change to the parent project path.
cd "${BASE_DIR}"

# Create the Git repository for the project, and setup the capability to
# push changes to GitHub.
hub init -g ${PROJECT_NAME}

# Change into the project folder.
cd "${PROJECT_DIR}"

# Create the files needed in this project.
touch index.html style.css

# Add the project files to version control and push them to the GitHub
# remote repository.
git add . && git commit -m "Initial Project Setup"
git push origin master
~~~
