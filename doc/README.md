# GJS

GJS is JavaScript bindings for the GNOME platform APIs.

## Documentation

If you are reading this file in the GJS repository, you may find it more
convenient to browse and search in our [DevDocs][gjs-docs] instance instead.

To find out when a JavaScript language feature was implemented in GJS, review
the [NEWS](https://gitlab.gnome.org/GNOME/gjs/raw/HEAD/NEWS) file in the GitLab
repository.

There are also a growing number of [code examples][gjs-examples] and thorough
tests of language features in the [GJS test suite][gjs-tests].

Finally, there is a community maintained website at [gjs.guide][gjs-guide] with
many in-depth tutorials and usage examples for a number of core GNOME APIs.

[gjs-docs]: https://gjs-docs.gnome.org/
[gjs-examples]: https://gitlab.gnome.org/GNOME/gjs/tree/HEAD/examples
[gjs-tests]: https://gitlab.gnome.org/GNOME/gjs/blob/HEAD/installed-tests/js
[gjs-guide]: https://gjs.guide

## Applications

GJS can be used to write stand-alone applications.

GNOME Applications written in GJS:

* [GNOME Characters](https://gitlab.gnome.org/GNOME/gnome-characters)
* [GNOME Documents](https://gitlab.gnome.org/GNOME/gnome-documents)
* [GNOME Maps](https://gitlab.gnome.org/GNOME/gnome-maps)
* [GNOME Sound Recorder](https://gitlab.gnome.org/GNOME/gnome-sound-recorder)
* [GNOME Weather](https://gitlab.gnome.org/GNOME/gnome-weather)
* [GNOME Books](https://gitlab.gnome.org/GNOME/gnome-books)
* [Polari](https://gitlab.gnome.org/GNOME/polari) IRC Client

Third party applications written in GJS:

* [Tangram](https://github.com/sonnyp/Tangram)
* [Quick Lookup](https://github.com/johnfactotum/quick-lookup)
* [Foliate](https://github.com/johnfactotum/foliate)
* [Marker](https://github.com/fabiocolacio/Marker)
* [Gnomit](https://github.com/small-tech/gnomit)
* [Clapper](https://github.com/Rafostar/clapper/)
* [Flatseal](https://github.com/tchx84/Flatseal)
* [Almond](https://github.com/stanford-oval/almond-gnome/)
* [Commit](https://github.com/sonnyp/commit/)
* [Junction](https://github.com/sonnyp/Junction)
* [Oh My SVG](https://github.com/sonnyp/OhMySVG)

### GNOME Shell Extensions

GJS is used to write [GNOME Shell Extensions](https://extensions.gnome.org),
allowing anyone to make considerable modifications to the GNOME desktop. This
can also be a convenient way to prototype changes you may want to contribute to
the upstream GNOME Shell project.

There is documentation and tutorials specifically for extension authors at
[gjs.guide/extensions](https://gjs.guide/extensions).

### Embedding GJS

GJS can also be embedded in other applications, such as with GNOME Shell,
providing a powerful scripting language with support for the full range of
libraries that support GObject-Introspection.

## Getting Help

* Discourse: https://discourse.gnome.org/
* Chat: https://matrix.to/#/#javascript:gnome.org
* Issue Tracker: https://gitlab.gnome.org/GNOME/gjs/issues
* StackOverflow: https://stackoverflow.com/questions/tagged/gjs

## See Also

* [GObject-Introspection](https://gitlab.gnome.org/GNOME/gobject-introspection)
* [GNOME Shell Extensions](https://gjs.guide/extensions)

