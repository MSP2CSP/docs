# Contributing to Docs
 
We'd like to make it as easy as possible for you to work in this repository. The documentation is published at https://MSP2CSPadmin.github.io/docs. The following sections guide you through the process of contributing to the documentation.

The project is managed entirely through the [GitHub repository](https://github.com/MSP2CSPadmin/docs). There you can:

* Use [issues](https://github.com/MSP2CSPadmin/docs/issues) to identify anything with an actionable next step. For example, a page in the documentation that needs to be fixed, a bug in the code, or a specific feature that has a clear scope.
* Submit a [pull request](https://github.com/MSP2CSPadmin/docs/pulls) with modifications to the codebase. Pull requests will be reviewed by one or more members of the core team.

## New contributor guide
---

To get an overview of the project, read the [README](README.md). Here are some resources to help you get started with open source contributions:

- [Set up Git](https://docs.github.com/en/get-started/quickstart/set-up-git)
- [GitHub flow](https://docs.github.com/en/get-started/quickstart/github-flow)
- [Collaborating with pull requests](https://docs.github.com/en/github/collaborating-with-pull-requests)
- [Writing docs in Markdown](https://www.markdownguide.org/)

In addition, you can join our vibrant and growing community

[Join us on Slack](#){ .md-button .md-button--primary }

## Guidelines for contibuting
---

There are two ways to contribute a pull request to the docs repository:

### **Make changes directly on Github**

   You can click the **Edit this page** icon in the right column of every page on [docs websitee] (https//.com)

   This opens the GitHub editor, which means you don't need to know a lot about Git, or even about Markdown. When you save, Git prompts you to create a fork if you don't already have one, and to create a branch in your fork and submit the pull request.

### **Setup the project locally**

Fork the repository on Github. This means that you will have a copy of this repository under `your-GitHub-username/repository-name`.

 - Clone the repository to your local computer.
    ``` 
    git clone https://github.com/github-username/repository-name.git.
    ```
 -   Open the the files in a code editor like Visual Studio Code or Sublime Text.

 - Add the documentation repo as an upstream remote, and fetch upstream data:
   ```
   git remote add upstream https://github.com/MSP2CSPadmin/docs.git
   git fetch upstream

   ```

 - Create and switch to a new local branch called `doc/[branch_name]` based on main branch of the remote upstream.
   ```
   git checkout -b ＜new-branch＞ ＜existing-branch＞

   git checkout -b doc/[branch_name] upstream/main

   ```

 -  Create a virtual environment and activate it
    ```
    python -m venv venv

    venv\Scripts\activate.bat

    ```
 -  Install the dependenciees

    ```
    pip install -r requirements.txt

    ```
 -  Serve/View the docs locally - You can see the local docs running at http://127.0.0.1:8000/

    ```
    run mike serve

    ```

   You should see this in the terminal
   ```
   INFO     -  Documentation built in 1.31 seconds
   INFO     -  [19:25:06] Watching paths for changes: 'docs', 'mkdocs.yml'
   INFO     -  [19:25:06] Serving on http://127.0.0.1:8000/
   INFO     -  [19:25:11] Browser connected: http://127.0.0.1:8000/
   ```

 - Make the changes to the documentation. You can always preview the changes locally. Read more about writng code in Markdown.

 -  Open a  Git bash terminal and add the changed or added files
    ```
    git add # include file location
    ```
 - Commit the changes to your repository with a descriptive message.

    ```
    git commit -m ".." #add your commit message

    ```
 -  Push the changes to your remote repository

    ```
     git push

    ```

 - Submit a pull request to the updtream repository. On your github repo, click on the `Create Pull request` button.

 -  In the description of the pull request, explain the changes that you made, any issues you think exist with the pull request you
    made, and any questions you have for the maintainer. It's OK if your pull request is not perfect (no pull request is), the reviewer will be able to help you fix any problems and improve it!

 -  Your pull request will be reviewed and merged by a maintainer.


