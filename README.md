erlang.bootstrap
================

Console utility for bootstrapping Erlang applications.

Requirements
------------

`erlang.bootstrap` requires the `dialog` and `wget` programs
to function, plus the standard unix tool set. On Windows, it
is probably easier to setup using cygwin or setup a Linux VM
to work in.

Usage
-----

Put `erlang.bootstrap` in your `$PATH`, and then call it in
the directory where you want to create your new application.

``` bash
$ erlang.bootstrap
```

A series of dialogs will appear, guiding you towards creating
your application. The application name will be taken from
the current directory, as Erlang/OTP expects it to be the
same.

You can also use it to add modules to an existing application.
If `erlang.bootstrap` finds a `.app.src` file of the same
name as the current folder, it will understand the application
already exists and go directly to the main menu allowing you
to add new modules and perform other common operations.
