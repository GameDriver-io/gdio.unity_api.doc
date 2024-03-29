# ApiClient.SkeletonInputEvent method (1 of 2)

Use this function to send arbitrary Skeleton Event states to the game.

```csharp
public bool SkeletonInputEvent(string inputControlPath, Quaternion[] value, ulong numberOfFrames, 
    int timeout = 30)
```

| parameter | description |
| --- | --- |
| inputControlPath | The Input Control Path for the New Input System |
| value | Value of the float[] event |
| numberOfFrames | The number of frames to press and hold the axis for. |
| timeout | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

## Return Value

TRUE if the GameDriver agent successfully processed the request.

## Examples

```csharp
api.SkeletonInputEvent("OculusLeftHand/skeleton", new float[]{0.0f,0.0f,0.0f,0.0f,0.0f}, 2); // Set hand skeleton to fully open hand.
```

## See Also

* class [ApiClient](../ApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

---

# ApiClient.SkeletonInputEvent method (2 of 2)

Use this function to send arbitrary Skeleton Event states to the game.

```csharp
public bool SkeletonInputEvent(string inputControlPath, uint index, Quaternion value, 
    ulong numberOfFrames, int timeout = 30)
```

| parameter | description |
| --- | --- |
| inputControlPath | The Input Control Path for the New Input System |
| index | Index of the bone |
| value | Value of the float event |
| numberOfFrames | The number of frames to press and hold the axis for. |
| timeout | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

## Return Value

TRUE if the GameDriver agent successfully processed the request.

## Examples

```csharp
api.SkeletonInputEvent("OculusLeftHand/skeleton", 2, 0.5f, 0); // Set hand skeleton to fully open hand.
```

## See Also

* class [ApiClient](../ApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unity_api.dll -->
