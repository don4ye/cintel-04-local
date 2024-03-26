# Name: MONSURU ADEBISI
# Cintel-04-Local

## Overview
This repository contains the code for the Cintel-04-Local project. It is a web application built using Shiny, Python, and other technologies.

## Getting Started
To run this project locally, follow these steps:

1. Clone this repository to your local machine.
2. Navigate to the project directory.
3. Create a virtual environment in the `.venv` folder:
   ```bash
   py -m venv .venv

## Activate the virtual environment:
.\.venv\Scripts\Activate

## Install the required packages:
py -m pip install -r requirements.txt

# Adding Penguins Folder and App.py
I've created a penguins folder and moved the app.py file into it. Now, the project structure looks like this:
cintel-04-local/
|-- .venv/
|-- docs/
|-- penguins/
|   |-- app.py
|-- .gitignore
|-- README.md
|-- requirements.txt


## Verify that the app runs:
shiny run --reload --launch-browser penguins/app.py

# Building the Client-Side App
To build the client-side app and publish it to GitHub Pages, follow these steps:

## Remove any existing assets:
shiny static-assets remove

## Export the app to the docs folder:
shinylive export penguins docs

## Serve the app locally:
py -m http.server --directory docs --bind localhost 8008

# Git Operations
After making changes to the project files, use the following commands to commit and push them to GitHub:
git add .
git commit -m "Your commit message"
git push origin master

# Publishing GitHub Pages

To publish the app on GitHub Pages, configure the repository settings as follows:

1. Go to the repository on GitHub and navigate to the Settings tab.
2. Scroll down and click the Pages section on the left.
3. Select main as the source branch.
4. Change the folder from the root to docs.
5. Click Save and wait for the site to build.
6. Once the site is published, copy the GitHub Pages URL for your app.

# Customizing the Browser Tab Title and Favicon
To customize the browser tab title and favicon, edit the index.html file in the docs folder. Update the <title> tag with a unique title, and add a link to your custom favicon using the following code:

  <title>Your Unique Title</title>
 <link rel="icon" type="image/x-icon" href="./favicon.ico">


# Project URL
