Making stable long life cycle OS(EL10*), alternative desktop options available and thereby encouragig others to include it in EPEL asap, or as upstream ALLOWS!
Upstream wants a pure KDE/GNOME, I say 'NOPE', it's too late for that concept. If it's in Fedora, it's going to filter down to EL10/Clones. Some people don't require a SIG to tell hem what/how to make it happen, though a SIG can be helpful in other ways :)

### Part 1:
### PORTING XFCE4 to EL10/Clones! 
## SPECS/Source/Releases for testing XFCE4 on Wayland/labwc on el10/clones


<hr>

**Fresh Meme!**

## Hey, I'm on Wayland....with XFCE4 :) 

*This is only for testing/not production quality yet*

*XFCE4 4.20.x on Wayland is functional on EL10/clones. It can be started up via 
<code>
startxfce --wayland
</code>

Or 

One can use GDM.


Recent rebuilds have resolved most outstanding issues.
  
  Desktop displays normally.
  Most all plugins seem to work now.

*Rebuilding both sets x86_64(v3, the default) and x86_64_v2(for older hw)
Soon I will upload the  SRPMS here, and release tarballs of the RPMS.*
FYI, I mostly use F43 SRPMS as upstream sources with a few older in order to keep from upgrading OS/EPEL available packages. I try my best to NOT modify or upgrade
OS/EPEL packages. I'm also trying to rebuild the EL10/clones packages with minimal SPEC modifciations as well. This requires a precise order due to vala trying to work it's way in early in core XFCE packages.

The idea will be that a person can start with a minimal install console only or and existing install 
and then :
<code>
dnf install *.rpm
</code>

*I have not created a package group or meta pkg  of the components/deps yet, so installing via a custom repo is a little more tedious as you need to know which packages to install. So for now its easier for most to just use the dnf * method.*


In Summary, things are progressing well. XFCE4 looks and runs great on Wayland with very little CPU cycles wasted and its very low on memory usage too!
*Running a lite yet modern functional Desktop on Wayland EL10/Clones is here!*

Maybe I will spin up a Alma10.X XFCE Live on Wayland soon as well.

Other news:
I'm also building some applications such as goffice, those will go in other GH project(s).
Note, native gimp builds for pure wayland also work as well(minus batch building).
I think some work still needs to be done porting xwayland-run --> Xvfb-run in order to make it fully functional with batch processing.

