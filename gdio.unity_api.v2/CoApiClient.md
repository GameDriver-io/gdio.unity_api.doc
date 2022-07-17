# CoApiClient class

```csharp
public class CoApiClient
```

## Public Members

| name | description |
| --- | --- |
| [CoApiClient](CoApiClient/CoApiClient.md)() | The default constructor. |
| event [LoggedMessage](CoApiClient/LoggedMessage.md) |  |
| [CallMethod&lt;T&gt;](CoApiClient/CallMethod.md)(…) | Use this function to execute a method on an object. |
| [CaptureScreenshot](CoApiClient/CaptureScreenshot.md)(…) | Use this function to capture a screenshot of the Game under test. |
| [Click](CoApiClient/Click.md)(…) | Use this function to perform in-game mouse-clicks. (2 methods) |
| [ClickEx](CoApiClient/ClickEx.md)(…) | Use this function to perform in-game mouse-clicks combined with key press operations. The total frame count of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames (2 methods) |
| [ClickObject](CoApiClient/ClickObject.md)(…) | Use this function to interact with an in-game object using mouse-clicks. |
| [ClickObjectEx](CoApiClient/ClickObjectEx.md)(…) | Use this function to interact with an in-game object using mouse-clicks combined with key press operations. The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames. |
| [Connect](CoApiClient/Connect.md)() | Use this function to connect to a Unity game with GameDriver Agent configured and active. This function can connect to only the UnityEditor, and must be used within the Unity Test Runner. |
| [Connect](CoApiClient/Connect.md)(…) | Use this function to connect to a Unity game with GameDriver Agent configured and active. This function can connect to the UnityEditor or a Standalone deployment of a game. |
| [DisableHooks](CoApiClient/DisableHooks.md)(…) | Disable input hooks in the game. |
| [EnableHooks](CoApiClient/EnableHooks.md)(…) | Enable input hooks in the game, which is required to perform various input types during replay. |
| [EnableObjectCaching](CoApiClient/EnableObjectCaching.md)(…) | Enable the use of object caching when performing HierarchyPath object resolution. Object caching is per HierarchyPath stored in a IDictionary. If a matching HierarchyPath is already in the dictionary, then the stored object is returned. The only way to update a cached reference is for the reference to be garbage collected or flush the cache with [`FlushObjectLookupCache`](./ApiClient/FlushObjectLookupCache.md). |
| [FlushObjectLookupCache](CoApiClient/FlushObjectLookupCache.md)(…) | If object caching is enabled, this method will request that the agent flush the cache being held for all object lookups. |
| [GetLastFPS](CoApiClient/GetLastFPS.md)() | This method returns the last frames per second that the API client has recieved from the GameDriver agent. |
| [GetNextCollisionEvent&lt;T&gt;](CoApiClient/GetNextCollisionEvent.md)(…) | Collision events are stored in a FIFO queue. Calling this method returns the next collision event that was returned. |
| [GetObjectDistance](CoApiClient/GetObjectDistance.md)(…) | This method returns the distance of two objects using vector subtraction. |
| [GetObjectFieldValue&lt;T&gt;](CoApiClient/GetObjectFieldValue.md)(…) | This method returns the field or property value of an object. (2 methods) |
| [GetObjectList](CoApiClient/GetObjectList.md)(…) | This method returns of a list of all GameObjects as returned by !:UnityEngine.GameObject.FindObjectsOfType(Type), where Type is UnityEngine.GameObject./&gt; |
| [GetObjectPosition](CoApiClient/GetObjectPosition.md)(…) | Return the position of a specific object. |
| [GetSceneName](CoApiClient/GetSceneName.md)(…) | Return the name of the current active scene. |
| [KeyPress](CoApiClient/KeyPress.md)(…) | Use this function to send arbitrary button states to the game. Defaults to LEFT ALT/CTRL/SHIFT/WINDOWS(COMMAND) |
| [LoadScene](CoApiClient/LoadScene.md)(…) | This method loads the scene, defined by the scene name passed as an argument. |
| [MouseDrag](CoApiClient/MouseDrag.md)(…) | Perform a mouse drag operation. |
| [MouseMoveToObject](CoApiClient/MouseMoveToObject.md)(…) | Move the mouse to the center of a specific object, identified by the HierarchyPath. |
| [MoveMouseToPoint](CoApiClient/MoveMouseToPoint.md)(…) | Move the mouse to the destination vector. |
| [NavAgentMoveToPoint](CoApiClient/NavAgentMoveToPoint.md)(…) | Move a NavAgent to a destination point. |
| [Raycast](CoApiClient/Raycast.md)(…) | Perform a Raycast to a point to find out what is in that position. |
| [RegisterCollisionMonitor](CoApiClient/RegisterCollisionMonitor.md)(…) | Register a collision monitor to recieve collision events on an object. |
| [RotateObject](CoApiClient/RotateObject.md)(…) | Rotate an object defined by the HierarchyPath and rotated by a Quaternion. [https://scriptinghelpers.org/blog/how-to-think-about-quaternions](https://scriptinghelpers.org/blog/how-to-think-about-quaternions) for more information. (4 methods) |
| [SetInputFieldText](CoApiClient/SetInputFieldText.md)(…) | Set the text of an InputField or TMP_InputField |
| [SetObjectFieldValue](CoApiClient/SetObjectFieldValue.md)(…) | Set the field or property of an object. |
| [Tap](CoApiClient/Tap.md)(…) | Tap the handheld device at the defined position. (2 methods) |
| [TapObject](CoApiClient/TapObject.md)(…) | Tap an object. |
| [TouchInput](CoApiClient/TouchInput.md)(…) | Send a raw TouchInput event to the game. (2 methods) |
| [UnregisterCollisionMonitor](CoApiClient/UnregisterCollisionMonitor.md)(…) | Unregister the monitoring of collision events on a GameObject that has been previously registered for monitoring. |
| [Wait](CoApiClient/Wait.md)(…) | Wait for a fixed period of seconds. |
| [WaitForCollisionEvent](CoApiClient/WaitForCollisionEvent.md)(…) | Wait for a collision event to fire on an element that is being monitored for collisions. |
| [WaitForCollisionEvent&lt;T&gt;](CoApiClient/WaitForCollisionEvent.md)(…) | Wait for a collision event to fire on an element that is being monitored for collisions. If the method has been called before, there is the potential that another event was recieved before waiting on the event again. Check with [`GetNextCollisionEvent`](./CoApiClient/GetNextCollisionEvent.md) to see if it returns null to see if an event was missed. |
| [WaitForEmptyInput](CoApiClient/WaitForEmptyInput.md)(…) | Wait for an Empty Input event to be received. |
| [WaitForFixedUpdate](CoApiClient/WaitForFixedUpdate.md)() | Wait for a fixed update in the UnityEngine game loop. |
| [WaitForObject](CoApiClient/WaitForObject.md)(…) | Wait for an object to exist. |
| [WaitForObjectValue](CoApiClient/WaitForObjectValue.md)(…) | Wait for an object to exist and have a specific value for a specified field/property. |
| static [THROW_EXCEPTIONS](CoApiClient/THROW_EXCEPTIONS.md) |  |
| static [GetVersionsString](CoApiClient/GetVersionsString.md)() | Returns the GameDriver component versions in this build. |

## See Also

* namespace [gdio.unity_api.v2](../gdio.unity_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unity_api.dll -->
