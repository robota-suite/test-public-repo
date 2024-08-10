# test-public-repo

A repository for acceptance testing of RoboTA Suite packages.

The RoboTA Suite provides tools for platform agnostic analysis of hosted Git projects.

This repository gives an example hosted project for acceptance testing purposes.

An identical copy of the repository should be maintained on all Git project hosting sites
that are supported by RoboTA Suite.  This can be done by:

1. Cloning the GitHub version of this project.
1. Adding extra remotes for all other hosted platforms.
1. When changes are made to the repository, push them to all remotes.

For example, to add the remote for the GitLab.com hosted test project, you can use:

    git remote add gitlab git@gitlab.com:robota-suite/test-public-repo.git

Then make sure to push to both the `origin` and `gitlab` remotes.

(You can also make a single remote with multiple URLs using
`git remote set-url --add` if you prefer.  As long as identical commits and references
are pushed to all the test repos, we're good.)

Ideally, the project should have the same group/organisation name and project/repository
name on all hosted platforms.  Only the initial part of the URL should change, to
reflect the different providers.

Maintaining identical copies of the repositories (at least as far as content is concerned)
we hope to facilitate cross-platform testing, requiring only minimal configuration of a
test to the specific platform.  We recognise that this isn't going to be possible for
all project aspects, however.


## Features of the Repository Needed in Testing

Since existing test cases will depend on this repository, RoboTA Suite developers looking
to add features to be used in new test cases should make only additions to the project
and should not delete or change any existing features unless really certain that it will
not cause existing tests to break.

If in doubt, assume that some feature of the project that is here when you come to work
with it is needed for some test case or other.

Please add your new features and a description of what they are needed for to the list
below, for future reference.

* TBA


