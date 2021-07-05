![Photo_1625007046053](https://user-images.githubusercontent.com/68080176/124511787-79b37800-ddc6-11eb-8360-569c19b28d25.png)

PrototypeOS is the first of it's kind: 
Simple. Easy. Reliable. We aim to provide a smooth easy going experience with a bit of customization.

# Getting Started:

To initialize your local repository, use a command like this:

    repo init -u git://github.com/PrototypeOS/manifest.git -b ranch
    
 You can alternatively use this command to save some space and time :

    repo init --depth=1 -u git://github.com/PrototypeOS/manifest.git -b ranch;
 

Then to sync up:-

    repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
   

You can just use repo sync or above command, but this will save you from lot of terminal spam, data and time.

    repo sync -c -q --force-sync --optimized-fetch --no-tags --no-clone-bundle --prune -j$(nproc --all);  
    
    
# Compilation of Prototype:


 . build/envsetup.sh

 lunch prototype_$device-userdebug

 mka prototype


