# ApiClient.DoubleClickEx method (1 of 2)

Use this function to perform in game mouse double clicks combined with key press operations. The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames

```csharp
public bool DoubleClickEx(MouseButtons buttonId, Vector2 position, ulong clickFrameCount, 
    KeyCode[] keys = null, ulong keysNumberOfFrames = 5, KeyCode[] modifiers = null, 
    ulong modifiersNumberOfFrames = 3, int delayAfterModifiersMsec = 500, int timeout = 30)
```

| parameter | description |
| --- | --- |
| buttonId | The mouse button to use for the click operation. See MouseButtons. |
| position | The Vector2 position of where to double click in Screen space. |
| clickFrameCount | The number of frames to click the specific position. |
| keys | An array of [`KeyCode`](../../gdio.unity_api/KeyCode.md) keys to press during the click operation. |
| keysNumberOfFrames | The number of frames to press the keys parameter down. This parameter is not additive to the total count and is automatically accumulated by the function call. |
| modifiers | An array of [`KeyCode`](../../gdio.unity_api/KeyCode.md) modifier keys to press during the click operation. |
| modifiersNumberOfFrames | The number of frames to press the modifier keys parameter down. This parameter is not additive to the total count and is automatically accumulated by the function call. |
| delayAfterModifiersMsec | Total time in milliseconds to wait after pressing modifier keys, before clicking the object. This is needed when a delay is required to register the modifier keys have been pressed in the game. If this delay is longer than the frame count for all the key presses and click operation that the behavior of the result may not be what the user intends. |
| timeout | The number of seconds to wait for a response that the ClickEx request was processed. Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

## Return Value

TRUE if the GameDriver agent successfully processed the request.

## Examples

```csharp
//Double-clicks the left mouse button at the position 0, 0 for 30 frames with the left mouse button while holding the left-shift key for 3 frames, and the left-CTRL key for 5 frames.
            api.DoubleClickEx(MouseButtons.LEFT, new Vector2 (0, 0), 30,
                new KeyCode[] { KeyCode.LeftControl }, 5,
                new KeyCode[] { KeyCode.LeftShift }, 3,
                500, 30);
```

## See Also

* enum [KeyCode](../../gdio.unity_api/KeyCode.md)
* class [ApiClient](../ApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

---

# ApiClient.DoubleClickEx method (2 of 2)

Use this function to perform in game mouse double clicks combined with key press operations. The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames

```csharp
public bool DoubleClickEx(MouseButtons buttonId, float x, float y, ulong clickFrameCount, 
    KeyCode[] keys = null, ulong keysNumberOfFrames = 5, KeyCode[] modifiers = null, 
    ulong modifiersNumberOfFrames = 3, int delayAfterModifiersMsec = 500, int timeout = 30)
```

| parameter | description |
| --- | --- |
| buttonId | The mouse button to use for the click operation. See MouseButtons. |
| x | The X coordinate of the game to double click in Screen space. |
| y | The Y coordinate of the game to double click in Screen space. |
| clickFrameCount | The number of frames to click the specific position. |
| keys | An array of [`KeyCode`](../../gdio.unity_api/KeyCode.md) keys to press during the click operation. |
| keysNumberOfFrames | The number of frames to press the keys parameter down. This parameter is not additive to the total count and is automatically accumulated by the function call. |
| modifiers | An array of [`KeyCode`](../../gdio.unity_api/KeyCode.md) modifier keys to press during the click operation. |
| modifiersNumberOfFrames | The number of frames to press the modifier keys parameter down. This parameter is not additive to the total count and is automatically accumulated by the function call. |
| delayAfterModifiersMsec | Total time in milliseconds to wait after pressing modifier keys, before clicking the object. This is needed when a delay is required to register the modifier keys have been pressed in the game. If this delay is longer than the frame count for all the key presses and click operation that the behavior of the result may not be what the user intends. |
| timeout | The number of seconds to wait for a response that the ClickEx request was processed. Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

## Return Value

TRUE if the GameDriver agent successfully processed the request.

## Examples

```csharp
//Double-clicks the left mouse button at the position 0, 0 for 30 frames with the left mouse button while holding the left-shift key for 3 frames, and the left-CTRL key for 5 frames.
            api.DoubleClickEx(MouseButtons.LEFT, 0, 0, 30,
                new KeyCode[] { KeyCode.LeftControl }, 5,
                new KeyCode[] { KeyCode.LeftShift }, 3,
                500, 30);
```

## See Also

* enum [KeyCode](../../gdio.unity_api/KeyCode.md)
* class [ApiClient](../ApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unity_api.dll -->
