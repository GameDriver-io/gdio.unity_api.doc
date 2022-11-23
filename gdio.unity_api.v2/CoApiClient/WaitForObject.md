# CoApiClient.WaitForObject method

Wait for an object to exist.

```csharp
public IEnumerator<bool> WaitForObject(string hierarchyPath, int timeout = 30)
```

| parameter | description |
| --- | --- |
| hierarchyPath | The HierarchyPath of the object. |
| timeout | The amount of time to wait for the object to exist. |

## Return Value

Returns TRUE if the object exists within the alloted timeout.

## See Also

* class [CoApiClient](../CoApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unity_api.dll -->