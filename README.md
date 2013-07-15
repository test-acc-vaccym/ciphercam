ciphercam
=========

ciphercam is camera library that writes all media it records (video and images) direct into an IOCipher instance in as secure a fashion as possible


## Setting up Development Environment

**Prerequisites:**

* [Android SDK](https://developer.android.com/sdk/installing/index.html)
* Working [Android NDK](https://developer.android.com/tools/sdk/ndk/index.html) toolchain

Follow these steps to setup your dev environment:

1. Checkout ciphercam git repo
2. Init and update git submodules

    git submodule update --init --recursive

3. Ensure `NDK_BASE` env variable is set to the location of your NDK, example:

    export NDK_BASE=/path/to/android-ndk

4. Ensure the ndk tools are on your path

    export PATH=$NDK_BASK:$PATH

5. Import externals into eclipse

    Import into Eclipse (using the "existing projects" option) the projects in this order:

        external/IOCipher/
        external/CacheWord/cachewordlib
        
6. setup IOCipher according to it's README

7. setup CacheWord accoriding to it's README
