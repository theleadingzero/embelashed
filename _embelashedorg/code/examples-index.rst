Pure Data Examples
##################
It's always easier to modify or edit than to start with a blank page, so this is a collection of Pure Data examples that provide some simple interaction and functionality.


All examples can be found in the `pure-data-bela-tutorials Github repository <https://github.com/theleadingzero/pure-data-bela-tutorials>`_, in the folder ``examples``.


Installation
************
To run the example patches in Pure Data on your computer, add the path of the ``abstractions`` folder to Pure Data through the ``Pd -> Preferences -> Path...`` menu. You then will need to quit restart Pure Data.

To run on a Bela board:

* `either` copy the needed abstractions to the local project folder, 
* `or` ``scp`` the abstractions folder to ``~/Bela/Projects/pd-externals/``;
* `or` in the IDE, create a new project called ``pd-externals`` and upload the ``.pd`` files in the ``abstractions`` folder to the project. If a project with that name already exists, just upload the abstractions to that project.

Then create a new Pd project in the Bela IDE and upload the contents of the example project folder - this always includes a ``_main.pd`` and may includes some additional files.


Overview of Examples
********************
Examples 01 through 04 are to be run on a laptop, not on Bela. However, note that you need to install the abstractions with Pure Data using the above instructins. All other examples are intended for running on Bela.

The examples roughly build on each other and become more complex as their starting number increases. Most need at least one sensor attached to Bela. All only use either the Bela scope and/or audio as the sole output, no other actuation like LEDs or motors are used. It is entirely possible to add them yourself.