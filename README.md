ParCook
-------

ParCook is a plugin for less meant to partially compile LESS and CSS to LESS, filling in variables, resolving paths, optimizing nesting, and formatting the output for readability, or crunching it for bandwidth.

ParCook is meant to be used where the server can't know all the stylesheets, variables, and functions that will be used in the final site, but you want to be able to collect, optimize, and minify your stylesheet, rather than creating a suite of requests for your highly modularized base LESS.

Expect an alpha version of ParCook to show up some time in July 2015.  There's a lot to do, and I'm just getting started.

Roadmap:
--------

* a0 (July): Ingest a LESS or CSS file, parse it to an AST using LESS' internals, and output LESS with only formatting changes.
* a1 (September): Same, but with variable and function resolution where variables and functions exist.
* a2 (November): Scan AST for repeating patterns of rules, and create functions or nests where most optimal to do so
* b0, b1, b2 (December): bugfixes
* 1.0 (Januray 2016): First release

Long term goals:
----------------

* Parse LESS/SASS/SCSS to common AST, and compile to any of these targets
* Compile LESS to pure Javascript
* Define simplified JSON-based aCSS AST spec for inclusion into Ember/Angular/Backbone/etc components
