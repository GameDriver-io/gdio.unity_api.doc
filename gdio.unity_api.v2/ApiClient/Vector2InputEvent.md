# ApiClient.Vector2InputEvent method

Use this function to send arbitrary Vector2 Event states to the game.

```csharp
public bool Vector2InputEvent(string inputControlPath, Vector2 value, ulong numberOfFrames, 
    int timeout = 30)
```

| parameter | description |
| --- | --- |
| inputControlPath | The Input Control Path for the New Input System |
| value | Value of the Vector2 event |
| numberOfFrames | The number of frames to press and hold the axis for. |
| timeout | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

## Return Value

TRUE if the GameDriver agent successfully processed the request.

## Examples

```csharp
api.Vector2InputEvent("OculusRightHand/Primary2DAxis", new Vector2(0, 1), 2); //Move the right joystick up. 
```

## See Also

* class [ApiClient](../ApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unity_api.dll -->
