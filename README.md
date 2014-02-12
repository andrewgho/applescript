applescript - AppleScript utilities
===================================

This repository contains AppleScript utilities meant for running from
the command line (via the `osascript` command line utility in OS X).
In particular, the utilities are meant for UI scripting: reflecting on
and affecting the positions and sizes of windows.

Scripts
-------

`lswin` lists the application name, window title, position, and size of
every window open in the current space. You can optionally provide a
pattern substring that matches the `Application Name - Window Title`
output to restrict the windows that are listed.

`movewin` takes a pattern substring, X and Y coordinates for new window
position, and optionally a width and height in pixels. It moves the
first window that matches the pattern to the new location specified, and
also resizes it if the width and height are supplied.

`displaysize` prints the width and height of the current display (or
aggregate display, in the case of multiple monitors) in pixels.

`ctrl` is a simple command line utility which emits a given keystroke
with the `Ctrl` key modifier enabled. This is useful for switching to
different Mission Control spaces.

Prerequisites
-------------

All the scripts except for `displaysize` require the "Enable access for
assistive devices" setting to be enabled in the "Accessibility" System
Preferences pane in OS X pre-Mavericks. To enable assistive UI scripting
in Mavericks, see this Apple KB article:
[http://support.apple.com/kb/HT5914](http://support.apple.com/kb/HT5914)

Author
------

Andrew Ho (<andrew@zeuscat.com>)

License
-------

    Copyright (c) 2013-2014, Andrew Ho
    All rights reserved.
    
    Redistribution and use in source and binary forms, with or without
    modification, are permitted provided that the following conditions
    are met:
    
    1. Redistributions of source code must retain the above copyright
       notice, this list of conditions and the following disclaimer.
    
    2. Redistributions in binary form must reproduce the above copyright
       notice, this list of conditions and the following disclaimer in the
       documentation and/or other materials provided with the distribution.
    
    3. Neither the name of Andrew Ho nor the names of its contributors may
       be used to endorse or promote products derived from this software
       without specific prior written permission.
    
    THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS
    IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED
    TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
    PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT
    HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
    SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED
    TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
    PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
    LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
    NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
    SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
