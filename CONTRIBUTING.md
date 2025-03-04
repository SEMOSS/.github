# Contributing to SEMOSS / AI Core

Thank you for your interest in contributing to the SEMOSS / AI Core base platform! 
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

If you are a new developer looking to contribute to the base platform and require access to the SEMOSS GitHub and sprint board(s), please reach out to **Kathy Yang**.

## <a name="question"></a> General Question or Problem?

For general questions, first check the [Community Discussion Board](https://github.com/SEMOSS/community/discussions), where you can search for common questions and answers from our community of users and developers
or start a new Discussion. Just be sure to exclude any sensitive information like personal identifiers or connection keys, as the Discussion board is publicly accessible. 

The AI Core Global team also hosts **Office Hours every other Thursday**, where users from different member firms can clarify how platform features function, 
troubleshoot their blockers, or raise recommendations for future platform development. Please reach out to **Jasneet Kaur** for the calendar invite if interested. 

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

Lastly, please add the issue to the **SEMOSS** Project on the right-hand menu, if you have access. 

### <a name="feature"></a> Idea for a New Feature or Feature Enhancement?

You can suggest a new feature or enhancement to an existing feature by [submitting an issue](https://github.com/SEMOSS/community/issues/new/choose) to our Community repository on GitHub using the **Feature Request** template.

Please provide a descriptive and concise title and fill out all relevant sections. If applicable, please include annotated screenshots in the “Additional context” section to 
illustrate the current state of the platform, where you envision the feature existing within the platform, and/or a rough mock-up of what the new feature might look like.

Lastly, please add the issue to the **SEMOSS** Project on the right-hand menu, if you have access. 


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

* Use past tense

* Avoid technical jargon

* Use names that the end-user would be familiar with (for example, "Custom Blocks" instead of "Grouped component", "Access Control tab" instead of "Settings tab")

* Do not leave it as the commit message

**For example:**

`"Added a Slider Block to System Blocks"` ✅

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

For example ticket number 10, with type test, and scope api with the commit message being 'added api tests', your commit would be:

`[#10] test(api): added api tests`

### Type

Commit type must be one of the following: 

* `build`: Changes that affect the build system or external dependencies 
* `chore`: 
* `ci`: Changes to our CI configuration files and scripts
* `docs`: Documentation only changes
* `feat`: A new feature
* `fix`: A bug fix
* `git`: 
* `perf`: A code change that improves performance
* `refactor`: A code change that neither fixes a bug nor adds a feature
* `revert`: 
* `style`: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
* `test`: Adding missing tests or correcting existing tests

### Scope

Commit scope must be one of the following:

* `(client)`: The "new" UI for the AI Core platform, including Agent Builder, Engine Catalogs, Engine Settings, etc. 
* `(legacy)`: The "old" UI, the BI tool, and terminal
* `(ui)`: Base component library for the UI
* `(renderer)`: Library used for Drag-and-Drop App Builder
* `(sdk)`: Tools to help developers tap into SEMOSS enviornment

