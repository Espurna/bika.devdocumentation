-----------------------------------------------
Configuring a Bika LIMS development environment
-----------------------------------------------

Steps to configuring a Bika LIMS development environment

    1) Install Plone and Bika LIMS

       Follow the `Bika-LIMS installation instructions.`_

    2) Install and configure git

       Follow these steps: `Github: Set Up Git <https://help.github.com/articles/set-up-git/>`_.

    3) Fork and Clone the Bika-LIMS sources

       Follow the instructions at `Github: Fork A Repo <https://help.github.com/articles/fork-a-repo/>`_.
       
       .. note::

	  When you clone the new fork that you have created, you should place it in the src/ directory inside your Plone installation.
	  By default, the directory name of the new clone will be that of the repository, but this is not required.

    4) Configure Buildout

       You must edit buildout.cfg. You will need to add or edit the "develop = " statement in the [buildout] section, to include the folder that contains the forked source.

       .. code-block:: rest

	  develop =
	      src/Bika-LIMS

       .. note::

	  Remember to run bin/buildout again.

    6) Next steps

       Join the bika-developers list at http://lists.sourceforge.net/lists/listinfo/bika-developers, and the IRC channel at irc.freenode.net/#bika immediately. We will be happy to help you acheive the highest code quality with your customisation project.

       Read the excellent `Plone developer documentation <http://docs.plone.org/develop/index.html>`_.


