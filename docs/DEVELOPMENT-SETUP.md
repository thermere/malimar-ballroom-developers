# Development setup

## What you can do today

The application source is private, so there is no application code to clone or run from this repository yet. Today you can:

1. **Read the documentation.** Start with [VISION.md](VISION.md) and [ARCHITECTURE.md](ARCHITECTURE.md).
2. **Try the public website.** The front page plays a recorded introduction. The conversation room is not open on the public website.
3. **Report a problem** with the public website or with these documents. Use the issue templates in this repository.
4. **Suggest an improvement.** Open a feature request, and say how it fits the principles in [VISION.md](VISION.md).
5. **Fix or improve a document.** Follow the steps below.

## Changing a document

You need Git and a GitHub account. Nothing else is installed.

1. Fork this repository on GitHub.
2. Clone your fork and create a branch.

   ```text
   git clone <the address of your fork>
   cd malimar-ballroom-developers
   git switch -c your-branch-name
   ```

3. Make one focused change. Keep every statement accurate: a plan must be labelled as a plan.
4. Commit, push the branch to your fork, and open a pull request against `main`.
5. Say in the pull request what you changed and how you checked it.

A maintainer reviews every pull request before it is merged. Contributors do not get write access to protected branches.

## When source code is shared

Approved application components will be published here with their own setup steps, tests and review rules. This page will then list the exact commands. Until then, no commands are listed, so that nothing here describes code you cannot see.

## Keep these out of issues and pull requests

- Keys, tokens, signed links and passwords.
- Personal data, and real legal, medical or financial matters.
- Details of a security problem. Follow [SECURITY.md](../SECURITY.md) instead.
