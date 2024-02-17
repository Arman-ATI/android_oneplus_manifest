Installing Repos

        repo init -u https://github.com/alphadroid-project/manifest -b alpha-14 --git-lfs

        git clone https://github.com/Arman-ATI/android_device_oneplus_manifest.git -b alpha .repo/local_manifests/
        
sync repo

        repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

for op 10pro
        
        . build/envsetup.sh
        lunch lineage_wly-userdebug
        make bacon
