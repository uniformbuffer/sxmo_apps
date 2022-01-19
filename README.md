# sxmo_apps

This scripts will dynamically generate the application list for Sxmo/Swmo by collecting data from the desktop files present in the system.
The first time it is used, it will take a little bit of time to generate the list. Then the result is cached, so the following launches will be much faster (basically instant).
When one of the folders containing desktop files is updated (so installing or uninstalling an application), the list is regenerated.
The generated list is stored in `$XDG_CACHE_HOME/sxmo/apps` (`$XDG_CACHE_HOME` is usually the `~/.cache` folder), so if for some reason you want to force the script to regenerate the list, just remove that file and the list will be regenerated on the next launch.
This is needed if, for example, icons changed (added, removed or modified).
The icons script simply contains the list of icons that can be associated to the applications.

To install, just copy the `apps` and `icons` files to `~/.config/sxmo/hooks/` folder (in case you don't have such path, create the folders accordingly).

Have fun!
