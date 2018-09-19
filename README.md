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

BASE_DIR="${HOME}/BootCampProjects/GitHub"
PROJECT_NAME='HW-Wireframe'

PROJECT_DIR="${BASE_DIR}/${PROJECT_NAME}"

mkdir -p "${BASE_DIR}"

hub init "${PROJECT_DIR}"

touch "${PROJECT_DIR}/index.html" "${PROJECT_DIR}/style.css"

~~~
