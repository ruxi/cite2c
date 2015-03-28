Live citations in IPython notebooks

![screenshot](search_screenshot.png)

To install this, run `python install.py` with the same Python that IPython is
installed in. It requires IPython 3.x, which is not yet released - you can
[install a development version](https://github.com/ipython/ipython/#development-installation)
from GitHub.

You will see two new toolbar buttons: ![toolbar buttons](toolbar_buttons.png).
The left one inserts a citation at the current point in a Markdown cell.
The right one inserts a bibliography.

This extension has two main components:
- UI for finding citations from a Zotero library and inserting them into Markdown cells.
  The citations are stored in the notebook metadata, and referenced by an ID.
- Code to run [citeproc-js](https://bitbucket.org/fbennett/citeproc-js/wiki/Home) when a Markdown cell is rendered, rendering both bibliographies and inline citations.

To make your zotero library viewable:
 - navigate to [privacy settings](https://www.zotero.org/settings/privacy) and tick 'Publish entire library'
