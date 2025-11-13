### SPECS/Source/Releases for testing XFCE4 on Wayland/labwc on el10/clones

*This is only for testing/not production.*

*XFCE4  is functional on EL10/clones but the default configurations I'm using needs work still.*

*At this time, xfce4-panel is the main parent process under labwc/wayland, and you must (for now) manually choose 'fullscreen' on startup, to properly place the panel.
This step is not currently saved to a confuration either, so has to be done on each login. Hopefully, a sticky config will appear in a rpm here once figured out.*

See Screenshots for examples.

More SPECS to be added soon, along with RPMS/SRPMS in releases.  

*Only the minimal required will be included, only whats missing from repos and RPMS requiring changes to make it work, eg. network-manager-applet (nm-applet) changes were required for el10 in the spec, so its included with a higher level build release of '9999'. This will allow the same naming and upgrade any present non-functional versions when testing with XFCE4/Wayland.*
