# ApiClient.GetLastFPS method

This method returns the last frames per second that the API client has recieved from the GameDriver agent.

```csharp
public double GetLastFPS()
```

## Return Value

The last published FPS as a double.

## Examples

```csharp
// Can be used as input for time-sensitive functions such as input.
// For example, this will press the Down key for roughly 1 second:
api.KeyPress(new KeyCode[] { KeyCode.DownArrow }, (ulong)api.GetLastFPS());
```

## See Also

* class [ApiClient](../ApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unity_api.dll -->
