# Changelog for GameDriver for Unity releases

## 06-22-2025 Version 2025.06

### Touch Input & Mobile Support

#### New Touch Recording System

* Comprehensive touch input recording capabilities for mobile testing  
* Support for both Legacy Input and New Input System touch recording

### Enhanced Input System Support

#### Custom Device Creation

* Custom device creation using Unity descriptions (`CreateDeviceCustom()`)  
* Enhanced gamepad and controller support

### VR/XR Support Enhancements

#### Virtual Reality Integration

* Automatic real device removal for headset testing  
* OpenXR headset detection and configuration  
* Improved VR input simulation  
* Custom VR device creation support

### UI/UX Enhancements

#### Light Infobox System

* Complete redesign replacing legacy OnGUI system  
* Modern, lightweight UI with improved visual design  
* Sprite-based graphics and better Unity UI integration  
* Automatic fallback to legacy infobox when needed

#### API Control & Configuration

* `ConfigureInfoBox()` for enabling/disabling, positioning, and scaling  
* `SetInfoBoxStatusMessage()` for custom status messaging  
* Configurable canvas render modes for VR/AR compatibility

### Unity Editor Integration

* Enhanced recording interface with improved visual layout

### Technical Improvements

#### Object Reference & HPath System

* Support for HPath-based object references (`CreateObjectRef(hPath)`, `RemoveObjectRef()`)  
* Improved object resolution and caching  
* Enhanced property lookup with binding flags

#### Video Recording Enhancements

* Fixed memory leaks during frame encoding  
* Better error handling for missing video libraries  
* More stable video recording across different platforms  
* Improved error reporting and diagnostics

#### API Enhancements

* Enhanced video recording API (`StartVideoRecording`, `StopVideoRecording`)  
* Better input management with `WaitForEmptyInput` improvements  
* Improved `GetObjectDistance` functionality  
* Enhanced debugging and error reporting capabilities

#### Platform & Compatibility

* WebGL build improvements and fixes  
* Console platform support improvements  
* iOS/Xcode build improvements with fixed OVR configuration

### Bug Fixes & Stability

#### Performance Optimizations

* Memory leak fixes  
* Better texture processing and resource cleanup  
* Improved connection management and stability  
* Enhanced thread safety across components

#### Input System Fixes

* Improved handling of double-click to prevent duplicate input events  
* Better input system detection and initialization  
* Fixed pointer events on mobile platforms  
* Improved touch device handling

#### General Stability

* Enhanced logging and diagnostic capabilities  
* Better screenshot functionality with UI element hiding  
* Improved error handling and exception management  
* More robust license validation and error reporting

### Developer Experience

#### Enhanced Developer Resources

* Comprehensive API documentation updates 
* Included XML for inline API documentation 
* New examples for video recording workflows  
* Enhanced touch input examples  
* Improved object reference usage patterns

#### Better Development Tools

* Enhanced error messages and debugging information  
* Improved diagnostic capabilities and logging  
* Better validation and error reporting throughout the system

## 02-25-2025 Version 2025.02

- Fixed a memory leak in video capture
- Fixed an issue with AutoPlay
- Fixed an issue with WebGL builds

## 01-01-2025 Version 2025.01

- GameDriver Test Assistant (TA)
  - Recorder
  - Object Explorer
  - HPath Debugger
  - Code Gen/Editor
  - Test/Unity Log Viewer
- UIToolkit Explorer enhancements
- OpenH264 Encoder Plugin and Video Capture APIs
- Improved HierarchyPath performance
- MRTK Support Updates
- Meta XR Support Updates
- Support for PlayMode options in newer versions of Unity (i.e. Domain Reload disabled)
- Added support for capturing client-side Object References to reduce the number of agent-side requests
- Misc. fixes and updates

## 03-13-2024 Version 2024.07

- Added configurable retry for WebSockets connections
- Extending fn:count() to support all objects resolved by an hpath and not just lists
- Added PlayStation 5 Support
- Added GetObjectPosition support for UIToolkit elements
- Updated Scroll API to support UIToolkit elements
- Gated SmartAgent and input hooking for ease of troubleshooting
- Fixed issue with AutoPlay targeting multiple editors using regex expressions
- Fixed an issue with MouseDrag on mobile devices
- Fixed an issue with GetObjectList not returning all object
- Misc performance and stability fixes

