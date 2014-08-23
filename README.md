TEAM Gummy
==============

Gummy AOSP 4.4.4

JAVA NOTICE:
------------

Gummy now builds with OpendJdk as it's default java, if your build environment still uses java6 then prior to building Gummy enter from the root of your build dir:

    {x}   export LEGACY_USE_JAVA6=true

Sync and Build:
---------------

In terminal enter:

    {x}   repo init -u git://github.com/k2wlxda/gum_manifest.git -b kk4.4
    {x}   repo sync
    {x}   prebuilts/misc/linux-x86/ccache/ccache -M 50G
    {x}   . build/envsetup.sh && brunch "device" -j8

