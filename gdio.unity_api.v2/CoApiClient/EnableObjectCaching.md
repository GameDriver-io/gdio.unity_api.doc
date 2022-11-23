# CoApiClient.EnableObjectCaching method

Enable the use of object caching when performing HierarchyPath object resolution. Object caching is per HierarchyPath stored in a IDictionary. If a matching HierarchyPath is already in the dictionary, then the stored object is returned. The only way to update a cached reference is for the reference to be garbage collected or flush the cache with [`FlushObjectLookupCache`](../ApiClient/FlushObjectLookupCache.md).

```csharp
public IEnumerator<bool> EnableObjectCaching(int timeout = 30)
```

| parameter | description |
| --- | --- |
| timeout | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

## Return Value

TRUE if the GameDriver agent successfully processed the request.

## Examples

```csharp
api.EnableObjectCaching();
```

## See Also

* class [CoApiClient](../CoApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unity_api.dll -->