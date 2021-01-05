# 23 Technologies Contributor Guide

## The Four Opens

We stand behind [the four opens](https://governance.openstack.org/tc/reference/opens.html)
of the [Open Infrastructure Foundation](https://osf.dev).

* Open Source
* Open Design
* Open Development
* Open Community

## Developer Certificate of Origin

The [Developer Certificate of Origin](https://developercertificate.org) (DCO)
is a lightweight way for contributors to certify that they wrote or otherwise
have the right to submit the code they are contributing to the projects of
[23 Technologies](https://23technologies.cloud).

```
Developer Certificate of Origin
Version 1.1

Copyright (C) 2004, 2006 The Linux Foundation and its contributors.
1 Letterman Drive
Suite D4700
San Francisco, CA, 94129

Everyone is permitted to copy and distribute verbatim copies of this
license document, but changing it is not allowed.

Developer's Certificate of Origin 1.1

By making a contribution to this project, I certify that:

(a) The contribution was created in whole or in part by me and I
    have the right to submit it under the open source license
    indicated in the file; or

(b) The contribution is based upon previous work that, to the best
    of my knowledge, is covered under an appropriate open source
    license and I have the right under that license to submit that
    work with modifications, whether created in whole or in part
    by me, under the same open source license (unless I am
    permitted to submit under a different license), as indicated
    in the file; or

(c) The contribution was provided directly to me by some other
    person who certified (a), (b) or (c) and I have not modified
    it.

(d) I understand and agree that this project and the contribution
    are public and that a record of the contribution (including all
    personal information I submit with it, including my sign-off) is
    maintained indefinitely and may be redistributed consistent with
    this project or the open source license(s) involved.
```

## Sign-off commits

The following content is [taken from the Pi-Hole project](https://github.com/pi-hole/docs/blob/master/docs/guides/github/how-to-signoff.md).
There you can also find more details about the used Git commands.

23 Technologies requires a sign-off message in the following format appear on each commit in the pull request:

```
This is my commit message

Signed-off-by: Random Developer <random@23technologies.xyz>
```

The text can either be manually added to your commit body, or you can add
either ``-s`` or a ``--signoff`` to your usual Git commit commands.

## Licenses

We use the ASL 2.0 and the CC-BY-SA 4.0.

## Commit messages

For the commit messages we follow the [best practices from the OpenStack project](https://wiki.openstack.org/wiki/GitCommitMessages).
Please read the [best practices](https://wiki.openstack.org/wiki/GitCommitMessages) completely. The following is an excerpt.

* Provide a brief description of the change in the first line.
* Insert a single blank line after the first line.
* Provide a detailed description of the change in the following lines, breaking paragraphs where needed.
* The first line should be limited to 50 characters and should not end with a period.
* Subsequent lines should be wrapped at 72 characters.

## Collaborating with issues and pull requests

We use the GitHub flow to track and discuss changes in issues, then propose and
review changes in pull requests. See the
[GitHub documentation](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests)
for more details. The main-branch is considered to be a stable and working base.
When a new feature/bug/enhancement is developed, a new branch should be created from the
main branch. After all necessary changes are commited, the branch can be suggested for a merge
via a GitHub pull request.

## Pull request labels

We use the GitHub action [PR Labeler](https://github.com/marketplace/actions/pr-labeler)
to automatically label new pull requests.

```
---
'Type: Bugfix': ['fix/*', 'issue/*']
'Type: Build': build/*
'Type: CI': ['ci/*', 'travis/*', 'zuul/*']
'Type: Documentation': ['docs/*', 'doc/*', 'documentation/*']
'Type: Feature': ['feature/*', 'feat/*']
'Type: Maintenance': ['chore/*', 'renovate/*']
'Type: Refactoring': ['refactor/*', 'refactoring/*']
'Type: Release': release/*
'Type: Style': style/*
'Type: Testing': ['test/*', 'testing/*']
```

Then if a pull request is opened with the branch name ``bugfix/218-testing`` the action
will automatically apply the ``Type: Bugfix`` label.

## Use of the terms "master" and "slave"

Master and slave are politically incorrect terms. We do not use the terms ``master`` and
``slave`` anywhere. Instead of ``master`` terms like ``main`` or ``primary`` are
used. Instead of ``slave`` terms like ``secondary``, ``minion`` or ``worker`` are used.

On GitHub, ``master`` is still used as the primary branch until the end of the year.

By the end of 2020, GitHub will have a feature that allows you to rename the ``master``
branch to ``main``. See https://github.com/github/renaming for more details.

If at any point (except for the name of the primary branch until the end of 2020) the term
``master`` or ``slave`` is found in one of our repositories or documents, please let us know.
