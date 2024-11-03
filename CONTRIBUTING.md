# BioHackCloud contributor guide

<!-- TOC start (generated with https://github.com/derlin/bitdowntoc) -->

* [Basic workflow](#basic-workflow)
* [Your issue isn't there? Open one!](#your-issue-isnt-there-open-one)
* [Proposing changes to GitHub projects](#proposing-changes-to-github-projects)
* [Issues not involving changes to GitHub projects](#issues-not-involving-changes-to-github-projects)

<!-- TOC end -->

<!-- TOC --><a name="basic-workflow"></a>
## Basic workflow

To start contributing, please follow these simple steps:

1. Join [GitHub][github-join].
2. Share your GitHub handle with us by filling in the [contributor info
   form][bh-contributor-form].
2. Check out our [hackathon project board][bh-project-board] to see the
   available issues to work on.
4. After we have added you to the [ELIXIR Cloud & AAI GitHub
   organization][elixir-cloud-aai-github], assign yourself to an issue you
   would like to work on.
6. Please carefully read the guidelines below.
7. Start hacking! :computer:

<!-- TOC --><a name="your-issue-isnt-there-open-one"></a>
## Your issue isn't there? Open one!

If you want to work on something for which no issue exists yet, please [open
an issue first][bh-new-issue]. Please use the default issue template and
follow the instructions. In particular, please label your issue appropriately
and associate it with the "BioHackathon Europe '24" project board.

<!-- TOC --><a name="proposing-changes-to-github-projects"></a>
## Proposing changes to GitHub projects

Many issues require proposing changes to projects on GitHub. In such cases,
please make sure to check the project you are contributing to for specific
contributing guidelines. If nothing else is mentioned, we are using the
[GitHub flow][github-flow]:

1. From a local clone of the repository (not a fork!), [**create a
   "feature branch"**][git-branch] from the default branch; make sure the
   default [branch is up to date][git-pull] before creating the new branch
2. [**Commit** code changes][git-commit] to address the issue you are working
   on; make sure to provide or adapt any relevant tests and documentation
3. [**Push** the feature branch][git-push] to the remote and [**create a pull
   request**][github-pr] against the default branch in GitHub; for your PR
   title, please follow the rules outlined [below](#how-to-name-pull-requests);
   make sure to succinctly describe your changes in the PR description
4. **Request reviews** from one or more other contributors (e.g., the
   subproject lead for your issue); if necessary, you can address reviewer
   comments by reviewers by pushing additional commits to your feature branch
5. Once all issues are resolved, code owners will merge the feature branch into
   the default branch using the ["squash merging"][github-merge-squash]
   method, i.e., all individual commits in your feature branch will be merged
   into a single commit

> **Please keep pull requests as small as possible!** Address one thing at a
> time, as per the issue you are working on. If you feel that the changes are
> getting too subtantial, consider breaking up the issue into smaller chunks.
> However, each pull request should always include the necessary test and
> documentation changes corresponding to the issue you are working on.

### How to name pull requests

No specific formatting of individual commit messages is required when working
on _feature branches_. However, your **pull request titles** should follow
the [Conventional Commits specification][conv-commits]** - as these will be
used as the commit messages when squash merging your feature branches into
the default branch.

The general format for PR titles is as follows:

```console
<type>(optional scope): <description>
```

Please also follow these rules:

- Keep your entire header/title line (including type and, if available, scope)
  at **50 characters or less**
- Only use the types listed in the table below; choose the type according to the
  predominant reason for the change
- Start the `<description>` with a verb in imperative form (e.g., `add`, `fix`)

Available types:

| Type | Description |
| --- | --- |
| build | For changes related to the build system (e.g., scripts, configurations and tools) and package dependencies |
| chore | For changes related to mundane repository maintenance tasks that are not covered by any of the other types (e.g., adding a `.gitignore file) | 
| ci | For changes related to the continuous integration and deployment system (e.g., workflows, scripts, configurations and tools) |
| docs | For changes related to the project documentation, regardless of the audience (end users, developers) |
| feat | For changes related to new abilities or functionality |
| fix | For changes related to bug fixes |
| perf | For changes related to performance improvements |
| refactor | For changes related to modifying the codebase, which neither adds a feature nor fixes a bug (e.g., removing redundant code, simplifying code, renaming variables) |
| revert | For changes that revert one or more previous commits |
| style | For changes related to styling the codebase (e.g., indentation, parentheses/brackets, white space, trailing commas) |
| test | For changes related to tests |

<!-- TOC --><a name="issues-not-involving-changes-to-github-projects"></a>
## Issues not involving changes to GitHub projects

If your issue does not involve changes to GitHub repositories, check its
description for details on desired/expected outcomes. If nothing else is
mentioned, report the outcome as comments to the issue, either:

* directly via markdown and/or attaching files, or
* indirectly via references

> When using references, please make sure that the referenced documents
> are publicly accessible.

[bh-contributor-form]: <https://forms.gle/5bcA5V7Vfz4miiNx8>
[bh-new-issue]: <https://github.com/elixir-cloud-aai/biohackeu24-issues/issues/new/choose>
[bh-project-board]: <https://github.com/orgs/elixir-cloud-aai/projects/23>
[conv-commits]: <https://www.conventionalcommits.org/en/v1.0.0-beta.2/#specification>
[elixir-cloud-aai-github]: <https://github.com/elixir-cloud-aai/>
[git-branch]: <https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging>
[git-commit]: <https://git-scm.com/docs/git-commit>
[git-pull]: <https://git-scm.com/docs/git-pull>
[git-push]: <https://git-scm.com/docs/git-push>
[github-flow]: <https://docs.github.com/en/get-started/quickstart/github-flow>
[github-join]: <https://github.com/join>
[github-merge-squash]: <https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/incorporating-changes-from-a-pull-request/about-pull-request-merges#squash-and-merge-your-commits>
[github-pr]: <https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request>
