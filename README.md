# Oculus-Quest-Starter-UE4
![](https://raw.github.com/swenyan/Oculus-Quest-Starter-UE4/master/Readme/readme_0.png)

Oculus Quest Starter is a boilerplate project ready for Oculus Quest deployment. If you are new to Oculus Quest or Android development, setting up the environment could be really frustrating. This project (and this documentation) will probably save your day, seriously.

Supported Engine Version: Unreal Engine 4.25-4.26

#### Want to add Alyx-like gravity gloves in your game? Check this plugin:
https://www.unrealengine.com/marketplace/en-US/product/vr-gravity-grab-oculus

## BEFORE YOU START
Before you launch UE4 and dive into this project, you should get your Android SDK, NDK and JDK installed. If you have no idea about those SDK, NDK, JDK stuff, never mind, just remember you need to have them to make apps for Oculus Quest.

### You can follow the steps below to install the SDK, NDK, JDK stuff :

#### 1.Install Android Studio 3.5.3, which you can find here:
https://developer.android.com/studio/archive
![](https://raw.github.com/swenyan/Oculus-Quest-Starter-UE4/master/Readme/readme_1.png)

#### 2.Use Android Studio to install Android SDK, from API Level 25 to 29
![](https://raw.github.com/swenyan/Oculus-Quest-Starter-UE4/master/Readme/readme_2.png)

#### 3.Go to UE4 folder, open Engine/Extras/Android, run the SetupAndroid script to install NDK
![](https://raw.github.com/swenyan/Oculus-Quest-Starter-UE4/master/Readme/readme_3.png)
NDK path will be: C:/Users/[Username]/AppData/Local/Android/SDK/ndk/21.1.6352462

#### 4.Download and install JDK. This project is tested with JDK8u131, which you can find here:
https://www.oracle.com/java/technologies/javase/javase8-archive-downloads.html

## PROJECT SETTINGS
With the SDK, NDK, JDK stuff installed, you can now open the project in UE4, and set the SDK, NDK, JDK path in project settings.
![](https://raw.github.com/swenyan/Oculus-Quest-Starter-UE4/master/Readme/readme_4.png)

After setting the SDK, NDK, JDK path, go to “Project Settings -> Android”, click “Accept SDK License”.
![](https://raw.github.com/swenyan/Oculus-Quest-Starter-UE4/master/Readme/readme_5.png)

Now the project should be ready to launch on Oculus Quest.

## LAUNCH ON QUEST
With all settings done, connect your Quest to PC, disable oculus link, make sure developer mode and debugging is enabled.

Use the launch drop-down menu to launch the preview on Quest.

![](https://raw.github.com/swenyan/Oculus-Quest-Starter-UE4/master/Readme/readme_6.png)

If the Quest does not show up in the drop-down menu, open Project Launcher to find it.
![](https://raw.github.com/swenyan/Oculus-Quest-Starter-UE4/master/Readme/readme_7.png)

## BLUEPRINT REFERENCE
*BP_MotionControllerPawn_Oculus* – Pawn class inherited from BP_MotionControllerPawn, call setup function of BP_MotionController_Oculus at BeginPlay.

*BP_MotionController_Oculus* – Motion Controller inherited from BP_MotionController, setup offset and rotation of hand mesh for Oculus devices.

*BP_PickupCube, BP_PickupSphere* – Pickup blueprint examples.

To learn about more detail about implementation, please reference orange comment blocks and variable tooltips in each blueprint.


## REFERENCE
Oculus Quest Unreal Quick Start Guide:

https://developer.oculus.com/documentation/unreal/unreal-quick-start-guide-quest/

Setting Up Android SDK and NDK for Unreal:

https://docs.unrealengine.com/en-US/SharingAndReleasing/Mobile/Android/Setup/AndroidStudio/index.html
