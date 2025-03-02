# ApiClient.StartVideoRecording method (1 of 3)

Use this function to start a video recording of the screen space viewport.

```csharp
public void StartVideoRecording(float imageScale = 1, float magnification = 1, int timeout = 60)
```

| parameter | description |
| --- | --- |
| imageScale | The factor to multiply the current screen resolution by to get the resolution for the output video |
| magnification | The factor to scale the captured texture by. 2.0f == 2x magnification. Treats the value of *centerOnPosition* as the point magnify towards |
| timeout | The number of seconds to wait for a response |

## Examples

```csharp
// Record a video with half the resolution of the screen
api.StartVideoRecording(0.5f, 1.0f, 60);
api.Wait(3000);
// Save the video local to the test with the name "output.avi" and overwrite if it already exists
api.StopVideoRecording("output", false, FileCollisionOption.UseExisting);
```

## See Also

* class [ApiClient](../ApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

---

# ApiClient.StartVideoRecording method (2 of 3)

Use this function to start a video recording of the screen space viewport. Optionally center the video capture on the position of a game object.

```csharp
public void StartVideoRecording(string trackObjectFromPath, float imageScale = 1, 
    float magnification = 1, int timeout = 60)
```

| parameter | description |
| --- | --- |
| trackObjectFromPath | The hierarchy path of a game object for the capture to be centered on. |
| imageScale | The factor to multiply the current screen resolution by to get the resolution for the output video. |
| magnification | The factor to scale the captured texture by. 2.0f == 2x magnification. Treats the position of the object provided by *trackObjectFromPath* as the point magnify towards. |
| timeout | The number of seconds to wait for a response |

## Examples

```csharp
// Record a video that tracks the Cube object at half resolution with a magnification of 2x.
api.StartVideoRecording("//*[@name='Cube']", 0.5f, 2.0f, 60);
api.Wait(3000);
// Save the video local to the test with the name "output.avi" and overwrite if it already exists
api.StopVideoRecording("output", false, FileCollisionOption.UseExisting);
```

## See Also

* class [ApiClient](../ApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

---

# ApiClient.StartVideoRecording method (3 of 3)

Use this function to start a video recording of the screen space viewport. Optionally center the video capture on a specific screen position.

```csharp
public void StartVideoRecording(Vector2 centerOnPosition, float imageScale = 1, 
    float magnification = 1, int timeout = 60)
```

| parameter | description |
| --- | --- |
| centerOnPosition | The screen-position to center the video capture on. |
| imageScale | The factor to multiply the current screen resolution by to get the resolution for the output video. |
| magnification | The factor to scale the captured texture by. 2.0f == 2x magnification. Treats the value of *centerOnPosition* as the point to magnify towards |
| timeout | The number of seconds to wait for a response |

## Examples

```csharp
// Record a video recording at the 250, 250 coordinates of the screen at half resolution with a magnification of 2x.
api.StartVideoRecording(new Vector2(250, 250) ,0.5f, 2.0f);
api.Wait(3000);
// Save the video local to the test with the name "output.avi" and overwrite if it already exists
api.StopVideoRecording("output", false, FileCollisionOption.UseExisting);
```

## See Also

* class [ApiClient](../ApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unity_api.dll -->
