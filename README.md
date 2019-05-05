# Phonograph Pro
[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](https://github.com/kabouzeid/Phonograph/blob/master/LICENSE.txt)

**A material designed local music player for Android.**

![Screenshots](./art/art.jpg?raw=true)

## Pro Version
Under the **GPLv3 License**, users are allowed to modify and redistribute this software.

## Download
You can download an apk file of the pro version [here](https://github.com/RebornQ/Phonograph/releases).

## Do it yourself
1. Fork the original [Phonograph repo](https://github.com/kabouzeid/Phonograph)
2. Go to `/app/src/main/java/com/kabouzeid/gramophone/App.java`
3. Change the contents of this method:
    
    ```java
    public static boolean isProVersion() {
            return BuildConfig.DEBUG || app.billingProcessor.isPurchased(PRO_VERSION_PRODUCT_ID);
    }
    ```
        
    To this: 
    
    ```java
    public static boolean isProVersion() {
        //        return BuildConfig.DEBUG || app.billingProcessor.isPurchased(PRO_VERSION_PRODUCT_ID);
            return true;
    }
    ```
    
4. Enjoy yourself.
