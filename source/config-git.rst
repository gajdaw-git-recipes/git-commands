Config git
==========

Basic git config in the classroom.


Set password's caching:

::

    $ git config --global credential.helper wincred


Set the configuration for line-endings:

::

    $ git config --global core.autocrlf input


Set pushing branches:

::

    $git config --global push.defaults current


Set your name and email:

::

    git config --global user.email student@example.net
    git config --global user.name "Mr. Student"


Install the aliases:

::

    git clone https://github.com/gajdaw-git-recipes/aliases.git
    cd aliases
    cat aliases.txt >> ~/.gitconfig


