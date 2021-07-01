
PrototypeOS is the first of it's kind: 
Simple. Easy. Reliable. We aim to provide a smooth easy going experience with a bit of customization.

To get started with the building process, you'll need to get familiar with Git and Repo.

To initialize your local repository, use this command:

repo init -u https://github.com/PrototypeOS/manifest.git -b ranch

To sync the repository, use this command:

repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

To Build, use following commands:

. build/envsetup.sh

lunch prototype_device-userdebug

mka prototype -j$(nproc --all)

