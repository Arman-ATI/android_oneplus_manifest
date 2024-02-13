Installing Repos

        repo init -u https://github.com/Evolution-X/manifest -b udc

        git clone https://github.com/Arman-ATI/android_device_oneplus_manifest.git -b EvoX-GT .repo/local_manifests/
        
sync repo

        repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

for gt2 pro
        
        . build/envsetup.sh
        lunch evolution_ferrarri-userdebug
        m evolution
