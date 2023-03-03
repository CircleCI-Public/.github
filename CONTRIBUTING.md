# Contributing

Thank you for considering to contribute to CircleCI! Before you
get started, we recommend taking a look at the guidelines below:

- [Have a Question?](#question)
- [Issues and Bugs](#issue)
- [Feature Requests](#feature)
- [Contributing](#contribute)
  - [Submission Guidelines](#guidelines)
  - [Release Process](#release)

## <a name="question"></a>Have a Question?

Have a question about CircleCI?

### I have a general question about CircleCI or CircleCI's `config.yml` file.

Contact CircleCI's general support by filing a ticket here: [Submit a request](https://support.circleci.com/hc/en-us/requests/new)

### I have a question about general CircleCI best practices

Share your question with [CircleCI's community Discuss forum](https://discuss.circleci.com/).

## <a name="issue"></a>Discover a Bug?

Find an issue or bug? You can help us resolve the issue by submitting an issue to the specific CircleCI Public Github repository.

Up for a challenge? If you think you can fix the issue, consider sending in a [Pull Request](#pull) in that repo.

## <a name="feature"></a>Missing Feature?

Is anything missing? You can request a new feature by submitting an issues to that specific GitHub repository, utilizing the  `Feature Request` template (if applicable for the repo), or labeling the issue accordingly.

If you would like to instead contribute a pull request, please follow the [Submission Guidelines](#guidelines)

## <a name="contribute"></a>Contributing

Thank you for desiring to contribute to CircleCI!

Before submitting any new Issue or Pull Request, search that respective repository for any
existing or previous related submissions.

### <a name="guidelines"></a>Submission Guidelines

#### <a name="commit"></a>Commit Conventions

Most of our projects strictly adheres to the [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/) specification for creating human readable commit messages with appropriate automation capabilities, such as changelog generation.

##### Commit Message Format

Each commit message consists of a header, a body and a footer. The header has a
special format that includes a type, a scope and a subject:

```markdown
<type>(optional <scope>): <subject>
<BLANK LINE>
<body>
<BLANK LINE>
<footer>
```

Footer should contain a [closing reference to an issue](https://help.github.com/articles/closing-issues-via-commit-messages/) if any.

##### Breaking Change

Append a `!` to the end of the `type` in your commit message to suggest a `BREAKING CHANGE`

```markdown
<type>!(optional <scope>): <subject>
```

##### Type

Must be one of the following:

- **build**: Changes that affect the build system or external dependencies (example scopes: npm, eslint, prettier)
- **ci**: Changes to our CircleCI configuration
- **chore**: No production code changes. Updates to readmes and meta documents
- **docs**: Changes to the automated documentation or TSDoc comments
- **feat**: A new feature
- **fix**: A bug fix
- **refactor**: A code change that neither fixes a bug nor adds a feature
- **style**: Changes that do not affect the meaning of the code (white-space, formatting, missing semi-colons, etc)
- **test**: Adding missing tests or correcting existing tests
- **sample**: A change to the samples

#### <a name="pull"></a>Submitting a Pull Request

After searching for potentially existing pull requests or issues in progress, if none are found, please open a new issue describing your intended changes and stating your intention to work on the issue.

Creating issues helps us plan our next release and prevents folks from duplicating work.

After the issue has been created, follow these steps to create a Pull Request.

1. Fork the corresponding CircleCI Public repo.
1. Clone your newly forked repository to your local machine.
1. Create a new branch for your changes: `git checkout -b fix_my_issue main`
1. Run any initialization steps, like: `npm run setup`
1. Implement your change with appropriate test coverage.
1. Utilize our [commit message conventions](#commit).
1. Run tests, linters, and formatters locally, with the appropriate command, like: `npm run prep`
1. Push all changes back to GitHub: `git push origin fix_my_issue`
1. In GitHub, send a Pull Request to the main branch of the repo, like: `circleci-config-sdk-ts:main`

Thank you for your contribution!

##### After Your PR Has Been Merged

After your pull request is merged, you can safely delete your branch and pull the changes from the main (upstream) repository:

- Delete the remote branch on GitHub either through the GitHub web UI or your local shell as follows:

  ```shell
  git push origin --delete fix_my_issue
  ```

- Check out the main branch:

  ```shell
  git checkout main -f
  ```

- Delete the local branch:

  ```shell
  git branch -D fix_my_issue
  ```

- Update your main with the latest upstream version:

  ```shell
  git pull --ff upstream main
  ```

#### <a name="release"></a>How To Issue a Release

Releases are handled by maintainers only, and each specific repo will have the steps to follow.

## Code of Conduct

All community members are expected to adhere to our [Code of Conduct](https://raw.githubusercontent.com/CircleCI-Public/.github/main/CODE_OF_CONDUCT.md).