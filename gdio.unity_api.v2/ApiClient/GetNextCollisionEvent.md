# ApiClient.GetNextCollisionEvent method

Collision events are stored in a FIFO queue. Calling this method returns the next collision event that was returned.

```csharp
public Collision GetNextCollisionEvent(string eventId)
```

| parameter | description |
| --- | --- |
| eventId | The eventId returned from [`RegisterCollisionMonitor`](./RegisterCollisionMonitor.md) |

## Return Value

The Collision event next in the FIFO queue of events recieved. NULL is returned if the eventId doesn't match a Collision event or if no new event is available in the queue.

## See Also

* class [ApiClient](../ApiClient.md)
* namespace [gdio.unity_api.v2](../../gdio.unity_api.md)

<!-- DO NOT EDIT: generated by xmldocmd for gdio.unity_api.dll -->
