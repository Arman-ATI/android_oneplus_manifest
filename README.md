Installing Repos

        repo init -u https://github.com/ProjectMatrixx/android.git -b 14.0 --git-lfs

        git clone https://github.com/Arman-ATI/android_device_oneplus_manifest.git -b matrixx-GT .repo/local_manifests/
        
sync repo

        repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

for gt2 pro
        
        . build/envsetup.sh
        lunch lineage_ferrarri-userdebug
        make bacon
