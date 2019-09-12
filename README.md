﻿[日本語はこちら / Japanese](README.ja.md)

# Unity Editor Extension Controls Field of View (FoV) in Scene View

|Demo				|
|--------------------		|
|![demo](images/SceneViewFovControl.gif)	|

|Wide angle			|Telescopic (narrow angle)		|
|--------------------		|-------------------------		|
|![WideFov](images/WideFov.png)	|![NarrowFov](images/NarrowFov.png)	|

One thing [people](https://feedback.unity3d.com/suggestions/editor-camera-fov-adjustable) [repeatedly say](https://feedback.unity3d.com/suggestions/scene-view-camera-field-of-view-adjustment) is missing in Unity Editor's Scene View is that there is no way to control the Field of View (FoV).
With this extension, you will now be able to do this using the Unity Editor's private API.


## How to use
|Keyboard/Mouse					|Effect							|Note			|
|--------------------				|-------------------------				|----			|
|`FoV` button in the toolbar of Scene View	|Toggle FoV mode (auto / manual)			|			|
|Ctrl + Alt + Wheel				|Changes FoV						|			|
|Ctrl + Alt + Shift + Wheel			|Changes FoV (high speed)				|Unavailable on Mac	|
|Ctrl + Alt + O					|Increases FoV (wide angle)				|			|
|Ctrl + Alt + P					|Reduces FoV (narrow angle/telescopic)			|			|
|Ctrl + Alt + Shift + O				|Increases FoV (high speed, wide angle)			|			|
|Ctrl + Alt + Shift + P				|Reduces FoV (high speed, narrow angle/telescopic)	|			|

You can also right click the `FoV` button to use the following functionalities

|Menu name					|Effect						|Note							|
|--------------------				|-------------------------			|----							|
|FoV : Auto (Default behaviour)			|Set FoV mode to "Auto"				|"Auto" means Unity Editor's normal behaviour		|
|FoV : Manual					|Set FoV mode to "Manual"			|							|
|Reset Slave Camera				|Reset Slave Camera				|							|
|Slave Camera submenu				|You can select a camera which follows SceneView|If there're multiple Scene/GameView, you can set them independently	|


## Changing and Saving Settings

Select "Edit" > "Scene View FoV Settings" in the Unity Editor menu to open the settings window.

|Item				|Meaning						|
|--------------------		|-------------------------				|
|FoV Speed			|Changes FoV speed					|
|FoV Shift Modifier Multiplier	|Multiplies the modifier speed when pressing Shift	|
|Min FoV			|Minimizes FoV (angular unit)				|
|Max FoV			|Maximizes FoV (angular unit)				|
|				|							|
|Save				|Saves the settings					|
|Restore Default Settings	|Restores the default settings				|
|Restore Saved Settings		|Restores the saved settings				|
|Close				|Closes the window					|


## Prerequisites

This package needs Unity 5.5 or greater.  I've checked this package with Unity 5.5, 5.6 and 2017.1.


## References

- Slave Camera mode is based on [SyncCamera](https://github.com/anchan828/unitejapan2014/tree/master/SyncCamera/Assets) by @anchan828.


## License

[MIT](LICENSE.txt)
