Open problems
=============


How to merge a branch automatically when there are
conflicts that are stored by rerere?
When new conflicts are discovered the operation should be
interrupted.


Use:

    git rerere remaining


------------------------------------------------------------------------

Clone only one commit from a given branch:


    git clone --depth 1 --branch 2.6 --single-branch https://github.com/symfony/symfony-standard.git

The parameter --single-branch is not necessary:

    DOC:

        --single-branch
        Clone only the history leading to the tip of a single branch,
        either specified by the --branch option or the primary branch
        remote’s HEAD points at. When creating a shallow clone with the
        --depth option, this is the default, unless --no-single-branch
        is given to fetch the histories near the tips of all branches.


    git clone --depth 1 --branch 2.6 https://github.com/symfony/symfony-standard.git



How to clone only one commit with a given tag?

    DOC:

     --branch can also take tags and detaches the HEAD at that commit in the resulting repository.


    git clone --depth 1 --branch v2.6.1 https://github.com/symfony/symfony-standard.git



------------------------------------------------------------------------

Update submodules:


During the clone:

git clone --recursive [URL]

After the clone:

git submodule update --init --recursive

------------------------------------------------------------------------

Avoiding problems with:   /bin/bash^M not found when working in
Vagrant/Windows:

Bash scripts have to user lf always.

.gitattritubes

*.bash     eol=lf
script.sh  eol=lf

