
gtaxlwifi-lineage-19.1
===========

To initialize your local repository use a command like this:
````bash
repo init -u https://github.com/LineageOS-UL/android.git -b lineage-19.1 --git-lfs
````
Then you need to clone the local_manifest:
````bash
git clone https://github.com/FlominatorGD/manifest-gtaxlwifi.git -b lineage-19.1 .repo/local_manifests
````
Then to sync up:
````bash
repo sync --force-sync --no-tags --no-clone-bundle -c
````
Finally to build:
````bash
. build/envsetup.sh && brunch lineage_gtaxlwifi-userdebug
````
