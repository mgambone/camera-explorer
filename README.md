Camera Explorer
===============

Camera Explorer application demonstrates the use of the new advanced
Windows Phone 8 camera API, the Windows.Phone.Media.Capture.PhotoCaptureDevice
and the related classes and enumerations on Nokia Lumia devices. The updated 
application adds tap-to-focus and Lens Picker integration.

The example has been developed with Silverlight for Windows Phone devices
and tested to work on Nokia Lumia devices with Windows Phone 8.

This example application is hosted in GitHub:
https://github.com/nokia-developer/camera-explorer

For more information on implementation and porting, visit Nokia Lumia
Developer's Library:
http://developer.nokia.com/Resources/Library/Lumia/#!imaging/advanced-photo-capturing/camera-explorer.html


What's new
----------

* Version 1.3.1.0: Minor bug fixes.
* Version 1.3.0.0: Support for devices without front camera, flash setting
  fixed, half-pressing camera key now reactivates auto-focus after tap-to-focus,
  settings (for each sensor) are now persistent.


1. Usage
-------------------------------------------------------------------------------

This is a simple build-and-run solution. Learn about Windows Phone 8
camera features by trying out the application. 


2. Prerequisites
-------------------------------------------------------------------------------

* C# basics
* Windows 8
* Development environment Microsoft Visual Studio Express for Windows Phone 2012


3. Project structure and implementation
-------------------------------------------------------------------------------

3.1 Folders
-----------

* The root folder contains the project file, the license information and this
  file (release_notes.txt).
* `CameraExplorer`: Root folder for the implementation files.
 * `Assets`: Graphic assets like icons and tiles.
 * `Properties`: Application property files.
 * `Resources`: Application resources.


3.2 Important files and classes
-------------------------------

| File | Description |
| ---- | ----------- |
| MainPage.xaml(.cs) | The main page with viewfinder and overlays. |
| SettingsPage.xaml(.cs) | The page that is used to modify camera parameters. |
| Parameter.cs | Implementations for binding. |
| RangeParameter.cs | PhotoCameraDevice API properties to XAML. |
| ArrayParameter.cs | controls in the SettingsPage UI. |


3.3 Used APIs/Windows Phone Components
--------------------------------------

* System.Windows.Media.Imaging
* Windows.Phone.Media.Capture


4. Compatibility
-------------------------------------------------------------------------------

* Windows Phone 8

Tested to work on Nokia Lumia 520, Nokia Lumia 820, and Nokia Lumia 920. 
Developed with Microsoft Visual Studio Express for Windows Phone 2012.


4.1 Required Capabilities
-------------------------

* `ID_CAP_ISV_CAMERA`
* `ID_CAP_MEDIALIB_PHOTO`


4.2 Known Issues
----------------

None.


5. Building, installing, and running the application
-------------------------------------------------------------------------------

5.1 Preparations
----------------

Make sure you have the following installed:

* Windows 8
* Windows Phone SDK 8.0


5.2 Using the WINDOWS PHONE 8 SDK
---------------------------------

1. Open the SLN file:
   File > Open Project, select the file CameraExplorer.sln
2. Select the target 'Device'.
3. Press F5 to build the project and run it on the device.


5.3 Deploying to Windows Phone 8
--------------------------------

Please see official documentation for deploying and testing applications on
Windows Phone devices:
http://msdn.microsoft.com/en-us/library/gg588378%28v=vs.92%29.aspx


6. License
-------------------------------------------------------------------------------

See the license text file delivered with this project. The license file is also
available online at 
https://github.com/nokia-developer/camera-explorer/blob/master/Licence.txt


7. Related documentation
-------------------------------------------------------------------------------

An article "Advanced Photo Capturing" published on Nokia Lumia Developer's Library
(http://www.developer.nokia.com/Resources/Library/Lumia/#!advanced-photo-capturing.html) 
describes the usage of PhotoCaptureDevice properties in more detail.


8. Version history
-------------------------------------------------------------------------------

* 1.3.1.0 Minor bug fixes.
* 1.3.0.0 Support for devices without front camera, flash setting fixed,
  half-pressing camera key now reactivates auto-focus after tap-to-focus,
  settings (for each sensor) are now persistent.
* 1.2.0.0 Bug fix to tap-to-focus (Ticket #5)
* 1.1.0.0 Tap-to-focus and Lens Picker integration added.
* 1.0.0.0 First release
