![Photo_1625007046053](https://user-images.githubusercontent.com/68080176/123878990-a4698080-d92f-11eb-8246-82af43c61115.png)


PrototypeOS is the first of it's kind: 
Simple. Easy. Reliable. We aim to provide a smooth easy going experience with a bit of customization.

To get started with the building process, you'll need to get familiar with Git and Repo.

To initialize your local repository, use a command like this:

    repo init -u git://github.com/PrototypeOS/manifest.git -b ranch

Then to sync up:-

    repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

Start the build:-

  $ . build/envsetup.sh

  $ lunch prototype_<device_codename>-userdebug
  
  $ mka bacon -jx
