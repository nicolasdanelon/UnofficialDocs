===================================
File Navigation and File Management
===================================

Goto Anything
=============

Goto Anything lets you **navigate the filesystem** swiftly. Open it with :kbd:`Ctrl+P`.
As you type into the input area, names of open files and files in open
directories will be searched, and a preview of the best match will be shown.
This preview is *transient*; that is, it won't become the actual active buffer
until you perform some operation on it. Transient views go away when you press
:kbd:`Esc`. You will see transient views in other situations; they are something
like ghosts.

Goto Anything lives up to its name--there's more to it than locating files:

To perform a **fuzzy search**, append ``#`` and then keep typing, like this:

::

	island#treasure

This instructs Sublime Text to perform a fuzzy search for *treasure* in the
file whose name matches *island*. Pressing :kbd:`Ctrl+;` will open Goto
Anything and type the ``#`` for you.

And, there's more:

To **search symbols** in the active buffer, press :kbd:`Ctrl+R`. The operator
``@`` can be used too, as explained above.

To **go to a line number**, press :kbd:`Ctrl+G`. The operator ``:`` can be
used as explained above too.

Searching for symbols will work only with file types that have symbols defined
for them.

Sidebar
=======

The sidebar gives you an overview of your project. Files and folders added to
the sidebar will be available in Goto Anything, and for project-wide actions.
Projects and the sidebar are closely related. There's always an open project,
whether or not it's explicit.

To **open or close** (toggle) the sidebar, press :kbd:`Ctrl+K, Ctrl+B`.

The sidebar can be navigated with the arrow keys, but first you need to give
it the **input focus** by pressing :kbd:`Ctrl+0`. To return input focus to the
buffer, press :kbd:`Esc`. Alternatively, you can use the mouse for the same
effect, but why would you?

The sidebar, through context menus, also provides basic file management
operations.

Projects
========

Projects group together (into a unit) sets of files and directories you need to work on.
Once you've set up your project by adding folders in a way that suits you, save
it and give it a name.

To save a project, go to **Project | Save Project As...**.

To switch among projects quickly, press :kbd:`Ctrl+Alt+P`.

Project data are stored in JSON files with a `.sublime-project` extension.
Wherever there's a `.sublime-project` file, you'll find an ancillary
`.sublime-workspace` file too. The second one is created by Sublime Text and you
shouldn't edit it yourself.

Project files can define settings specific only to that project; there's more
in the `official documentation`_.

.. _official documentation: http://www.sublimetext.com/docs/2/projects.html

You can open a project from the **command line** by passing the *.sublime-
project* file as an argument.

.. TODO: talk about settings related to projects
