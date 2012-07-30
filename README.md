Gnome 3 Window Buttons Extension
================================

This is an exntesion for Gnome 3 which puts minimize, maximize and close buttons in the top panel.

Supports custom button layouts and css theming!

You have to restart gnome-shell to apply a new theme properly.

Currently the buttons only control the active window.

Settings can be found at _org.gnome.shell.extensions.window-buttons_ in **dconf-editor**

Installation
------------

### GNOME 3.4
Install the extension (gnome3.4 branch):

	$ cp window_buttons@biox.github.com ~/.local/share/gnome-shell/extensions/

Configure using `gnome-shell-extension-prefs`.

### GNOME 3.2

Copy the schema file to _/usr/share/glib-2.0/schemas_

	# cp org.gnome.shell.extensions.window-buttons.gschema.xml /usr/share/glib-2.0/schemas/

Install schema:

	# glib-compile-schemas /usr/share/glib-2.0/schemas

Install the extension itself

	$ cp window_buttons@biox.github.com ~/.local/share/gnome-shell/extensions/

or

	# cp window_buttons@biox.github.com /usr/share/gnome-shell/extensions/

To-do
-----

- Check for theme matching metacity theme
- Add unfocused window support for better theming
- Add option to handle only maximized windows
- Add option to hide if there are no maximized windows
- Moar themes!
