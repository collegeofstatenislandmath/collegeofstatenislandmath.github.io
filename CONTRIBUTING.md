# Contribution Guide

We are delighted that you are considering in contributing to the ***CSI Mathematics Department Website!***

## Before Contributing

But before you get started, you will need to setup your local desktop with the correct tools.

### 1. Fork this repository

Fork this repository by clicking on the fork button at the top of this page. This will create a copy of this repository in your personal Github account.

### 2. Clone this repository

Now clone the forked repository into your personal desktop. Go to your Github account, open the forked repository, click on the code button, and then click
the *copy url* to clipboard icon. Whether that is HTTPS or SSH (*recommended*).

Open a terminal and run the following command:

```bash
git clone <url_you_just_copied>
```

### 3. Create a branch

Change to the repository directory on your local desktop (if you aren't already there):

```bash
cd collegeofstatenislandmath.github.io   
```

Now create a branch (using the git switch command), based on what new feature or issue you would be solving:

```bash
git switch -c <branch_name>
```

For example:

```bash
git switch -c updating_readme
```

### 4. Installing Quarto

Our website is not built off a traditional web stack like HTML + CSS + JS. But rather [Quarto](https://quarto.org/), a tool that turns text files (Markdown) into websites, PDFs, and reports, etc. 
It is also integratable with Python, R, Julia, and Observable!

### Windows

1. Go to the official Quarto downloads page:

    https://quarto.org/docs/get-started/ 

2. Download the Windows installer (.msi)

3. Run the installer which will automatically add quarto to your PATH

4. Verify the installation:

    ```bash
    quarto --version
    ```

### MacOS

For MacOS users, you can install Quarto in two different ways:

Option 1: **Manual Installer**

Follow the same steps as mentioned for the Window users but install the Mac OS installer (.pkg)

Option 2: **Homebrew (recommended)**

If you have [homebrew](https://brew.sh/) installed, simply run:

```bash
brew install quarto
```

### 5. Making & Comitting Changes

You can now start making chnages to your forked version of our repository. Here are some basic pointers on where to start:

#### *Announcements*

Edit the `_quarto.yml` file for a quick announcement

#### *Nav bar*

For a new nav bar entry, edit the `_quarto.yml` file 

#### *News*

Create a new file with `yaml` details including title and date

#### *Faculty*

Create a new file, copy over the template using `about`

#### *New folder*

Create an index.qmd landing page and link to files

After making some changes, whether that is adding a new feature, fixing some syntax issues, etc. execute the `git status` command, where you are able to see which files have uncommitted changes. 

Add those changes to the branch you created using:

```bash
git add <file_name>
```

for adding uncommitted files individually.

OR

```bash
git add .
```

to add ALL uncommitted files at once.

Now commit those changes using the `git commit` command:

```bash
git commit -m "Explain in detail what you are adding/fixing..."
```

The commit messages should be short but descriptive, as you would add more information about what you are doing in your ***pull request***.

### 6. Pushing changes to Github

Push your changes using the `git push` command:

```bash
git push -u origin <your_branch_name>
```

### 7. Submit your changes for review

Remember, when you are pushing your changes to Github, you are not affecting the main repository. You are only making changes to your forked version of the main repository, as you made in the beginning. 

In order to see your changes live:

1. Go to your forked repository on Github, you'll see a *Compare & pull request* button button. Click on that button.

2. Choose a tag to add to your PR title based on what issue you are working on:
    - feat
    - fix
    - docs
    - style
    - refactor
    - perf
    - test

    And a brief description of your PR is focusing on.
    
In your PR description, describe what changes you have made and the following *issue number* that the PR is correlated too. For example:

```
Title: docs: update CONTRIBUTING file (#108)

This PR updates the CONTRIBUTING.md file.

Changes include:
- Added CONTRIBUTING.md with basic contribution workflow and branch naming guide
- ...
- ...

Fixes/Closes #108
```

Finally, you are now able to submit the *pull request*.

### 8. Next Steps

Faculty & Staff will review your PR and either make some suggestions and or comments in the discussion thread
of your *pull request*. 

After everything is set and done, you'll be considered as a contributor and be able to see your changes live on our ***[CSI Mathematics Department Website!](https://collegeofstatenislandmath.github.io/)*** 