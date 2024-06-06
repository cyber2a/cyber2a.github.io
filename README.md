# Cyber2A Project Website

## Repository structure

Here's an overview of the main directories in this repository:

* **assets/**: Store images and files for the main page.
* **people/**: Information about team members.
* **news/**: News articles and updates.
* **webinars/**: Files and information related to webinars.
* **workshop/**: Files related to workshops. 

## How to Add New Items

### Adding team members / news articles / webinars
1. Navigate to the `{people/news/webinars}/content/` directory.
2. Create a new file using the `_template.qmd` file as a template.
3. Add the content in the Quarto Markdown format.
4. Save the file and commit your changes.

### Modifying workshop introduction content
1. Navigate to the `workshop/` directory.
2. Edit the `index.qmd` file.
3. Save the file and commit your changes.

### Modifying workshop session preview content
1. Navigate to the `workshop/preview/` directory.
2. Edit corresponding session files as needed within this directory.
3. Save the file and commit your changes.

## How to Build the Website
Once you push the changes to the repository, Github Actions will automatically build the website and deploy it. You can view the website at [https://cyber2a.github.io/](https://cyber2a.github.io/).