## 03-13-2024 Version 2024.05

- Support for Meta XR SDK
- Added InitializeApi method for enabling optional input support (e.g. Rewired, OVR)
- Misc bug fixes

## 03-13-2024 Version 2024.03

- Unity 2023 Support
- ECS/DOTS Support - contact <support@gamedriver.io> for more info
- Rewired Input Support
- Meta OVR Gesture Support
- Enforcement for node-locked licenses - read the EULA at <https://gamedriver.io/download>
- Additional GDIOAgent configuration updates:
  - Add Agent option added under the GameDriver menu
  - Change font type - Requires user to drop a .ttf file in the resources folder
  - Change font size and color
  - Change background size, color, and opacity
- Added support for debugging SmartAgents
- Misc Bug fixes
  - SmartAgent support for getting primitive type properties
  - TouchInput/Tap fixes
  - Input fixes (center click, caps lock, drag selection)
  - Config localization Fix
  - Fixed a crashing issue when Domain Reload was disabled
  - Fixed an issue where Trace logging wasn't reflected in the GameDriver menu
  - Fixed a potential memory leak in the HierarchyPath debugger
  - Added support for high code stripping in IL2CPP*
  - Fixed issue with GetObjectDistance reliability
  - Misc API doc fixes

## Known Issues

- iOS may crash if enhanced logging is enabled. We included a fix in this release to minimize this behavior, but this is a known issue [within Unity](https://forum.unity.com/threads/unity-2021-3-9f1-xcode-14-ios-16-problem.1335296/)

## 10-22-2023 Version 2023.10

- **GameDriver SmartAgents**
  - Embedded LUA scripting engine (Moonsharp)
  - Allows for complex agent-side behavior
  - Schedule and Execute scripts at runtime
- Nintendo Switch Support (GA)
- MRTK 2.0 Support
- OculusVR (OVR) Support
- Standalone Object Explorer (Beta)
- Re-enabled Unity 2019 with limited functionality (see [Product Availability Matrix](https://support.gamedriver.io/support/solutions/articles/69000836923) for details)
- Updated Input Recorder to perform post-processing of events. This will greatly improve performance while recording from XR devices such as the Meta Quest 2
- Added PoseInputEvent command for working with SteamVR
- Added support for HostID license locking
- Fixed several input hooking issues with IL2CPP
- Fixed an issue where an error was thrown while searching for disabled UI Documents in a scene
- Fixed an issue where the GameDriver version was not displayed in the Get Started dialog
- Fixed an issue with duplicate simulated XR device creation
- Fixed several issues with TouchObject
- Fixed several docs issues

## 06-15-2023 Version 2023.06

- Added support for Unity 2022.3 LTS
- Added TouchInput UI Toolkit support, including ScrollView objects
- Added Recorder support for Legaxy XR implementations (non Input System)
- Various Bug Fixes
  - Fixed a UTF Connection issue where the initial connection would loop indefinitely
  - Fixed an issue where `CreateDevice` with multiple devices using the same name and type strings would cause a StackOverflow exception
  - Fixed multiple IL2CPP issues
    - Added support for high code stripping
    - Removed requirement for custom script defines
    - Fixed an issue with `CreateInputDeviceFromDescription`

## 04-13-2023 Version 2023.04

- Added support for WebGL target builds
- Added support for SteamVR target builds
- Added support Nintendo Switch target builds (Beta)
- Added support for Xbox target builds (Beta)
- Added support for additional Unity Input Methods:
  - Gamepad Support
  - Updated XR Simulation workflow
  - Legacy XR Support
- Added support for UI Toolkit:
  - Click, ClickEx, (Double)ClickObject MouseMoveToObject, and Tap commands now support `fn:q` for accessing UIToolkit document nodes
  - Added `ClickObject_UIElement` and `ClickUIToolkit` commands
- Additional HierarchyPath Improvements:
  - Allow GameObjects to be resolved as method arguments using HPath
  - Search by `fn:type`
- Added menu option to enable/disable trace level logging
- Fixed issue with `EulerToQuat` maths
- Fixed issue with `WaitForObject` flooding the logs when an object was not found
- Additional documentation fixes

## Known Issues

- UTF Tests are not able to connect in 2023.04. Please continue to use the previous version until this is resolved.

## 12-27-2022 Version 2022.12

- Added UTF-8 support in license validation
- Added ObjectExists api
- Added `match` function for HPath using regular expressions
- Added `datetime` function for using date formats in HPath
- Added quote escaping in HPath strings
- Added descendant axis search to HPath
- Fixed several minor issues with the Recorder tool
- Various additional fixes

## 11-10-2022 Version 2022.11

- Added support for XR Recording
- Updated HierarchyPath Engine and new HPath Debugger
- New UnityLoggedMessage for passing unhandled exceptions to the ApiClient
- Added argument to GetObjectList to specify a root object via HPath
- Linux support (beta)
- Fixed an issue with Object Explorer throwing exceptions in some component types
- Fixed an issue with the Recorder flipping the origin and destination for MouseDrag events
- Additional bug fixes

## 09-19-2022 Version 2022.09

- Added argument to GetObjectList to include/exclude HPath for all objects returned
- Fixed an issue where destroying/recreating the agent would result in connection failures
- Minor bug fixes

## 07-16-2022 Version 2022.07

- XR Simulated Input
- New Recording tool
- New Input System commands
- HPath REPL (Read, Evaluate, Print, Loop)
- Various HierarchyPath (HPath) improvements and fixes
- Updated KeyCode mappings
- Improved agent stability
- Unity 2021 LTS support
- Apple Silicon support
- Python Client (beta)

For more information, visit <https://gamedriver.io/latest>

## 10-9-2021 (Beta)

- Added support for Unity New Input System
  - Projects using the New Input System will automatically be picked up by the GameDriver agent.
  - Projects using _both_ New Input System and Legacy Input Manager will default to the New Input System unless "Force Old Input System" is checked in the GameDriver Agent config.

**Limitations**: IL2CPP currently not supported on macOS/iOS when using the New Input System.

## 09-6-2021

Updated packages to include some additional fixes, as well as a static version of the API documentation (markdown viewer required). This build also includes:

- New StopEditorPlay, ToggleEditorPause, and ToggleEditorPlay commands for controlling editor Play mode during and after tests.
- ApiClient.Launch now returns a PID.
- New ApiClient.TerminateGame command for terminating a standalone instance of the running build.

## 08-14-2021

- Collision Detection updates and fixes. More information on how to test Collision Detection can be found in the [knowledge base](https://support.gamedriver.io).
- Object Explorer now supports exporting Absolute and Relative HierarchyPath values. The Object Explorer can be found in the Unity Editor under Window > GameDriver > Object Explorer.
- Additional type support within gdio.common.objects. See the [API documentation](https://github.com/GameDriver-io/gdio.unity_api.doc/blob/main/gdio.common.objects.md) for details.
- Various fixes for IL2CPP support on Android, iOS, and Windows build targets.
- Improved error messaging.
- API Documentation fixes and updates.

## 06-13-2020 Version 2.0

The GameDriver 2.0 release represents a major step forward in the evolution of automated testing for gaming. This release includes fixes for known issues, new APIs and features, and a new approach to testing in multi-deployment environments; allowing testers to write tests once and execute them on multiple platforms with little to no changes. Below is a list of the changes in this release.

It is required to remove all previously-installed GameDriver components from your Unity project in order to use this release. For detailed instructions on how to install GameDriver, please see this article.

- Added Android execution support

Now you can deploy and test against Android build targets, including emulators and physical devices via the Android SDK or an Appium server. To enable communications with the device, you need to issue the command:

```bash
adb forward tcp:19734 tcp:19734
```

This forwards port 19734 from your machine to the emulator or device running the GameDriver agent, allowing you to connect on localhost:19734. Replace 19734 with whatever port you are using for the GameDriver agent. To remove port forwarding after a test (if needed), run the command:

```bash
adb forward --remove tcp:19734
```

Additional Android details can be found in this article.

- New API notation. Eg:

```c#
ApiClient api = new ApiClient();
api.Connect("localhost", 19734);
api.WaitForObject("//*[@name = 'Capsule']");
api.RotateObject("//*[@name = 'Capsule']", new Vector3(5,2,-1));
api.MoveMouseToObject("//*[@name='InputField (TMP)']", 300);          
api.MoveMouseToPoint(new Vector2(0, 0), 4000);
```

- Expanded AutoPlay to support multiple Unity game instances and multithreading.

These examples are all generally the same thing when running on localhost. If you use a *, it will broadcast and any Unity Instance running on your network could respond with games that are playable via AutoPlay plugin. Supports Regular expression for matching a specific game when you have multiple instances running.

```c#
api.Connect("localhost", 19734, true); // Connects to a running Unity Editor. AutoPlay = true is the default

api.Connect("localhost", 19734, false); // Connects to a standalone build (no AutoPlay to Unity Editor)

api.Connect("*", ".*?myunitygame.**"); // Connects to any running instance of the Unity editor on the local network (broadcast) with the project name of myunitygame

api.Connect("localhost", ".*?myunitygame.*"); // Connects to any running instance of the Unity editor on the local machine with the project name of myunitygame

api.Connect("localhost"); // Connects to any running instance of the Unity editor on the local machine

api.Connect("*"); // Connects to any running instance of the Unity editor on the local network
```

Note that launching the agent is not supported across hosts and that it is required to set the project into a running state first.

- Updated SetInputFieldText() so that it calls the InputMethod text fields for standard or TMP Pro InputField.

```c#
api.SetInputFieldText("//*[@name='InputField']", "Hello GDIO API");   

api.SetObjectFieldValue("//*[@name='Text']/fn:component('UnityEngine.UI.Text')", "text", Guid.NewGuid().ToString());
```

- New GetObjectDistance API for measuring the distance between two objects. This method calculates the distance using vector subtraction, which compares all three position properties.

- New TouchInput API for simulating touch input. Refer to the API documentation for usage details.

- New object caching API to help reduce the frequency of which object queries are performed. Use EnableObjectCaching to enable the cache, and DisableObjectCaching to disable. FlushObjectCache can be used to clear the cache if needed.

- CallMethod now supports native types for public and private game methods. Use CallMethod\<T> to execute methods attached to game objects using various types and formats Examples:

```c#
// void return type
api.CallMethod("//*[@name = 'Capsule']/fn:component('KeyTest')", "TestMethod1",null);

string ksahdfksh = api.CallMethod<string>("//*[@name = 'Capsule']/fn:component('KeyTest')", "TestMethod2", null);

int skjhdfkjlah = api.CallMethod<int>("//*[@name = 'Capsule']/fn:component('KeyTest')", "TestMethod3", null);

int[] skjhfjshks = api.CallMethod<int[]>("//*[@name = 'Capsule']/fn:component('KeyTest')", "TestMethod4", null);

bool sdiuejd = api.CallMethod<bool>("//*[@name = 'Capsule']/fn:component('KeyTest')", "TestMethod5", new object[] { 7 });

bool agd7hgh = api.CallMethod<bool>("//*[@name = 'Capsule']/fn:component('KeyTest')", "TestMethod5", new object[] { 9, 3 });

// void return type
api.CallMethod("//*[@name = 'Capsule']/fn:component('KeyTest')", "TestMethod6", new object[] { new string[] { "game","driver","io" } });
```

- Added a tracing level to the logging which shows the commit hash for major components, which is useful for troubleshooting. Enable by adding the following line to GDIO/Resources/config/gdio.unity_agent.config.txt:

```xml
<logging><trace enabled="true" /></logging>
```

- Access Agent and Api version information via ApiClient.GetVersionsString

- All input-related methods now have a boolean WaitForEmptyInput=true/false argument, which is default to true for synchronous input. Set to false for asynchronous input.

- MouseDrag now accepts Vector2 as coordinate input. Example:

Old:

```c#
MouseDrag(Api.MouseButtons.Button, float x1, float y1, float x2, float y2, ulong frameCount);
```

New:

```c#
MouseDrag(MouseButtons.Button, Vector2 destination, ulong frameCount, [Vector2 origin = null], [bool waitForEmptyInput = true], [int timeout = 60])
```

- GetObjectPosition now returns a Vector3 object representing the x, y, z coordinates. Use .ToString or .x, .y or .z methods to extract individual coordinates.

- ClickObject has changed from (object, mouse button, duration) to (mouse button, object, duration) for consistency

- Added a Camera argument to GetObjectPosition and RayCast commands, allowing you to override the default Camera.main when more than one Camera exists in a scene.

- gdio.license has been renamed to gdio.license.txt for ease of use with external readers. The license file should now be saved to the Assets\GDIO\Resources folder of your Unity project.

- EnableMouseHooks and EnableKeybordHooks have been replaced with EnableHooks(HookingObject), which now includes KEYBOARD, MOUSE, GAMEPAD, TOUCHINPUT, and ALL) options. Likewise, DisableKeybordHooks and DisableMouseHooks have been replaced with DisableHooks(HookingObject).

- GetObjectFieldValue now supports native object types, such as the primitives: string, int, float, and bool as well as translation classes such as color, vertex, and transform. Certain containers such as List and Dictionary are also supported. Type is dependent on the target object, component, and field. For example:

```c#
String invisCube = api.GetObjectFieldValue<String>("//*[@name='HiddenCube']/fn:component('UnityEngine.Behaviour')/@isActiveAndEnabled");
```

Note: Object types supported by GameDriver are representations of their UnityEngine equivalent in order to keep them light and independent. These are implemented in the gdio.common.objects namespace.

- GetObjectList now returns additional information as a gdio.common.objects.LiteGameObject. Example usage:

```c#
// Pull a list of the scene objects
System.Collections.Generic.List<LiteGameObject> objects = api.GetObjectList();

//Test whether the list is null
Assert.IsNotNull(objects, "GetObjectList failed!");

//Print a full object list
foreach (var obj in objects)
{
Console.WriteLine("Object Name: " + obj.Name);
Console.WriteLine("Object Tag: " + obj.Tag);
Console.WriteLine("Object Position: " + obj.Position);
Console.WriteLine("Object Rotation: " + obj.Rotation);
}
```

Output:

```bash
Object Name: GameDriver
Object Tag: Untagged
Object Position: (0, 0, 0)
Object Rotation (w): 1, (x): 0, (y): 0, (z): 0

Object Name: Cube
Object Tag: MovementCube
Object Position: (0, 0, -700)
Object Rotation (w): 1, (x): 0, (y): 0, (z): 0

Object Name: Main Camera
Object Tag: MainCamera
Object Position: (0, 0, -800)
Object Rotation (w): 1, (x): 0, (y): 0, (z): 0

Object Name: ReturnButton
Object Tag: Untagged
Object Position: (793.5, 383, 0)
Object Rotation (w): 1, (x): 0, (y): 0, (z): 0

Object Name: Canvas
Object Tag: Untagged
Object Position: (0, 0, 0)
Object Rotation (w): 1, (x): 0, (y): 0, (z): 0
```

etc...

- New Logging Control. To enable logging, you will need to register to receive logging events in the client (test). To do so, simply add the following to your test script, or substitute with your own output method as desired.

```c#
ApiClient api = new ApiClient(); // This should already be part of your test

api.LoggedMessage += (s, e) =>
{
    Console.WriteLine(e.Message);
};
```

- Removed GDIOBuildProcessor.dll, which is no longer required.

- Fixed an issue where the text property of a TMP Input Field object appends an unprintable Unicode character on the end, making it impossible to query the field from within a test. Now when doing string comparisons, by default, users have the option to ignore that code point. Configure via a new config value in GDIO/Resources/config/gdio.unity_agent.config.txt:

```c#
<unicode><ignoreZeroWidthSpace enabled="true"/></unicode>
```

**Note** this setting is not applicable to GetObjectFieldValue\<T>, which is intended to capture the precise value of the field, including unprintable characters.
