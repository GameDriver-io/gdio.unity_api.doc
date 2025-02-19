# ApiClient class

GameDriver.io Unity API Client class.

```csharp
public class ApiClient
```

## Public Members

| name | description |
| --- | --- |
| [ApiClient](ApiClient/ApiClient.md)() | GameDriver Unity API Client class constructor. |
| event [LoggedMessage](ApiClient/LoggedMessage.md) | Event handler for logged messages. Add a callback method to this handler to recieve all logging messages from the API. |
| event [ScriptSignal](ApiClient/ScriptSignal.md) | Event handler for SmartAgent events. Add a callback method to this handler to recieve all event signals from an executing Lua script. |
| event [UnityLoggedMessage](ApiClient/UnityLoggedMessage.md) | Event handler for Unity logged messages. Add a callback method to this handler to recieve all logging messages from the Agent. |
| [AxisPress](ApiClient/AxisPress.md)(…) | Use this function to send arbitrary Axis states to the game. |
| [ButtonPress](ApiClient/ButtonPress.md)(…) | Use this function to send arbitrary button states to the game. Defaults to LEFT ALT/CTRL/SHIFT/WINDOWS(COMMAND) (2 methods) |
| [CallMethod](ApiClient/CallMethod.md)(…) | Use this function to execute a [System.Void](https://learn.microsoft.com/en-us/dotnet/api/system.void) method on an object or from a static class. |
| [CallMethod&lt;T&gt;](ApiClient/CallMethod.md)(…) | Use this function to execute a method on an object or from a static class. |
| [CaptureScreenshot](ApiClient/CaptureScreenshot.md)(…) | Use this function to capture a screenshot of the Game under test. |
| [Click](ApiClient/Click.md)(…) | Use this function to perform in-game mouse-clicks at the current mouse position. (3 methods) |
| [ClickEx](ApiClient/ClickEx.md)(…) | Use this function to interact with an in-game object or UI items using mouse-clicks combined with modifier key press operations. The total frame count of this operation is clickFrameCount + modifiersNumberOfFrames (3 methods) |
| [ClickObject](ApiClient/ClickObject.md)(…) | Use this function to interact with an in-game object using mouse-clicks. |
| [ClickObjectEx](ApiClient/ClickObjectEx.md)(…) | Use this function to interact with an in-game object using mouse-clicks combined with key press operations. The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames. (2 methods) |
| virtual [Connect](ApiClient/Connect.md)(…) | Use this function to connect to a Unity game with GameDriver Agent configured and active. This function can connect to the Unity editor or a Standalone deployment of a game. |
| [Connect](ApiClient/Connect.md)(…) | Use this function to connect to a Unity game with GameDriver Agent configured and active. This function can connect to the Unity editor or a Standalone deployment of a game. |
| [CreateInputDevice](ApiClient/CreateInputDevice.md)(…) | Use this function to create a device of any type from a Unity layout (OculusHMD, Mouse, etc). |
| [CreateInputDeviceFromDescription](ApiClient/CreateInputDeviceFromDescription.md)(…) | Use this function to create a device from a controller's description file. Use "LoadDeviceDescription" to obtain the jsonDescription string, or create your own. |
| [CreateObjectRef](ApiClient/CreateObjectRef.md)(…) | Instantiate an Object (Not a GameObject) using its `Type` and Constructor params if any and store it's reference as an ObjectRef. (3 methods) |
| [DisableHooks](ApiClient/DisableHooks.md)(…) | Disable input hooks in the game. |
| [DisableObjectCaching](ApiClient/DisableObjectCaching.md)(…) | Disable the use of object caching when doing HierarchyPath object resolution. |
| virtual [Disconnect](ApiClient/Disconnect.md)() | Use this function to disconnect the API client from the Game. |
| [DoubleClick](ApiClient/DoubleClick.md)(…) | Use this function to perform in-game mouse double-clicks. (2 methods) |
| [DoubleClickEx](ApiClient/DoubleClickEx.md)(…) | Use this function to perform in game mouse double clicks combined with key press operations. The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames (2 methods) |
| [DoubleClickObject](ApiClient/DoubleClickObject.md)(…) | Use this function to interact with an object in game using a mouse double-click. |
| [DoubleClickObjectEx](ApiClient/DoubleClickObjectEx.md)(…) | Use this function to interact with an object in game using a mouse double-click, combinated with key press operations. The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames |
| [EnableHooks](ApiClient/EnableHooks.md)(…) | Enable input hooks in the game, which is required to perform various input types during replay. |
| [EnableObjectCaching](ApiClient/EnableObjectCaching.md)(…) | Enable the use of object caching when performing HierarchyPath object resolution. Object caching is per HierarchyPath stored in a [System.Collections.IDictionary](https://learn.microsoft.com/en-us/dotnet/api/system.collections.idictionary). If a matching HierarchyPath is already in the dictionary, then the stored object is returned. The only way to update a cached reference is for the reference to be garbage collected or flush the cache with [`FlushObjectLookupCache`](./ApiClient/FlushObjectLookupCache.md). |
| [EulerToQuat](ApiClient/EulerToQuat.md)(…) | Method will convert Euler Angles to Quaternion, if using Vector3 is an issue. (2 methods) |
| [ExecuteScript](ApiClient/ExecuteScript.md)(…) | This method executes a Lua script. |
| [ExecuteScript&lt;T&gt;](ApiClient/ExecuteScript.md)(…) |  |
| [FlushObjectLookupCache](ApiClient/FlushObjectLookupCache.md)(…) | If object caching is enabled, this method will request that the agent flush the cache being held for all object lookups. |
| [GetConnectedGameDetails](ApiClient/GetConnectedGameDetails.md)() | This method returns the details of the game that the API client is connected to. |
| [GetDeviceLicenseIdentifier](ApiClient/GetDeviceLicenseIdentifier.md)() | This method retrieves the License Identifier for the device running the Unity Game. |
| [GetLastFPS](ApiClient/GetLastFPS.md)() | This method returns the last frames per second that the API client has recieved from the GameDriver agent. |
| [GetMethodList](ApiClient/GetMethodList.md)(…) | Returns a dictionary of the methods attached to the target object. The key of the dictionary is a string representing the method signature. The value of the dictionary is the hierarchy path of the object the method is attached to. |
| [GetNextCollisionEvent](ApiClient/GetNextCollisionEvent.md)(…) | Collision events are stored in a FIFO queue. Calling this method returns the next collision event that was returned. |
| [GetObjectDistance](ApiClient/GetObjectDistance.md)(…) |  |
| [GetObjectFieldValue&lt;T&gt;](ApiClient/GetObjectFieldValue.md)(…) | This method returns the field or property value of an object. (2 methods) |
| [GetObjectList](ApiClient/GetObjectList.md)(…) | This method returns of a list of all GameObjects as returned by [UnityEngine.GameObject.FindObjectsOfType(Type)](https://docs.unity3d.com/ScriptReference/Object.FindObjectsOfType.html), where Type is UnityEngine.GameObject. (2 methods) |
| [GetObjectPosition](ApiClient/GetObjectPosition.md)(…) | Return the position of a specific object. |
| [GetPropertyList](ApiClient/GetPropertyList.md)(…) | Returns a dictionary of the properties and fields attached to the target object. The key of the dictionary is the hierarchy path of the property. The value of the dictionary is the value of the property represented as a string. |
| [GetSceneName](ApiClient/GetSceneName.md)(…) | Return the name of the current active scene. |
| [InitializeApi](ApiClient/InitializeApi.md)(…) | Use this function to initialize Rewired if the Rewired Input Manager was not in the starting scene. |
| [IntegerInputEvent](ApiClient/IntegerInputEvent.md)(…) | Use this function to send diferent kinds of Input Events to an action based Input System. |
| [KeyPress](ApiClient/KeyPress.md)(…) | Use this function to send arbitrary button states to the game. Defaults to LEFT ALT/CTRL/SHIFT/WINDOWS(COMMAND) |
| [LoadDeviceDescription](ApiClient/LoadDeviceDescription.md)(…) | Loads a controller description file. Can be obtained in Unity in the Input Debug by right clicking a device and selecting "Copy Device Description" then pasting to a .json file |
| [LoadScene](ApiClient/LoadScene.md)(…) | This method loads the scene, defined by the scene name passed as an argument. |
| [MapInputControlPathsUsed](ApiClient/MapInputControlPathsUsed.md)(…) | This method returns all the control input paths being used. |
| [MouseDrag](ApiClient/MouseDrag.md)(…) | Perform a mouse drag operation. |
| [MouseMoveToObject](ApiClient/MouseMoveToObject.md)(…) | Move the mouse to the center of a specific object, identified by the HierarchyPath. |
| [MouseMoveToPoint](ApiClient/MouseMoveToPoint.md)(…) | Move the mouse to the destination vector. |
| [NavAgentMoveToPoint](ApiClient/NavAgentMoveToPoint.md)(…) | Move a NavAgent to a destination point. |
| [ObjectExists](ApiClient/ObjectExists.md)(…) | Check for an object to exist. Do NOT use this to poll, use WaitForObject instead. There is a builtin response timeout of 5 seconds if the Agent/Game does not respond. |
| [PoseInputEvent](ApiClient/PoseInputEvent.md)(…) | Use this function to send arbitrary combinations of Vector3 and Quaternions to a game. This is usually the way when dealing with matrices. This is only used by SteamVR for now. |
| [QuaternionInputEvent](ApiClient/QuaternionInputEvent.md)(…) | Use this function to send arbitrary Quaternion Event states to the game. |
| [Raycast](ApiClient/Raycast.md)(…) | Perform a Raycast to a point to find out what is in that position. |
| [ReconfigurePort](ApiClient/ReconfigurePort.md)(…) | Used to modify the listening port of the GDIOAgent once a connection has been established with the client. |
| [RegisterCollisionMonitor](ApiClient/RegisterCollisionMonitor.md)(…) | Register a collision monitor to recieve collision events on an object. |
| [RemoveInputDevices](ApiClient/RemoveInputDevices.md)(…) | Removes all devices created by GDIO "CreateDevice" methods. Should be used in OneTimeTearDown to prevent issues with controllers remaining in the scene. |
| [RemoveObjectRef](ApiClient/RemoveObjectRef.md)(…) | Remove an objectRef |
| [RotateObject](ApiClient/RotateObject.md)(…) | Rotate an object defined by the HierarchyPath and rotated by a Quaternion. [https://scriptinghelpers.org/blog/how-to-think-about-quaternions](https://scriptinghelpers.org/blog/how-to-think-about-quaternions) for more information. (4 methods) |
| [ScheduleScript](ApiClient/ScheduleScript.md)(…) | This method schedules the execution of a Lua script. |
| [Scroll](ApiClient/Scroll.md)(…) | Use this function to simulate mouse wheel scrolling. NOTE: The new input system values are a factor of 120 |
| [SetInputFieldText](ApiClient/SetInputFieldText.md)(…) | Set the text of an InputField or TMP_InputField |
| [SetObjectFieldValue](ApiClient/SetObjectFieldValue.md)(…) | Set the field or property of an object. |
| [SetXRDeviceMode](ApiClient/SetXRDeviceMode.md)(…) | Used to change between controller and hand modes in XR if one of the used modes is not working or being rendered. Mostly for OVR. Set by default to both: XRDeviceModes.CONTROLLER &#x7C; XRDeviceModes.HAND. Ex: SetXRDeviceModes("GDIOLeftHand", XRDeviceModes.HAND) or SetXRDeviceModes("GDIOLeftHand", XRDeviceModes.CONTROLLER &#x7C; XRDeviceModes.HAND). |
| [SkeletonInputEvent](ApiClient/SkeletonInputEvent.md)(…) | Use this function to send arbitrary Skeleton Event states to the game. (2 methods) |
| [StartVideoRecording](ApiClient/StartVideoRecording.md)(…) | Use this function to start a video recording of the screen space viewport. (3 methods) |
| [StopEditorPlay](ApiClient/StopEditorPlay.md)() | Stop a game from playing in the Editor, if it is currently in Play mode. |
| [StopVideoRecording](ApiClient/StopVideoRecording.md)(…) | Use this function to stop a video recording. |
| [Tap](ApiClient/Tap.md)(…) | Tap the handheld device at the defined position. (2 methods) |
| [TapObject](ApiClient/TapObject.md)(…) | Tap an object. (2 methods) |
| [ToggleEditorPause](ApiClient/ToggleEditorPause.md)() | Toggle the Pause mode in the Editor, if a game is in Play mode. If AutoPlay is not used, then 127.0.0.1 will be used as a default. |
| [TouchInput](ApiClient/TouchInput.md)(…) | Send a raw TouchInput event to the game. (2 methods) |
| [UnregisterCollisionMonitor](ApiClient/UnregisterCollisionMonitor.md)(…) | Unregister the monitoring of collision events on a GameObject that has been previously registered for monitoring. |
| [UnscheduleScript](ApiClient/UnscheduleScript.md)(…) | Unschedules a Script that was scheduled by the ScheduleScript command. |
| [UseWebSockets](ApiClient/UseWebSockets.md)(…) | Configure a WebSocket server for a client (GDIOAgent) to connect to. |
| [Vector2InputEvent](ApiClient/Vector2InputEvent.md)(…) | Use this function to send arbitrary Vector2 Event states to the game. |
| [Vector3InputEvent](ApiClient/Vector3InputEvent.md)(…) | Use this function to send arbitrary Vector3 Event states to the game. |
| [Wait](ApiClient/Wait.md)(…) | Client side Wait or Pause. |
| [WaitForCollisionEvent](ApiClient/WaitForCollisionEvent.md)(…) | Wait for a collision event to fire on an element that is being monitored for collisions. If the method has been called before, there is the potential that another event was recieved before waiting on the event again. Check with [`GetNextCollisionEvent`](./ApiClient/GetNextCollisionEvent.md) to see if it returns null to see if an event was missed. |
| [WaitForEmptyInput](ApiClient/WaitForEmptyInput.md)(…) | Wait for an Empty Input event to be received. (2 methods) |
| [WaitForObject](ApiClient/WaitForObject.md)(…) | Wait for an object to exist. |
| [WaitForObjectValue](ApiClient/WaitForObjectValue.md)(…) | Wait for an object to exist and have a specific value for a specified field/property. |
| static [AUTOPLAY_BROADCAST_ADDR](ApiClient/AUTOPLAY_BROADCAST_ADDR.md) | The broadcast address to use for sending out AutoPlay requests. The default is for localhost: 127.0.0.1 |
| static [AUTOPLAY_DEFAULT_PORT](ApiClient/AUTOPLAY_DEFAULT_PORT.md) | The default AUTOPLAY port to use when searching for running games. This port is configured in the Unity preferences. |
| static [AUTOPLAY_ENABLED](ApiClient/AUTOPLAY_ENABLED.md) | NOT IN USE. |
| static [AUTOPLAY_RECEIVE_PORT](ApiClient/AUTOPLAY_RECEIVE_PORT.md) | The port to listen for responses from the AutoPlay plugin running in Unity. Due to loopback limitations, this port must be different than the [`AUTOPLAY_DEFAULT_PORT`](./ApiClient/AUTOPLAY_DEFAULT_PORT.md) |
| static [THROW_EXCEPTIONS](ApiClient/THROW_EXCEPTIONS.md) | If TRUE, the API will throw exceptions instead of logging errors and where applicable returning false/NULL. The default is FALSE. |
| static [GetVersionsString](ApiClient/GetVersionsString.md)() | Returns the GameDriver component versions in this build. |
| static [Launch](ApiClient/Launch.md)(…) | Use this function to launch the Unity game build from an executable. In order to automate execution, games should be set to automatically start at the desired screen resolution and require no additional external dialogs to start. These can typically be set in Unity under Build Settings &gt; Resolution, Other Settings, etc... |
| static [TerminateGame](ApiClient/TerminateGame.md)() | If a standalone game was started with Launch, this method will terminate the Game process. |

## Protected Members

| name | description |
| --- | --- |
| virtual [IsRecorder](ApiClient/IsRecorder.md) { get; } |  |
| [client](ApiClient/client.md) |  |
| event [MessageReceived](ApiClient/MessageReceived.md) | Passthrough event handler for for Api Extensions, eg: Recorder |
| [SendMessage](ApiClient/SendMessage.md)(…) | Passthrough SendMessage Method for Api Extensions, eg: Recorder. |

## See Also

* namespace [gdio.unity_api.v2](../gdio.unity_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unity_api.dll -->
