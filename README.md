
PrototypeOS is the first of it's kind: 
Simple. Easy. Reliable. We aim to provide a smooth easy going experience with a bit of customization.

To initialize your local repository, use a command like this:

    repo init -u git://github.com/PrototypeOS/manifest.git -b ranch

Then to sync up:-

    repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

Start the build:-

  . build/envsetup.sh
  lunch prototype_<devicecodename>-userdebug
  mka prototype -jx
