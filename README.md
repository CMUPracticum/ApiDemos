#API DEMO#

*This project is the API Demo of Android SDK (API level 19, a.k.a. Andoird 4.4, Kitkat). The code can be found under /ANDROID SDK ROOT/samples/android-19/legacy.*

======

###Setting Up
1. Fetch the code from GitHub
2. Import to IDE. In Eclipse, File > Import > Android > Existing Android Code into Workspace
3. Clean and build the project
4. Setup Debug Configuration. In Eclipse, Run > Debug Configurations

###Common Problems
**1. Cannot resolve parent="android:Theme.Holo" in res/values-v11/styles.xml**    
This is due to incorrect project build target. The project should be built in Android 4.4, while the default target is usually Android 2.2.    

To set project build target, right click on the project on the Package Explorer side panel, Properties > Android > Project Build Target, select Android 4.4.2. Then clean and build the project again.   

If you cannot found the expected build target, check SDK Manager to see if SDK is properly installed.   

**2. Cannot find a package named android.support.v4.app**   
This project support down to Android 2.2, so it requires package android.support.v4.app, which is not imported in default.    

To import it, right click on the project on the Package Explorer side panel, Properties > Java Build Path > Add External JARs. The .jar can be found under /ANDROID SDK ROOT/extra/android/support/v4. Import it, then clean and build the project. World peace achieved!   

======

Ching-Lun Lin, clallenlin@gmail.com
