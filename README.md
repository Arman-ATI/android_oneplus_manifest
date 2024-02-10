Installing Repos

        repo init -u https://github.com/PixelOS-AOSP/manifest.git -b fourteen --git-lfs

        git clone https://github.com/Arman-ATI/android_device_oneplus_manifest.git -b PixelOS .repo/local_manifests/
        
sync repo

        repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

for op 10pro
        
        . build/envsetup.sh
        lunch aosp_wly-userdebug
        make bacon

for gt2 pro
        
        . build/envsetup.sh
        lunch aosp_ferrarri-userdebug
        make bacon
