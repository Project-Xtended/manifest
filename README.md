<a href="#"><img src="https://github.com/Project-Xtended/docs/blob/master/XT-Banner.png" /></a>
#

### 1. Setup Build environment
Setup your Build Environment and related dependencies from [HERE](https://source.android.com/docs/setup/build/building)
#
### 2. Initialize Xtended source
~~~bash
repo init -u https://github.com/Project-Xtended/manifest.git -b xt
~~~
#
### 3. Sync the repository ###
~~~bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
~~~
#
### 4. Start building Xtended
~~~bash
. build/envsetup.sh
lunch xtended_device-userdebug
make xtended -j$(nproc --all)
~~~    
#
### 5. Contributions
To submit changes/patches, please send a pull request on GitHub. We will review and merge.
#
### 6. How to get Official Maintainer
<details>
<br>
<summary><b>Make sure you can follow our rules-and-guidelines</b></summary>

## Project-Xtended Official Requirements

- You must have knowledge about source control tools such as git and repo.
- Device sources should be public on our official [Device Github](https://github.com/orgs/Xtended-Devices/repositories)
- Device sources must have proper commit history & authorship.
- All sources must be fully synced (pushed to GitHub) prior to every official build release
- Maintainers must test every build before release this including with testers if possible in order to avoid issues
- A Forum thread link must be made using [Official template](https://raw.githubusercontent.com/Project-Xtended/docs/master/XT-ThreadTemplate.txt) with your build on a dedicated community like XDA for example.
- Forum thread must contain all the device documentation such as installation steps,download links, sources etc.
- All hardware & basic sensors function must be operational 
- You can't redirect your official build's download link, Use only official downlaod server for release.

<b>After following above just message to Mukesh over [Telegram](https://telegram.me/mukesh22584) with the device you want to maintain.</b>
</details>

#

### Thanks to our open source communities
We are grateful to all the open source communities that have made this possible. Here it is worth to give them credit. 

- AOSP
- AOSPA
- Arrow OS
- crDroid Android
- DerpFest
- Flamingo-OS
- LineageOS
- OmniROM
- PixelExperience
- POSP
- ProtonAOSP
- StagOS
- Statix OS
- YAAP
