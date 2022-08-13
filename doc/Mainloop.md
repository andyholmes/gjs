# Mainloop

The `Mainloop` module is a deprecated convenience layer for some common event
loop methods in GLib, such as [`GLib.timeout_add()`][gtimeoutadd].

This module is no longer recommended, but is documented to help port old code to
standard GLib methods. Each method below contains links to the corresponding
GLib method.

For an introduction to the GLib event loop, see the
[Asynchronous Programming Tutorial][].

[gtimeoutadd]: https://gjs-docs.gnome.org/glib20/glib.timeout_add

#### Import

> Attention: This module is not available as an ECMAScript Module

The `Mainloop` module is available on the global `imports` object:

```js
const Mainloop = imports.mainloop
```

### Mainloop.idle_add(handler, priority)

> Deprecated: Use [`GLib.idle_add()`][gidleadd] instead

Type:
* Static

Parameters:
* handler (`Function`) — The function to call
* priority (`Number`) — Optional priority

Returns:
* (`GLib.Source`) — The newly-created idle source

Adds a function to be called whenever there are no higher priority events
pending. If the function returns `false` it is automatically removed from the
list of event sources and will not be called again.

If not given, `priority` defaults to `GLib.PRIORITY_DEFAULT_IDLE`.

[gidleadd]: https://gjs-docs.gnome.org/glib20/glib.idle_add

### Mainloop.idle_source(handler, priority)

> Deprecated: Use [`GLib.idle_source_new()`][gidlesourcenew] instead

Type:
* Static

Parameters:
* handler (`Function`) — The function to call
* priority (`Number`) — Optional priority

Returns:
* (`GLib.Source`) — The newly-created idle source

Creates a new idle source.

If not given, `priority` defaults to `GLib.PRIORITY_DEFAULT_IDLE`.

[gidlesourcenew]: https://gjs-docs.gnome.org/glib20/glib.idle_source_new

### Mainloop.quit(name)

> Deprecated: Use [`GLib.MainLoop.quit()`][gmainloopquit] instead

Type:
* Static

Parameters:
* name (`String`) — Optional name

Stops a main loop from running. Any calls to `Mainloop.run(name)` for the loop
will return.

If `name` is given, this function will create a new [`GLib.MainLoop`][gmainloop]
if necessary.

[gmainloop]: https://gjs-docs.gnome.org/glib20/glib.mainloop
[gmainloopquit]: https://gjs-docs.gnome.org/glib20/glib.mainloop#method-quit

### Mainloop.run(name)

> Deprecated: Use [`GLib.MainLoop.run()`][gmainlooprun] instead

Type:
* Static

Parameters:
* name (`String`) — Optional name

Runs a main loop until `Mainloop.quit()` is called on the loop.

If `name` is given, this function will create a new [`GLib.MainLoop`][gmainloop]
if necessary.

[gmainloop]: https://gjs-docs.gnome.org/glib20/glib.mainloop
[gmainlooprun]: https://gjs-docs.gnome.org/glib20/glib.mainloop#method-run

### Mainloop.source_remove(id)

> Deprecated: Use [`GLib.Source.remove()`][gsourceremove] instead

Type:
* Static

Parameters:
* id (`Number`) — The ID of the source to remove

Returns:
* (`Boolean`) — For historical reasons, this function always returns `true`

Removes the source with the given ID from the default main context.

[gsourceremove]: https://gjs-docs.gnome.org/glib20/glib.source#function-remove

### Mainloop.timeout_add(timeout, handler, priority)

> Deprecated: Use [`GLib.timeout_add()`][gtimeoutadd] instead

Type:
* Static

Parameters:
* timeout (`Number`) — The timeout interval in milliseconds
* handler (`Function`) — The function to call
* priority (`Number`) — Optional priority

Returns:
* (`GLib.Source`) — The newly-created timeout source

Sets a function to be called at regular intervals, with the given priority. The
function is called repeatedly until it returns `false`, at which point the
timeout is automatically destroyed and the function will not be called again.

The scheduling granularity/accuracy of this source will be in milliseconds. If
not given, `priority` defaults to `GLib.PRIORITY_DEFAULT`.

[gtimeoutadd]: https://gjs-docs.gnome.org/glib20/glib.timeout_add

### Mainloop.timeout_add_seconds(timeout, handler, priority)

> Deprecated: Use [`GLib.timeout_add_seconds()`][gtimeoutaddseconds] instead

Type:
* Static

Parameters:
* timeout (`Number`) — The timeout interval in seconds
* handler (`Function`) — The function to call
* priority (`Number`) — Optional priority

Returns:
* (`GLib.Source`) — The newly-created timeout source

Sets a function to be called at regular intervals, with the given priority. The
function is called repeatedly until it returns `false`, at which point the
timeout is automatically destroyed and the function will not be called again.

The scheduling granularity/accuracy of this source will be in seconds. If not
given, `priority` defaults to `GLib.PRIORITY_DEFAULT`.

[gtimeoutaddseconds]: https://gjs-docs.gnome.org/glib20/glib.timeout_add_seconds

### Mainloop.timeout_source(timeout, handler, priority)

> Deprecated: Use [`GLib.timeout_source_new()`][gtimeoutsourcenew] instead

Type:
* Static

Parameters:
* timeout (`Number`) — The timeout interval in milliseconds
* handler (`Function`) — The function to call
* priority (`Number`) — Optional priority

Returns:
* (`GLib.Source`) — The newly-created timeout source

Creates a new timeout source.

The scheduling granularity/accuracy of this source will be in milliseconds. If
not given, `priority` defaults to `GLib.PRIORITY_DEFAULT`.

[gtimeoutadd]: https://gjs-docs.gnome.org/glib20/glib.timeout_source_new

### Mainloop.timeout_seconds_source(timeout, handler, priority)

> Deprecated: Use [`GLib.timeout_source_new_seconds()`][gtimeoutsourcenewseconds]
> instead

Type:
* Static

Parameters:
* timeout (`Number`) — The timeout interval in seconds
* handler (`Function`) — The function to call
* priority (`Number`) — Optional priority

Returns:
* (`GLib.Source`) — The newly-created timeout source

Creates a new timeout source.

The scheduling granularity/accuracy of this source will be in seconds. If not
given, `priority` defaults to `GLib.PRIORITY_DEFAULT`.

[gtimeoutsourcenewseconds]: https://gjs-docs.gnome.org/glib20/glib.timeout_source_new_seconds

