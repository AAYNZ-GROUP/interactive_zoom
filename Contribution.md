## Table of Contents

1. [Task and Issue Management](#1.task-and-issue-management)
2. [Branching Strategy](#2.branching-strategy)
3. [Pull Request Workflow](#3.pull-request-workflow)
4. [Code Review and Merging](#4.code-review-and-merging)
5. [Documentation](#5.documentation)
6. [Finding Error in code](#6.finding_error_in_code)

## 1.task-and-issue-management

We’ll use GitHub Issues to manage tasks, bugs, and feature requests.

### Creating and Managing Issues

> in progress
> steps for creating and assigning task will be decided later

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/zveekxs9wlo3q38es1m7.png)

### Using the Project Board

- We’ll organize our work using a project board with columns like `To Do`, `In Progress`, `Review`, and `Done`.
- Assigned issues will be moved from `To Do` to `In Progress` when work begins.

## 2.branching-strategy

To keep our codebase organized and ensure that we can work on features and fixes without interfering with each other’s work, we’ll follow a structured branching strategy.

### Working on a Task

1. **Clone the Repository**: Clone the repository to your local machine if you haven’t already.

```bash
git clone https://github.com/your-repo-url.git
```

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/yicodeep262wnheqrrym.png) 2. **Create a Branch**: From the `main` branch, create a new branch locally for the task or issue you are working.

```bash
# move to your local main branch
git checkout main
# pull the latest changes from the global main branch
git branch branchname
# to make sure u are up to date
git pull origin main
# create and move to your new branch
git checkout  issue-123-fix-bug
```

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/8888x42nvol3ulaei9jg.png)

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/zobirfjcbyxym057xq8i.png)

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/ua12d0bv9lzcpgmgdpmi.png)

1. **Work on the Task**: Implement your changes, commit them locally, and push the branch to GitHub.

```bash
# check being up to date with
git pull origin main
# add your latest changing to staging are in your local machine
git add .
# commit your changes to the branch you created
git commit -m "Fix bug related to issue #123"
# push the branch you created to github
git push origin issue-123-fix-bug
```

## 3.pull-request-workflow

Once your work is done, you’ll submit a pull request (PR) to have your changes reviewed and merged into `main`.

### Creating a Pull Request

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/p36s3ycwuqq3k3s50yvl.png)

- **Link to the Issue**: When opening a PR, make sure to link it to the relevant issue by mentioning the issue number in the PR description (e.g., `Closes #123`).

> by mentioning the issue number in your description with tag fixes or closes.. etc
> The issue automatically is connected with the pull request

> Use the tag Closes or fixes when the pull
> request finishes the issue completely `Closes: #123` `Fixes: #123`
> if not
> Just mention the issue number `#123`

- **PR Description**: Provide a clear title and description of the changes you made. Include any context or screenshots that might be helpful during the review.

## 4.code-review-and-merging

### Reviewing Pull Requests

> in progress

- **Review Process**: 2 members must accept pull request before merging it to the main branch.
- **Feedback**: If changes are needed, feedback will be provided in the PR. Once all requested changes are made and the PR is approved, it can be merged.

### Merging PRs

> in progress

## 5.documentation

> in progress

## 6.finding_error_in_code

> in progress

- if u find an error in code already in the code base don't change it
- create an issue first on GitHub
- add a clear description of the issue u found

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/3uvs7a50a9284cpc580v.png)

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/1kt7uagse6gg6028g4fp.png)

![Image description](https://dev-to-uploads.s3.amazonaws.com/uploads/articles/1i6rmtaoeepyllshe4vi.png)
