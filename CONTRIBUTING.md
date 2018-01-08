Contributing to librsvg
=======================

Thank you for looking in this file!  There are different ways of
contributing to librsvg, and we appreciate all of them.

* [Source repository](#source-code)
* [Reporting bugs](#reporting-bugs)
* [Feature requests](#feature-requests)
* [Pull requests](#pull-requests)

There is a **code of conduct** for contributors to librsvg; please see the
file [`code_of_conduct.md`][coc].

## Source repository

Librsvg's main source repository is at gitlab.gnome.org.  You can view
the web interface here:

https://gitlab.gnome.org/GNOME/librsvg

Development happens in the master branch.  There are also branches for
stable releases.

Alternatively, you can use the mirror at Github:

https://github.com/GNOME/librsvg

Note that we don't do bug tracking in the Github mirror; see the next
section.

If you need to publish a branch, feel free to do it at any
publically-accessible Git hosting service, although gitlab.gnome.org
makes things easier for the maintainers of librsvg.

## Reporting bugs

Please report bugs at https://gitlab.gnome.org/GNOME/librsvg/issues

If you want to report a rendering bug, or a missing SVG feature,
please provide an example SVG file as an attachment to your bug
report.  It really helps if you can minimize the SVG to only the
elements required to reproduce the bug or see the missing feature, but
it is not absolutely required.  **Please be careful** of publishing
SVG images that you don't want other people to see, or images whose
copyright does not allow redistribution; the bug tracker is a public
resource and attachments are visible to everyone.

You can also [browse the existing bugs][bugs-browse].

## Feature requests

Librsvg aims to be a small and relatively simple SVG rendering
library.  Currently we do not plan to support scripting, animation, or
interactive features like mouse events on SVG elements.

However, we *do* aim go provide good support for SVG's graphical
features.  Please see the "[reporting bugs](#reporting-bugs)" section for
information about our bug tracking system; feature requests should be
directed there.

It is especially helpful if you file bug for a feature request along
with a sample SVG file.

## Merge requests / pull requests

You may created a forked version of librsvg in [GNOME's Gitlab
instance][gitlab], or any other publically-accesible Git hosting
service.  You can register an account there, or log in with your
account from other OAuth services.

Note that the maintainers of librsvg only get notified about merge
requests (or pull requests) if your fork is in
[gitlab.gnome.org][gitlab].

For technical reasons, the maintainers of librsvg do not get
automatically notified if you submit a pull request through the GNOME
mirror in Github.  [Please mail the maintainer][mail] directly if you
have a pull request there or a branch that you would like to
contribute.

**Test suite:** Please make sure that the test suite passes with the
changes in your branch.  The easiest way to run all the tests is to go
to librsvg's toplevel directory and run `make check`.  This will run
both the small unit tests and the black box tests in the
`librsvg/tests` directory.

If you need to add new tests (you should, for new features, or for
things that we weren't testing!), or for additional information on how
the test suite works, please see the file [`tests/README.md`][tests-readme].

[coc]: code_of_conduct.md
[gitlab]: https://gitlab.gnome.org/GNOME/librsvg
[bugs-browse]: https://gitlab.gnome.org/GNOME/librsvg/issues
[mail]: mailto:federico@gnome.org
[tests-readme]: tests/README.md