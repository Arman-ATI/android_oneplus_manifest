Installing Repo

        git clone https://github.com/Arman-ATI/android_device_oneplus_manifest.git -b EvoX .repo/local_manifests/

        repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
