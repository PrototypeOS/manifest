![PrototypeOS](https://user-images.githubusercontent.com/68080176/123559962-1c7b4f00-d754-11eb-8c13-99991a1c94b2.png)
PrototypeOS Ranch
PrototypeOS is the first of it's kind, Simple. Easy. Reliable. We aim to provide smooth easy going experience with a bit of customization.

To get started with the building process, you'll need to get familiar with Git and Repo.

To initialize your local repository, use a command like this:

    repo init -u git://github.com/PrototypeOS/manifest.git -b ranch

Then to sync up:-

    repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

Start the build:-

  source build/envsetup.sh

  lunch prototype_device_codename-userdebug
  
  mka bacon -jx
