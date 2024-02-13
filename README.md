Installing Repos

        repo init -u https://github.com/PixelOS-AOSP/manifest.git -b fourteen --git-lfs

        git clone https://github.com/Arman-ATI/android_device_oneplus_manifest.git -b PixelOS-GT .repo/local_manifests/
        
sync repo

        repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

for gt2 pro
        
        . build/envsetup.sh
        lunch aosp_ferrarri-userdebug
        make bacon
