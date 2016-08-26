# Possible commands

You can execute an editor command by pressing `Ctrl-e` followed by the command.
Here are the possible commands that you can use.

* `quit`: Quits micro.

* `save`: Saves the current buffer.

* `replace "search" "value" flags`: This will replace `search` with `value`. 
   The `flags` are optional.
   At this point, there is only one flag: `c`, which enables `check` mode 
   which asks if you'd like to perform the replacement each time

   Note that `search` must be a valid regex.  If one of the arguments
   does not have any spaces in it, you may omit the quotes.

* `set option value`: sets the option to value. See the `options` help topic
   for a list of options you can set.

* `setlocal option value`: sets the option to value locally (only in the current
   buffer).

* `run sh-command`: runs the given shell command in the background. The 
   command's output will be displayed in one line when it finishes running.

* `bind key action`: creates a keybinding from key to action. See the sections on
   keybindings above for more info about what keys and actions are available.

* `vsplit filename`: opens a vertical split with `filename`. If no filename is
   provided, a vertical split is opened with an empty buffer

* `hsplit filename`: same as `vsplit` but opens a horizontal split instead of
   a vertical split

* `tab filename`: opens the given file in a new tab.

---

The following commands are provided by the default plugins:

* `lint`: Lint the current file for errors.

* `gofmt`: Run gofmt on the current file.

* `goimports`: Run goimports on the current file.