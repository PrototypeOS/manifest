![Photo_1625007046053](https://user-images.githubusercontent.com/68080176/123878990-a4698080-d92f-11eb-8246-82af43c61115.png)


PrototypeOS is the first of it's kind: 
Simple. Easy. Reliable. We aim to provide a smooth easy going experience with a bit of customization.

To get started with the building process, you'll need to get familiar with Git and Repo.

To initialize your local repository, use this command:

repo init -u https://github.com/PrototypeOS/manifest.git -b ranch

To sync the repository, use this command:

repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags

To Build, use following commands:

. build/envsetup.sh
lunch xtended_device-userdebug
make xtended -j$(nproc --all)

