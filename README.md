![Photo_1625007046053](https://user-images.githubusercontent.com/68080176/123878990-a4698080-d92f-11eb-8246-82af43c61115.png)


PrototypeOS is the first of it's kind: 
Simple. Easy. Reliable. We aim to provide a smooth easy going experience with a bit of customization.

To get started with the building process, you'll need to get familiar with Git and Repo.

https://github.com/PrototypeOS/manifest#to-initialize-your-local-repository-use-this-command

repo init -u git://github.com/PrototypeOS/manifest.git -b ranch;


You can alternatively use this command to save some space and time :

repo init --depth=1 -u git://github.com/PrototypeOS/manifest.git -b ranch;

Then to sync up:

repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags;

You can just use repo sync or above command, but this will save you from lot of terminal spam, data and time.

repo sync -c -q --force-sync --optimized-fetch --no-tags --no-clone-bundle --prune -j$(nproc --all);
Start the build:-

  $ . build/envsetup.sh

  $  lunch prototype_<device_codename>-userdebug
  
  $  mka prototype
