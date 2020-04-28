st - simple terminal
--------------------

st is a simple terminal emulator for X which sucks less.


Requirements
------------

In order to build st you need the Xlib header files.


Patches included
----------------

- Boxdraw:
    Better box drawing
- Ligatures:
    Supports ligatures (if the font supports them)
- Anysize:
    No weird gaps around st
- Some drop in """headers""" for colorschemes


Installation
------------
Edit config.mk to match your local setup (st is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

    make clean install

Running st
----------
If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

    tic -sx st.info

See the man page for additional details.

Credits
-------
Based on Aurélien APTEL <aurelien dot aptel at gmail dot com> bt source code.

Patch authors:
--------------

Augusto Born de Oliveira - augustoborn@gmail.com (anysize)

Avi Halachmi (:avih) - https://github.com/avih (boxdraw)

Alexander Rogachev - https://github.com/cog1to (ligatures)
