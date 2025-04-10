# Contributing to SEMOSS / GovConnect.ai

Thank you for your interest in contributing to the SEMOSS / GovConnect.ai base platform! 
Below are the guidelines we would like you to follow:

 - [GitHub Access](#access)
 - [General Platform Questions](#question)
 - [Ticket Submission Guidelines](#submit)
 - [Reporting Bugs](#bug)
 - [Feature Requests](#feature)
 - [Submitting a PR](#submit-pr)
 - [Coding Rules](#rules)
 - [Commit Message Conventions](#commit)


## <a name="access"></a> Need Access?

If you are a new developer looking to contribute to the base platform and require access to the SEMOSS GitHub and sprint board(s), please reach out to semoss@semoss.org

## <a name="question"></a> General Question or Problem?

For general questions, first check the [Community Discussion Board](https://github.com/SEMOSS/community/discussions), where you can search for common questions and answers from our community of users and developers
or start a new Discussion. Just be sure to exclude any sensitive information like personal identifiers or connection keys, as the Discussion board is publicly accessible.

## <a name="submit"></a> Submission Guidelines

New bug reports and feature requests from the community are housed in the [Issues tab of the Community respoitory](https://github.com/SEMOSS/community/issues).
Before you submit an issue, please search for your bug or feature request as a ticket may already exist. If it does, feel free to edit or comment with new supplementary information. 

**For all tickets, please crop and redact all sensitive information so that uploaded images and text
contain no user personal information (e.g. names, emails, IDs), platform URLs, or connection details (e.g. API keys).**

A more in-depth guide on how to submit a new ticket can be found on the README of the [Community repository](https://github.com/SEMOSS/community). 

### <a name="bug"></a> Found a Bug?

If you find a bug, you can help us by [submitting an issue](https://github.com/SEMOSS/community/issues/new/choose) to our Community repository on GitHub using the **Bug Report** template. 

Please provide a clear and concise title and fill out all the relevant sections, including steps to reproduce the error and screenshots of the UI or logs if applicable.
You can access the logs tab by right-clicking on the screen selecting Inspect from the menu. 

Lastly, please add the issue to the **Catch-All** Project on the right-hand menu, if you have access. 

### <a name="feature"></a> Idea for a New Feature or Feature Enhancement?

You can suggest a new feature or enhancement to an existing feature by [submitting an issue](https://github.com/SEMOSS/community/issues/new/choose) to our Community repository on GitHub using the **Feature Request** template.

Please provide a descriptive and concise title and fill out all relevant sections. If applicable, please include annotated screenshots in the “Additional context” section to 
illustrate the current state of the platform, where you envision the feature existing within the platform, and/or a rough mock-up of what the new feature might look like.

Lastly, please add the issue to the **Catch-All** Project on the right-hand menu, if you have access. 


## <a name="submit-pr"></a> Submitting a Pull Request (PR)

### Before you submit your PR

Make sure you have:

1. Tied your branch to the Issue it addresses. 

2. Tested your code thoroughly.

3. Followed the coding standards outlined in the README of the appropriate repository (semoss-ui for front end, Semoss for back end).

4. Committed your changes according to our commit message conventions

### PR Naming Convention

The name of the PR is what will appear on the Release Notes and Changelog. Please try to use a clean, descriptive line of accessible language that mirrors the original ticket title. 

Some keys to keep in mind:

* Use present-tense, imperative-style language, as if you are giving a command to the code base (e.g. "fix pagination bug in Members Table")

* Avoid technical jargon

* Use names that the end-user would be familiar with (for example, "Custom Blocks" instead of "Grouped component", "Access Control tab" instead of "Settings tab")

* Do not leave it as the commit message

**For example:**

`"Add a Slider Block to System Blocks"` ✅

`"feat(ui): slider component build"` 🚫


### Addressing reviewer feedback

If we ask for changes via code reviews then:

1. Make the required updates to the code.

2. Re-run tests to confirm they still pass.

3. Commit your changes following our conventions. 

### After your PR is merged

You can safely delete your branch and pull the changes from the main (upstream) repository.


## <a name="rules"></a> Coding Rules

To ensure consistency throughout the source code, please follow the coding standards outlined in the README of the
specific repository you are contributing to (Semoss for back end, semoss-ui for front end). 


## <a name="commit"></a> Commit Message Format

We have precise rules over how our Git commit messages must be formatted.

Fully flushed out syntax for a commit is:

`[#IssueNumberOnGithub] type(optional scope input): any message`

For example, for a ticket with an issue number of **10**, type of **feat**, scope of **client**, and commit message of **'add date picker drag-and-drop system block'**, your commit would be:

`[#10] feat(client): add date picker drag-and-drop system block`

### Type

Commit type must be one of the following: 

* `build`: Changes that affect the build system or external dependencies 
* `chore`: Grunt tasks like removing dead code,fixing comments, and removing completed todos
* `ci`: Changes to our CI configuration files and scripts
* `docs`: Changes to documentation only
* `feat`: A new feature
* `fix`: A bug fix
* `perf`: A code change that improves performance
* `refactor`: A code change that neither fixes a bug nor adds a feature
* `revert`: A code change that undoes a previous change
* `style`: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
* `test`: Adding missing tests or correcting existing tests

### Scope

Commit messages can contain a scope in parentheses after the type. However, these scopes differ between repos so it is best to 
check the README of the repo you are currently working on to see the list of scopes available for that repository.

