![Project PROJECT-XTENDED](https://github.com/Project-Xtended/docs/raw/master/Xtended-banner.png)
-------------------------------------------------------------------------------------------------------

Project-Xtended:
====================
A ROM Based on AOSP, with features from almost all Custom ROMs available.


To initialize your local repository, use this command:
-----------------------------------------------------

    repo init -u https://github.com/Project-Xtended/manifest.git -b xr

To sync the repository, use this command:
-----------------------------------------

    repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

To Build, use following commands:
---------------------------------
    
    . build/envsetup.sh
    lunch xtended_device-userdebug
    make xtended -j$(nproc --all)

---------------------------------------------------------------------------------------------------------

Thread template refer [**HERE**](https://github.com/Project-Xtended/docs/blob/master/Thread_template.txt)

---------------------------------------------------------------------------------------------------------
