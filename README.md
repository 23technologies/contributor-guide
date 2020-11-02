# 23 Technologies Contributor Guide

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
for more details.

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
