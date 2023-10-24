# ApiClient.ClickEx method (1 of 3)

Use this function to interact with an in-game object or UI items using mouse-clicks combined with modifier key press operations. The total frame count of this operation is clickFrameCount + modifiersNumberOfFrames

```csharp
public bool ClickEx(MouseButtons buttonId, ulong clickFrameCount, Vector2 position, 
    KeyCode[] modifiers = null, ulong modifiersNumberOfFrames = 3, int timeout = 30)
```

| parameter | description |
| --- | --- |
| buttonId | The mouse button to use for the click operation. See MouseButtons. |
| clickFrameCount | The number of frames to click the specific position. |
| position | The Vector2 position to perform the mouse click. |
| modifiers | An array of [`KeyCode`](../../gdio.unity_api/KeyCode.md) modifier keys to press during the click operation. |
| modifiersNumberOfFrames | The number of frames to press the modifier keys parameter down. This parameter is not additive to the total count and is automatically accumulated by the function call. |
| timeout | The number of seconds to wait for a response that the ClickEx request was processed. Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

## Examples

```csharp
//Clicks the left mouse button at coordinates 0,0 for 10 frames while holding the left-shift key for 3 frames longer.
            api.ClickEx(MouseButtons.LEFT, 10, new Vector2(0, 0), new KeyCode[] { KeyCode.LeftShift }, 3, 30);
```

## See Also

* enum [KeyCode](../../gdio.unity_api/KeyCode.md)
* class [ApiClient](../ApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

---

# ApiClient.ClickEx method (2 of 3)

Use this function to perform in-game mouse-clicks combined with key press operations. The total frame count of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames

```csharp
public bool ClickEx(MouseButtons buttonId, Vector2 position, ulong clickFrameCount, 
    KeyCode[] keys = null, ulong keysNumberOfFrames = 5, KeyCode[] modifiers = null, 
    ulong modifiersNumberOfFrames = 3, int delayAfterModifiersMsec = 500, int timeout = 30)
```

| parameter | description |
| --- | --- |
| buttonId | The mouse button to use for the click operation. See MouseButtons. |
| position | The Vector2 position to perform the mouse click. |
| clickFrameCount | The number of frames to click the specific position. |
| keys | An array of [`KeyCode`](../../gdio.unity_api/KeyCode.md) keys to press during the click operation. |
| keysNumberOfFrames | The number of frames to press the keys parameter down. This parameter is not additive to the total count and is automatically accumulated by the function call. |
| modifiers | An array of [`KeyCode`](../../gdio.unity_api/KeyCode.md) modifier keys to press during the click operation. |
| modifiersNumberOfFrames | The number of frames to press the modifier keys parameter down. This parameter is not additive to the total count and is automatically accumulated by the function call. |
| delayAfterModifiersMsec | Total time in milliseconds to wait after pressing modifier keys, before clicking the object. This is needed when a delay is required to register the modifier keys have been pressed in game. If this delay is longer than that of the frame count for all of the key presses and click operations, the resulting behavior may not be what the user intends. |
| timeout | The number of seconds to wait for a response that the ClickEx request was processed. Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

## Examples

```csharp
//Clicks the left mouse button at 0,0 for 30 frames while holding the left-shift key for 3 frames, and the C key for 5 frames.
            api.ClickEx(MouseButtons.LEFT, new Vector2(0, 0), 30, new KeyCode[] { KeyCode.C }, 5, new KeyCode[] { KeyCode.LeftShift }, 3, 500, 30);
```

## See Also

* enum [KeyCode](../../gdio.unity_api/KeyCode.md)
* class [ApiClient](../ApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

---

# ApiClient.ClickEx method (3 of 3)

Use this function to perform in game mouse-clicks combined with key press operations. The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames.

```csharp
public bool ClickEx(MouseButtons buttonId, float x, float y, ulong clickFrameCount, 
    KeyCode[] keys = null, ulong keysNumberOfFrames = 5, KeyCode[] modifiers = null, 
    ulong modifiersNumberOfFrames = 3, int delayAfterModifiersMsec = 500, int timeout = 30)
```

| parameter | description |
| --- | --- |
| buttonId | The mouse button to use for the click operation. See MouseButtons. |
| x | The X coordinate of the game to click in Screen space. |
| y | The Y coordinate of the game to click in Screen space. |
| clickFrameCount | The number of frames to click the specific position. |
| keys | An array of [`KeyCode`](../../gdio.unity_api/KeyCode.md) keys to press during the click operation. |
| keysNumberOfFrames | The number of frames to press the keys parameter down. This parameter is not additive to the total count and is automatically accumulated by the function call. |
| modifiers | An array of [`KeyCode`](../../gdio.unity_api/KeyCode.md) modifier keys to press during the click operation. |
| modifiersNumberOfFrames | The number of frames to press the modifier keys parameter down. This parameter is not additive to the total count and is automatically accumulated by the function call. |
| delayAfterModifiersMsec | Total time in milliseconds to wait after pressing modifier keys, before clicking the object. This is needed when a delay is required to register the modifier keys have been pressed in the game. If this delay is longer than that of the frame count for all of the key presses and click operations, the resulting behavior may not be what the user intends. |
| timeout | The number of seconds to wait for a response that the ClickEx request was processed. Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

## Examples

```csharp
//Clicks the left mouse button at 0,0 for 30 frames while holding the left-shift key for 3 frames, and the C key for 5 frames.
            api.ClickEx(MouseButtons.LEFT, 0, 0, 30,
                new KeyCode[] { KeyCode.C }, 5,
                new KeyCode[] { KeyCode.LeftShift }, 3,
                500, 30);
```

## See Also

* enum [KeyCode](../../gdio.unity_api/KeyCode.md)
* class [ApiClient](../ApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unity_api.dll -->
