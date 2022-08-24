![Project PROJECT-XTENDED](https://github.com/Project-Xtended/docs/raw/master/Xtended-banner.png)
-------------------------------------------------------------------------------------------------------

Project-Xtended:
====================
A ROM Based on AOSP, with features from almost all Custom ROMs available.


To initialize your local repository, use this command:
-----------------------------------------------------

    repo init -u https://github.com/Project-Xtended/manifest.git -b xt

To sync the repository, use this command:
-----------------------------------------

    repo sync

To Build, use following commands:
---------------------------------

    . build/envsetup.sh
    lunch xtended_device-userdebug
    mka xtended
