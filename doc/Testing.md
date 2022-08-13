# Testing

Testing infrastructure for GJS code is unfortunately not as complete as other
languages, and help in the area would be a greatly appreciated contribution to
the community.

## Jasmine

The [Jasmine][jasmine] testing framework is the recommended method for testing
GJS applications and code, as demonstrated in the [GJS test suite][gjs-tests].

[Jasmine GJS][jasmine-gjs] is a fork of upstream the upstream Jasmine project,
with minor alterations to make it function correctly in a GLib environment. All
features from Jasmine should work as expected, though.

[jasmine]: https://jasmine.github.io/
[jasmine-gjs]: https://github.com/ptomato/jasmine-gjs
[gjs-tests]: https://gitlab.gnome.org/GNOME/gjs/blob/HEAD/installed-tests/js

## jsUnit

> Deprecated: Use Jasmine GJS instead

The `jsUnit` module was originally used as the testing framework in GJS. It has
long been deprecated in favour of Jasmine.

