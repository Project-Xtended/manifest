![Project MSM-XTENDED](https://raw.githubusercontent.com/Project-Xtended/docs/master/template_Head.png)
-------------------------------------------------------------------------------------------------------

Project-Xtended:
====================
A ROM Based on AOSP, with features from almost all Custom ROMs available.


To initialize your local repository, use this command:
-----------------------------------------------------

    repo init -u https://github.com/Project-Xtended/manifest.git -b xq

To sync the repository, use this command:
-----------------------------------------

    repo sync -c --force-sync --no-tags --no-clone-bundle 

To Build, use following commands:
---------------------------------
    
    . build/envsetup.sh
    lunch xtended_device-userdebug
    make xtended

Apply for official maintainership [**HERE**](https://forms.gle/D9WPbBcbeVFiBMJb7)

--------------------------------------------------------------------------------------------------------
## Submitting Patches: ##

You can contribute to Project-Xtended just by registering at "https://review.msmxtended.me"

In order to submit patches, you will need an account setup with our Gerrit server and add changeid hooks.
To add changeid hook, use the following commands:

    cd <project>
    scp -p -P 29418 <username>@review.msmxtended.me:hooks/commit-msg .git/hooks/

You can also install the hook globally in all local Project-Xtended projects:

    cd <rom source>
    repo forall -c 'gitdir=$(git rev-parse --git-dir); scp -p -P 29418 <username>@review.msmxtended.me:hooks/commit-msg ${gitdir}/hooks/'

After that, you will have to create your ssh keys that are required for submitting patches to Gerrit:

```bash
ssh-keygen
```

Then in our Gerrit click on the "Settings" icon.

While in 'Settings' Click on "SSH Public Keys" on the left-hand side and then on "Add Key".

Then copy and paste the contents of ~/.ssh/id_rsa.pub to "Gerrit SSH Public Keys".

You can send patches to us by using these commands in terminal:

cd PROJECT - i.e
```bash
cd packages/apps/Xtensions
```
Make edits that you want to see .....
```bash
git add .
git commit -a
```
Type out a commit message that makes sense for the proposed change

Ctrl X, then Y to save and Enter

```bash
git push ssh://USERNAME@review.msmxtended.me:29418/Project-Xtended/PROJECT HEAD:refs/for/BRANCH
```
BRANCH - i.e xq

PROJECT - i.e packages_apps_Xtensions

USERNAME - i.e SuperDroidBond

A full command would look like this:

```bash
git push ssh://SuperDroidBond@review.msmxtended.me:29418/Project-Xtended/packages_apps_Xtensions HEAD:refs/for/xq
```

If you are going to make extra additions, just repeat steps (don't start a new patch), but instead of git commit -m
use git commit --amend. Gerrit will recognize it as a new patchset.

---------------------------------------------------------------------------------------------------------

Thread template refer [**HERE**](https://github.com/Project-Xtended/docs/blob/master/Thread_template.txt)

---------------------------------------------------------------------------------------------------------