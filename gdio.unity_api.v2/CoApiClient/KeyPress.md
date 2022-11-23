# CoApiClient.KeyPress method

Use this function to send arbitrary button states to the game. Defaults to LEFT ALT/CTRL/SHIFT/WINDOWS(COMMAND)

```csharp
public IEnumerator<bool> KeyPress(KeyCode[] keys, ulong numberOfFrames, KeyCode[] modifiers = null, 
    ulong modifierNumberOfFrames = 3, int delayAfterModifiersMsec = 500, int timeout = 30)
```

| parameter | description |
| --- | --- |
| keys | An array of keys([`KeyCode`](../../gdio.unity_api/KeyCode.md)) to press. |
| numberOfFrames | The number of frames to press and hold the keys for. |
| modifiers | An array of modifiers()[`KeyCode`](../../gdio.unity_api/KeyCode.md) to press. |
| modifierNumberOfFrames | The number of frames to hold the modifiers down for, before pressing the keys. |
| delayAfterModifiersMsec | The delay to wait between holding the modifies and pressing the keys. |
| timeout | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

## Return Value

TRUE if the GameDriver agent successfully processed the request.

## Examples

```csharp
//Press the down, left, up, then right keys in sequence
            api.KeyPress(new KeyCode[] { KeyCode.DownArrow}, 100);
            api.Wait(300);
            api.KeyPress(new KeyCode[] { KeyCode.LeftArrow}, 100);
            api.Wait(300);
            api.KeyPress(new KeyCode[] { KeyCode.UpArrow }, 100);
            api.Wait(300);
            api.KeyPress(new KeyCode[] { KeyCode.RightArrow }, 100);
            api.Wait(3000);
```

## See Also

* enum [KeyCode](../../gdio.unity_api/KeyCode.md)
* class [CoApiClient](../CoApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unity_api.dll -->