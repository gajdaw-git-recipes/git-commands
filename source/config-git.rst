Config git
==========

Basic git config in the classroom.


Set password's caching:

.. code-block::
    $ git config --global credential.helper wincred


Set the configuration for line-endings:

.. code-block::
    $ git config --global core.autocrlf input


Set pushing branches:

.. code-block::
    $git config --global push.defaults current


Set your name and email:

.. code-block::
    git config --global user.email student@example.net
    git config --global user.name "Mr. Student"


Install the aliases:

.. code-block::
    git clone https://github.com/gajdaw-git-recipes/aliases.git
    cd aliases
    cat aliases.txt >> ~/.gitconfig


