# My Emacs Configuration

This is my Emacs configuration. It's been written and rewritten and
refactored and migrated and changed and updated since the late '90s.

I keep this setup in git because I like to keep it up to date across
all the computers I use — work laptop, home workstation, home laptop,
development servers, etc.

A lot of this stuff is pretty specific to my personal needs, but feel
free to steal ideas.

## Structure

My Emacs configuration is kept in *Literate Configuration* style.
This means that my configuration is a human-readable document that
puts comments first, and embeds the actual configuration elisp as code
snippets.

The main file is called [configuration.org](configuration.org), and
is in `org-mode` format.

Files found in `~/.emacs.d/local` are ignore by Git, but added to
the load path.

Files found in `~/.emacs.d/lisp` are checked into Git, and added to
the load path.

## Getting Started

The process for bootstrapping all this stuff is complicated
a little bit by the fact that I use the latest `org-mode`
as a Git submodule. The full process for getting everything running
is as follows:

### Clone the Repository

    $ git clone git@github.com:sethm/emacs-files.git ~/.emacs.d

### Update the `org-mode` and `tera-mode` submodules

    $ cd ~/.emacs.d
    $ git submodule init
    $ git submodule update

### Build `org-mode`

    $ cd ~/.emacs.d/org-mode
    $ make

## License

Copyright 1995–2020, Seth J. Morabito &lt;web@loomcom.com&gt;

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT,
TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE
SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
