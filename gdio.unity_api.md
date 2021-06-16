<a name='assembly'></a>
# gdio.unity_api

## Contents

- [ApiClient](#T-gdio-unity_api-v2-ApiClient 'gdio.unity_api.v2.ApiClient')
  - [#ctor()](#M-gdio-unity_api-v2-ApiClient-#ctor 'gdio.unity_api.v2.ApiClient.#ctor')
  - [AUTOPLAY_DEFAULT_PORT](#F-gdio-unity_api-v2-ApiClient-AUTOPLAY_DEFAULT_PORT 'gdio.unity_api.v2.ApiClient.AUTOPLAY_DEFAULT_PORT')
  - [AUTOPLAY_ENABLED](#F-gdio-unity_api-v2-ApiClient-AUTOPLAY_ENABLED 'gdio.unity_api.v2.ApiClient.AUTOPLAY_ENABLED')
  - [AUTOPLAY_RECEIVE_PORT](#F-gdio-unity_api-v2-ApiClient-AUTOPLAY_RECEIVE_PORT 'gdio.unity_api.v2.ApiClient.AUTOPLAY_RECEIVE_PORT')
  - [THROW_EXCEPTIONS](#F-gdio-unity_api-v2-ApiClient-THROW_EXCEPTIONS 'gdio.unity_api.v2.ApiClient.THROW_EXCEPTIONS')
  - [AxisPress(axisId,value,numberOfFrames,timeout)](#M-gdio-unity_api-v2-ApiClient-AxisPress-System-String,System-Single,System-UInt64,System-Int32- 'gdio.unity_api.v2.ApiClient.AxisPress(System.String,System.Single,System.UInt64,System.Int32)')
  - [ButtonPress(buttonId,numberOfFrames,timeout)](#M-gdio-unity_api-v2-ApiClient-ButtonPress-System-String,System-UInt64,System-Int32- 'gdio.unity_api.v2.ApiClient.ButtonPress(System.String,System.UInt64,System.Int32)')
  - [CallMethod(hierarchyPath,methodName,arguments,timeout)](#M-gdio-unity_api-v2-ApiClient-CallMethod-System-String,System-String,System-Object[],System-Int32- 'gdio.unity_api.v2.ApiClient.CallMethod(System.String,System.String,System.Object[],System.Int32)')
  - [CallMethod<T>(hierarchyPath,methodName,arguments,timeout)](#M-gdio-unity_api-v2-ApiClient-CallMethod<T>-System-String,System-String,System-Object[],System-Int32- 'gdio.unity_api.v2.ApiClient.CallMethod<T>(System.String,System.String,System.Object[],System.Int32)')
  - [CaptureScreenshot(filename,storeInGameFolder,overwriteExisting,timeout)](#M-gdio-unity_api-v2-ApiClient-CaptureScreenshot-System-String,System-Boolean,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.CaptureScreenshot(System.String,System.Boolean,System.Boolean,System.Int32)')
  - [Click(buttonId,position,clickFrameCount,timeout)](#M-gdio-unity_api-v2-ApiClient-Click-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,System-Int32- 'gdio.unity_api.v2.ApiClient.Click(gdio.common.objects.MouseButtons,gdio.common.objects.Vector2,System.UInt64,System.Int32)')
  - [Click(buttonId,x,y,clickFrameCount,timeout)](#M-gdio-unity_api-v2-ApiClient-Click-gdio-common-objects-MouseButtons,System-Single,System-Single,System-UInt64,System-Int32- 'gdio.unity_api.v2.ApiClient.Click(gdio.common.objects.MouseButtons,System.Single,System.Single,System.UInt64,System.Int32)')
  - [ClickEx(buttonId,position,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout)](#M-gdio-unity_api-v2-ApiClient-ClickEx-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32- 'gdio.unity_api.v2.ApiClient.ClickEx(gdio.common.objects.MouseButtons,gdio.common.objects.Vector2,System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,System.Int32,System.Int32)')
  - [ClickEx(buttonId,x,y,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout)](#M-gdio-unity_api-v2-ApiClient-ClickEx-gdio-common-objects-MouseButtons,System-Single,System-Single,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32- 'gdio.unity_api.v2.ApiClient.ClickEx(gdio.common.objects.MouseButtons,System.Single,System.Single,System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,System.Int32,System.Int32)')
  - [ClickObject(buttonId,hierarchyPath,frameCount,timeout)](#M-gdio-unity_api-v2-ApiClient-ClickObject-gdio-common-objects-MouseButtons,System-String,System-UInt64,System-Int32- 'gdio.unity_api.v2.ApiClient.ClickObject(gdio.common.objects.MouseButtons,System.String,System.UInt64,System.Int32)')
  - [ClickObjectEx(buttonId,hierarchyPath,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout)](#M-gdio-unity_api-v2-ApiClient-ClickObjectEx-gdio-common-objects-MouseButtons,System-String,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32- 'gdio.unity_api.v2.ApiClient.ClickObjectEx(gdio.common.objects.MouseButtons,System.String,System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,System.Int32,System.Int32)')
  - [Connect(hostname,port,autoplay,timeout,autoPortResolution)](#M-gdio-unity_api-v2-ApiClient-Connect-System-String,System-Int32,System-Boolean,System-Int32,System-Boolean- 'gdio.unity_api.v2.ApiClient.Connect(System.String,System.Int32,System.Boolean,System.Int32,System.Boolean)')
  - [Connect(hostname,regex_MatchGamePath,port,autoplay,timeout,autoPortResolution)](#M-gdio-unity_api-v2-ApiClient-Connect-System-String,System-String,System-Int32,System-Boolean,System-Int32,System-Boolean- 'gdio.unity_api.v2.ApiClient.Connect(System.String,System.String,System.Int32,System.Boolean,System.Int32,System.Boolean)')
  - [DisableHooks(hookObject,timeout)](#M-gdio-unity_api-v2-ApiClient-DisableHooks-gdio-unity_api-v2-HookingObject,System-Int32- 'gdio.unity_api.v2.ApiClient.DisableHooks(gdio.unity_api.v2.HookingObject,System.Int32)')
  - [DisbleObjectCaching(timeout)](#M-gdio-unity_api-v2-ApiClient-DisbleObjectCaching-System-Int32- 'gdio.unity_api.v2.ApiClient.DisbleObjectCaching(System.Int32)')
  - [Disconnect()](#M-gdio-unity_api-v2-ApiClient-Disconnect 'gdio.unity_api.v2.ApiClient.Disconnect')
  - [DoubleClick(buttonId,position,clickFrameCount,timeout)](#M-gdio-unity_api-v2-ApiClient-DoubleClick-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,System-Int32- 'gdio.unity_api.v2.ApiClient.DoubleClick(gdio.common.objects.MouseButtons,gdio.common.objects.Vector2,System.UInt64,System.Int32)')
  - [DoubleClick(buttonId,x,y,clickFrameCount,timeout)](#M-gdio-unity_api-v2-ApiClient-DoubleClick-gdio-common-objects-MouseButtons,System-Single,System-Single,System-UInt64,System-Int32- 'gdio.unity_api.v2.ApiClient.DoubleClick(gdio.common.objects.MouseButtons,System.Single,System.Single,System.UInt64,System.Int32)')
  - [DoubleClickEx(buttonId,position,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout)](#M-gdio-unity_api-v2-ApiClient-DoubleClickEx-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32- 'gdio.unity_api.v2.ApiClient.DoubleClickEx(gdio.common.objects.MouseButtons,gdio.common.objects.Vector2,System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,System.Int32,System.Int32)')
  - [DoubleClickEx(buttonId,x,y,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout)](#M-gdio-unity_api-v2-ApiClient-DoubleClickEx-gdio-common-objects-MouseButtons,System-Single,System-Single,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32- 'gdio.unity_api.v2.ApiClient.DoubleClickEx(gdio.common.objects.MouseButtons,System.Single,System.Single,System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,System.Int32,System.Int32)')
  - [DoubleClickObject(buttonId,hierarchyPath,frameCount,timeout)](#M-gdio-unity_api-v2-ApiClient-DoubleClickObject-gdio-common-objects-MouseButtons,System-String,System-UInt64,System-Int32- 'gdio.unity_api.v2.ApiClient.DoubleClickObject(gdio.common.objects.MouseButtons,System.String,System.UInt64,System.Int32)')
  - [DoubleClickObjectEx(buttonId,hierarchyPath,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout)](#M-gdio-unity_api-v2-ApiClient-DoubleClickObjectEx-gdio-common-objects-MouseButtons,System-String,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32- 'gdio.unity_api.v2.ApiClient.DoubleClickObjectEx(gdio.common.objects.MouseButtons,System.String,System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,System.Int32,System.Int32)')
  - [EnableHooks(hookObject,timeout)](#M-gdio-unity_api-v2-ApiClient-EnableHooks-gdio-unity_api-v2-HookingObject,System-Int32- 'gdio.unity_api.v2.ApiClient.EnableHooks(gdio.unity_api.v2.HookingObject,System.Int32)')
  - [EnableObjectCaching(timeout)](#M-gdio-unity_api-v2-ApiClient-EnableObjectCaching-System-Int32- 'gdio.unity_api.v2.ApiClient.EnableObjectCaching(System.Int32)')
  - [FlushObjectLookupCache(timeout)](#M-gdio-unity_api-v2-ApiClient-FlushObjectLookupCache-System-Int32- 'gdio.unity_api.v2.ApiClient.FlushObjectLookupCache(System.Int32)')
  - [GetConnectedGameDetails()](#M-gdio-unity_api-v2-ApiClient-GetConnectedGameDetails 'gdio.unity_api.v2.ApiClient.GetConnectedGameDetails')
  - [GetLastFPS()](#M-gdio-unity_api-v2-ApiClient-GetLastFPS 'gdio.unity_api.v2.ApiClient.GetLastFPS')
  - [GetNextCollisionEvent<T>(eventId)](#M-gdio-unity_api-v2-ApiClient-GetNextCollisionEvent<T>-System-String- 'gdio.unity_api.v2.ApiClient.GetNextCollisionEvent<T>(System.String)')
  - [GetObjectDistance(objectA_HierarchyPath,objectB_HierarchyPath,timeout)](#M-gdio-unity_api-v2-ApiClient-GetObjectDistance-System-String,System-String,System-Int32- 'gdio.unity_api.v2.ApiClient.GetObjectDistance(System.String,System.String,System.Int32)')
  - [GetObjectFieldValue<T>(hierarchyPath,timeout)](#M-gdio-unity_api-v2-ApiClient-GetObjectFieldValue<T>-System-String,System-Int32- 'gdio.unity_api.v2.ApiClient.GetObjectFieldValue<T>(System.String,System.Int32)')
  - [GetObjectFieldValue<T>(hierarchyPath,fieldOrPropertyName,timeout)](#M-gdio-unity_api-v2-ApiClient-GetObjectFieldValue<T>-System-String,System-String,System-Int32- 'gdio.unity_api.v2.ApiClient.GetObjectFieldValue<T>(System.String,System.String,System.Int32)')
  - [GetObjectList(timeout)](#M-gdio-unity_api-v2-ApiClient-GetObjectList-System-Int32- 'gdio.unity_api.v2.ApiClient.GetObjectList(System.Int32)')
  - [GetObjectPosition(objectHierarchyPath,cordSpace,cameraHierarchyPath,timeout)](#M-gdio-unity_api-v2-ApiClient-GetObjectPosition-System-String,gdio-common-objects-CoordinateConversion,System-String,System-Int32- 'gdio.unity_api.v2.ApiClient.GetObjectPosition(System.String,gdio.common.objects.CoordinateConversion,System.String,System.Int32)')
  - [GetSceneName(timeout)](#M-gdio-unity_api-v2-ApiClient-GetSceneName-System-Int32- 'gdio.unity_api.v2.ApiClient.GetSceneName(System.Int32)')
  - [GetVersionsString()](#M-gdio-unity_api-v2-ApiClient-GetVersionsString 'gdio.unity_api.v2.ApiClient.GetVersionsString')
  - [KeyPress(keys,numberOfFrames,modifiers,modifierNumberOfFrames,delayAfterModifiersMsec,timeout)](#M-gdio-unity_api-v2-ApiClient-KeyPress-gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32- 'gdio.unity_api.v2.ApiClient.KeyPress(gdio.unity_api.KeyCode[],System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,System.Int32,System.Int32)')
  - [Launch(filename,arguments)](#M-gdio-unity_api-v2-ApiClient-Launch-System-String,System-String- 'gdio.unity_api.v2.ApiClient.Launch(System.String,System.String)')
  - [LoadScene(sceneName,timeout)](#M-gdio-unity_api-v2-ApiClient-LoadScene-System-String,System-Int32- 'gdio.unity_api.v2.ApiClient.LoadScene(System.String,System.Int32)')
  - [MouseDrag(button,destination,frameCount,origin,waitForEmptyInput,timeout)](#M-gdio-unity_api-v2-ApiClient-MouseDrag-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,gdio-common-objects-Vector2,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.MouseDrag(gdio.common.objects.MouseButtons,gdio.common.objects.Vector2,System.UInt64,gdio.common.objects.Vector2,System.Boolean,System.Int32)')
  - [MouseMoveToObject(objectHierarchyPath,frameCount,waitForObject,waitForEmptyInput,timeout)](#M-gdio-unity_api-v2-ApiClient-MouseMoveToObject-System-String,System-UInt64,System-Boolean,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.MouseMoveToObject(System.String,System.UInt64,System.Boolean,System.Boolean,System.Int32)')
  - [MoveMouseToPoint(destination,frameCount,origin,waitForEmptyInput,timeout)](#M-gdio-unity_api-v2-ApiClient-MoveMouseToPoint-gdio-common-objects-Vector2,System-UInt64,gdio-common-objects-Vector2,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.MoveMouseToPoint(gdio.common.objects.Vector2,System.UInt64,gdio.common.objects.Vector2,System.Boolean,System.Int32)')
  - [NavAgentMoveToPoint(navAgentHierarchyPath,destination,waitForMoveToComplete,timeout)](#M-gdio-unity_api-v2-ApiClient-NavAgentMoveToPoint-System-String,gdio-common-objects-Vector3,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.NavAgentMoveToPoint(System.String,gdio.common.objects.Vector3,System.Boolean,System.Int32)')
  - [Raycast(raycastPoint,cameraHierarchyPath,timeout)](#M-gdio-unity_api-v2-ApiClient-Raycast-gdio-common-objects-Vector3,System-String,System-Int32- 'gdio.unity_api.v2.ApiClient.Raycast(gdio.common.objects.Vector3,System.String,System.Int32)')
  - [RegisterCollisionMonitor(hierarchyPath,timeout)](#M-gdio-unity_api-v2-ApiClient-RegisterCollisionMonitor-System-String,System-Int32- 'gdio.unity_api.v2.ApiClient.RegisterCollisionMonitor(System.String,System.Int32)')
  - [RotateObject(hierarchyPath,quaternion,waitForObject,timeout)](#M-gdio-unity_api-v2-ApiClient-RotateObject-System-String,gdio-common-objects-Quaternion,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.RotateObject(System.String,gdio.common.objects.Quaternion,System.Boolean,System.Int32)')
  - [RotateObject(hierarchyPath,eulers,relativeTo,waitForObject,timeout)](#M-gdio-unity_api-v2-ApiClient-RotateObject-System-String,gdio-common-objects-Vector3,gdio-common-objects-Space,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.RotateObject(System.String,gdio.common.objects.Vector3,gdio.common.objects.Space,System.Boolean,System.Int32)')
  - [RotateObject(hierarchyPath,xAngle,yAngle,zAngle,relativeTo,waitForObject,timeout)](#M-gdio-unity_api-v2-ApiClient-RotateObject-System-String,System-Single,System-Single,System-Single,gdio-common-objects-Space,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.RotateObject(System.String,System.Single,System.Single,System.Single,gdio.common.objects.Space,System.Boolean,System.Int32)')
  - [RotateObject(hierarchyPath,axis,angle,relativeTo,waitForObject,timeout)](#M-gdio-unity_api-v2-ApiClient-RotateObject-System-String,gdio-common-objects-Vector3,System-Single,gdio-common-objects-Space,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.RotateObject(System.String,gdio.common.objects.Vector3,System.Single,gdio.common.objects.Space,System.Boolean,System.Int32)')
  - [SetInputFieldText(hierarchyPath,value,waitForObject,timeout)](#M-gdio-unity_api-v2-ApiClient-SetInputFieldText-System-String,System-String,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.SetInputFieldText(System.String,System.String,System.Boolean,System.Int32)')
  - [SetObjectFieldValue(hierarchyPath,fieldOrPropertyName,value,waitForObject,timeout,valueSerializer)](#M-gdio-unity_api-v2-ApiClient-SetObjectFieldValue-System-String,System-String,System-Object,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.SetObjectFieldValue(System.String,System.String,System.Object,System.Boolean,System.Int32)')
  - [Tap(position,tapCount,frameCount,timeout)](#M-gdio-unity_api-v2-ApiClient-Tap-gdio-common-objects-Vector2,System-Int32,System-UInt64,System-Int32- 'gdio.unity_api.v2.ApiClient.Tap(gdio.common.objects.Vector2,System.Int32,System.UInt64,System.Int32)')
  - [Tap(x,y,tapCount,frameCount,timeout)](#M-gdio-unity_api-v2-ApiClient-Tap-System-Single,System-Single,System-Int32,System-UInt64,System-Int32- 'gdio.unity_api.v2.ApiClient.Tap(System.Single,System.Single,System.Int32,System.UInt64,System.Int32)')
  - [TapObject(hierarchyPath,tapCount,frameCount,timeout)](#M-gdio-unity_api-v2-ApiClient-TapObject-System-String,System-Int32,System-UInt64,System-Int32- 'gdio.unity_api.v2.ApiClient.TapObject(System.String,System.Int32,System.UInt64,System.Int32)')
  - [TouchInput(startPosition,destinationPosition,fingerId,tapCount,frameCount,waitForEmptyInput,radius,pressure,altitudeAngle,azmulthAngle,maximumPossiblePressure,timeout)](#M-gdio-unity_api-v2-ApiClient-TouchInput-gdio-common-objects-Vector2,gdio-common-objects-Vector2,System-Int32,System-Int32,System-UInt64,System-Boolean,System-Single,System-Single,System-Single,System-Single,System-Single,System-Int32- 'gdio.unity_api.v2.ApiClient.TouchInput(gdio.common.objects.Vector2,gdio.common.objects.Vector2,System.Int32,System.Int32,System.UInt64,System.Boolean,System.Single,System.Single,System.Single,System.Single,System.Single,System.Int32)')
  - [TouchInput(x1,y1,x2,y2,fingerId,tapCount,frameCount,waitForEmptyInput,radius,pressure,altitudeAngle,azmulthAngle,maximumPossiblePressure,timeout)](#M-gdio-unity_api-v2-ApiClient-TouchInput-System-Single,System-Single,System-Single,System-Single,System-Int32,System-Int32,System-UInt64,System-Boolean,System-Single,System-Single,System-Single,System-Single,System-Single,System-Int32- 'gdio.unity_api.v2.ApiClient.TouchInput(System.Single,System.Single,System.Single,System.Single,System.Int32,System.Int32,System.UInt64,System.Boolean,System.Single,System.Single,System.Single,System.Single,System.Single,System.Int32)')
  - [UnregisterCollisionMonitor(hierarchyPath,timeout)](#M-gdio-unity_api-v2-ApiClient-UnregisterCollisionMonitor-System-String,System-Int32- 'gdio.unity_api.v2.ApiClient.UnregisterCollisionMonitor(System.String,System.Int32)')
  - [Wait(milliSeconds)](#M-gdio-unity_api-v2-ApiClient-Wait-System-Int32- 'gdio.unity_api.v2.ApiClient.Wait(System.Int32)')
  - [WaitForCollisionEvent(eventId,timeout)](#M-gdio-unity_api-v2-ApiClient-WaitForCollisionEvent-System-String,System-Int32- 'gdio.unity_api.v2.ApiClient.WaitForCollisionEvent(System.String,System.Int32)')
  - [WaitForCollisionEvent<T>(eventId,timeout)](#M-gdio-unity_api-v2-ApiClient-WaitForCollisionEvent<T>-System-String,System-Int32- 'gdio.unity_api.v2.ApiClient.WaitForCollisionEvent<T>(System.String,System.Int32)')
  - [WaitForEmptyInput(timeout)](#M-gdio-unity_api-v2-ApiClient-WaitForEmptyInput-System-Int32- 'gdio.unity_api.v2.ApiClient.WaitForEmptyInput(System.Int32)')
  - [WaitForObject(hierarchyPath,timeout)](#M-gdio-unity_api-v2-ApiClient-WaitForObject-System-String,System-Int32- 'gdio.unity_api.v2.ApiClient.WaitForObject(System.String,System.Int32)')
  - [WaitForObjectValue(hierarchyPath,fieldOrPropertyName,value,waitForObject,timeout,valueSerializer)](#M-gdio-unity_api-v2-ApiClient-WaitForObjectValue-System-String,System-String,System-Object,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.WaitForObjectValue(System.String,System.String,System.Object,System.Boolean,System.Int32)')
- [CoApiClient](#T-gdio-unity_api-v2-CoApiClient 'gdio.unity_api.v2.CoApiClient')
  - [CallMethod<T>(hierarchyPath,methodName,arguments,timeout)](#M-gdio-unity_api-v2-CoApiClient-CallMethod<T>-System-String,System-String,System-Object[],System-Int32- 'gdio.unity_api.v2.CoApiClient.CallMethod<T>(System.String,System.String,System.Object[],System.Int32)')
  - [CaptureScreenshot(filename,storeInGameFolder,overwriteExisting,timeout)](#M-gdio-unity_api-v2-CoApiClient-CaptureScreenshot-System-String,System-Boolean,System-Boolean,System-Int32- 'gdio.unity_api.v2.CoApiClient.CaptureScreenshot(System.String,System.Boolean,System.Boolean,System.Int32)')
  - [Click(buttonId,position,clickFrameCount,timeout)](#M-gdio-unity_api-v2-CoApiClient-Click-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,System-Int32- 'gdio.unity_api.v2.CoApiClient.Click(gdio.common.objects.MouseButtons,gdio.common.objects.Vector2,System.UInt64,System.Int32)')
  - [Click(buttonId,x,y,clickFrameCount,timeout)](#M-gdio-unity_api-v2-CoApiClient-Click-gdio-common-objects-MouseButtons,System-Single,System-Single,System-UInt64,System-Int32- 'gdio.unity_api.v2.CoApiClient.Click(gdio.common.objects.MouseButtons,System.Single,System.Single,System.UInt64,System.Int32)')
  - [ClickEx(buttonId,position,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout)](#M-gdio-unity_api-v2-CoApiClient-ClickEx-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32- 'gdio.unity_api.v2.CoApiClient.ClickEx(gdio.common.objects.MouseButtons,gdio.common.objects.Vector2,System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,System.Int32,System.Int32)')
  - [ClickEx(buttonId,x,y,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout)](#M-gdio-unity_api-v2-CoApiClient-ClickEx-gdio-common-objects-MouseButtons,System-Single,System-Single,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32- 'gdio.unity_api.v2.CoApiClient.ClickEx(gdio.common.objects.MouseButtons,System.Single,System.Single,System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,System.Int32,System.Int32)')
  - [ClickObject(buttonId,hierarchyPath,frameCount,timeout)](#M-gdio-unity_api-v2-CoApiClient-ClickObject-gdio-common-objects-MouseButtons,System-String,System-UInt64,System-Int32- 'gdio.unity_api.v2.CoApiClient.ClickObject(gdio.common.objects.MouseButtons,System.String,System.UInt64,System.Int32)')
  - [ClickObjectEx(buttonId,hierarchyPath,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout)](#M-gdio-unity_api-v2-CoApiClient-ClickObjectEx-gdio-common-objects-MouseButtons,System-String,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32- 'gdio.unity_api.v2.CoApiClient.ClickObjectEx(gdio.common.objects.MouseButtons,System.String,System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,System.Int32,System.Int32)')
  - [Connect(hostname,port,timeout)](#M-gdio-unity_api-v2-CoApiClient-Connect-System-String,System-Int32,System-Int32- 'gdio.unity_api.v2.CoApiClient.Connect(System.String,System.Int32,System.Int32)')
  - [DisableHooks(hookObject,timeout)](#M-gdio-unity_api-v2-CoApiClient-DisableHooks-gdio-unity_api-v2-HookingObject,System-Int32- 'gdio.unity_api.v2.CoApiClient.DisableHooks(gdio.unity_api.v2.HookingObject,System.Int32)')
  - [EnableHooks(hookObject,timeout)](#M-gdio-unity_api-v2-CoApiClient-EnableHooks-gdio-unity_api-v2-HookingObject,System-Int32- 'gdio.unity_api.v2.CoApiClient.EnableHooks(gdio.unity_api.v2.HookingObject,System.Int32)')
  - [EnableObjectCaching(timeout)](#M-gdio-unity_api-v2-CoApiClient-EnableObjectCaching-System-Int32- 'gdio.unity_api.v2.CoApiClient.EnableObjectCaching(System.Int32)')
  - [FlushObjectLookupCache(timeout)](#M-gdio-unity_api-v2-CoApiClient-FlushObjectLookupCache-System-Int32- 'gdio.unity_api.v2.CoApiClient.FlushObjectLookupCache(System.Int32)')
  - [GetLastFPS()](#M-gdio-unity_api-v2-CoApiClient-GetLastFPS 'gdio.unity_api.v2.CoApiClient.GetLastFPS')
  - [GetNextCollisionEvent<T>(eventId)](#M-gdio-unity_api-v2-CoApiClient-GetNextCollisionEvent<T>-System-String- 'gdio.unity_api.v2.CoApiClient.GetNextCollisionEvent<T>(System.String)')
  - [GetObjectDistance(objectA_HierarchyPath,objectB_HierarchyPath,timeout)](#M-gdio-unity_api-v2-CoApiClient-GetObjectDistance-System-String,System-String,System-Int32- 'gdio.unity_api.v2.CoApiClient.GetObjectDistance(System.String,System.String,System.Int32)')
  - [GetObjectFieldValue<T>(hierarchyPath,timeout)](#M-gdio-unity_api-v2-CoApiClient-GetObjectFieldValue<T>-System-String,System-Int32- 'gdio.unity_api.v2.CoApiClient.GetObjectFieldValue<T>(System.String,System.Int32)')
  - [GetObjectFieldValue<T>(hierarchyPath,fieldOrPropertyName,timeout)](#M-gdio-unity_api-v2-CoApiClient-GetObjectFieldValue<T>-System-String,System-String,System-Int32- 'gdio.unity_api.v2.CoApiClient.GetObjectFieldValue<T>(System.String,System.String,System.Int32)')
  - [GetObjectList(timeout)](#M-gdio-unity_api-v2-CoApiClient-GetObjectList-System-Int32- 'gdio.unity_api.v2.CoApiClient.GetObjectList(System.Int32)')
  - [GetObjectPosition(objectHierarchyPath,cordSpace,cameraHierarchyPath,timeout)](#M-gdio-unity_api-v2-CoApiClient-GetObjectPosition-System-String,gdio-common-objects-CoordinateConversion,System-String,System-Int32- 'gdio.unity_api.v2.CoApiClient.GetObjectPosition(System.String,gdio.common.objects.CoordinateConversion,System.String,System.Int32)')
  - [GetSceneName(timeout)](#M-gdio-unity_api-v2-CoApiClient-GetSceneName-System-Int32- 'gdio.unity_api.v2.CoApiClient.GetSceneName(System.Int32)')
  - [GetVersionsString()](#M-gdio-unity_api-v2-CoApiClient-GetVersionsString 'gdio.unity_api.v2.CoApiClient.GetVersionsString')
  - [KeyPress(keys,numberOfFrames,modifiers,modifierNumberOfFrames,delayAfterModifiersMsec,timeout)](#M-gdio-unity_api-v2-CoApiClient-KeyPress-gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32- 'gdio.unity_api.v2.CoApiClient.KeyPress(gdio.unity_api.KeyCode[],System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,System.Int32,System.Int32)')
  - [LoadScene(sceneName,timeout)](#M-gdio-unity_api-v2-CoApiClient-LoadScene-System-String,System-Int32- 'gdio.unity_api.v2.CoApiClient.LoadScene(System.String,System.Int32)')
  - [MouseDrag(button,destination,frameCount,origin,waitForEmptyInput,timeout)](#M-gdio-unity_api-v2-CoApiClient-MouseDrag-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,gdio-common-objects-Vector2,System-Boolean,System-Int32- 'gdio.unity_api.v2.CoApiClient.MouseDrag(gdio.common.objects.MouseButtons,gdio.common.objects.Vector2,System.UInt64,gdio.common.objects.Vector2,System.Boolean,System.Int32)')
  - [MouseMoveToObject(objectHierarchyPath,frameCount,waitForObject,waitForEmptyInput,timeout)](#M-gdio-unity_api-v2-CoApiClient-MouseMoveToObject-System-String,System-UInt64,System-Boolean,System-Boolean,System-Int32- 'gdio.unity_api.v2.CoApiClient.MouseMoveToObject(System.String,System.UInt64,System.Boolean,System.Boolean,System.Int32)')
  - [MoveMouseToPoint(destination,frameCount,origin,waitForEmptyInput,timeout)](#M-gdio-unity_api-v2-CoApiClient-MoveMouseToPoint-gdio-common-objects-Vector2,System-UInt64,gdio-common-objects-Vector2,System-Boolean,System-Int32- 'gdio.unity_api.v2.CoApiClient.MoveMouseToPoint(gdio.common.objects.Vector2,System.UInt64,gdio.common.objects.Vector2,System.Boolean,System.Int32)')
  - [NavAgentMoveToPoint(navAgentHierarchyPath,destination,waitForMoveToComplete,timeout)](#M-gdio-unity_api-v2-CoApiClient-NavAgentMoveToPoint-System-String,gdio-common-objects-Vector3,System-Boolean,System-Int32- 'gdio.unity_api.v2.CoApiClient.NavAgentMoveToPoint(System.String,gdio.common.objects.Vector3,System.Boolean,System.Int32)')
  - [Raycast(raycastPoint,cameraHierarchyPath,timeout)](#M-gdio-unity_api-v2-CoApiClient-Raycast-gdio-common-objects-Vector3,System-String,System-Int32- 'gdio.unity_api.v2.CoApiClient.Raycast(gdio.common.objects.Vector3,System.String,System.Int32)')
  - [RegisterCollisionMonitor(hierarchyPath,timeout)](#M-gdio-unity_api-v2-CoApiClient-RegisterCollisionMonitor-System-String,System-Int32- 'gdio.unity_api.v2.CoApiClient.RegisterCollisionMonitor(System.String,System.Int32)')
  - [RotateObject(hierarchyPath,quaternion,waitForObject,timeout)](#M-gdio-unity_api-v2-CoApiClient-RotateObject-System-String,gdio-common-objects-Quaternion,System-Boolean,System-Int32- 'gdio.unity_api.v2.CoApiClient.RotateObject(System.String,gdio.common.objects.Quaternion,System.Boolean,System.Int32)')
  - [RotateObject(hierarchyPath,eulers,relativeTo,waitForObject,timeout)](#M-gdio-unity_api-v2-CoApiClient-RotateObject-System-String,gdio-common-objects-Vector3,gdio-common-objects-Space,System-Boolean,System-Int32- 'gdio.unity_api.v2.CoApiClient.RotateObject(System.String,gdio.common.objects.Vector3,gdio.common.objects.Space,System.Boolean,System.Int32)')
  - [RotateObject(hierarchyPath,xAngle,yAngle,zAngle,relativeTo,waitForObject,timeout)](#M-gdio-unity_api-v2-CoApiClient-RotateObject-System-String,System-Single,System-Single,System-Single,gdio-common-objects-Space,System-Boolean,System-Int32- 'gdio.unity_api.v2.CoApiClient.RotateObject(System.String,System.Single,System.Single,System.Single,gdio.common.objects.Space,System.Boolean,System.Int32)')
  - [RotateObject(hierarchyPath,axis,angle,relativeTo,waitForObject,timeout)](#M-gdio-unity_api-v2-CoApiClient-RotateObject-System-String,gdio-common-objects-Vector3,System-Single,gdio-common-objects-Space,System-Boolean,System-Int32- 'gdio.unity_api.v2.CoApiClient.RotateObject(System.String,gdio.common.objects.Vector3,System.Single,gdio.common.objects.Space,System.Boolean,System.Int32)')
  - [SetInputFieldText(hierarchyPath,value,waitForObject,timeout)](#M-gdio-unity_api-v2-CoApiClient-SetInputFieldText-System-String,System-String,System-Boolean,System-Int32- 'gdio.unity_api.v2.CoApiClient.SetInputFieldText(System.String,System.String,System.Boolean,System.Int32)')
  - [SetObjectFieldValue(hierarchyPath,fieldOrPropertyName,value,waitForObject,timeout,valueSerializer)](#M-gdio-unity_api-v2-CoApiClient-SetObjectFieldValue-System-String,System-String,System-Object,System-Boolean,System-Int32,gdio-plugin-serializer-ICustomSerializer- 'gdio.unity_api.v2.CoApiClient.SetObjectFieldValue(System.String,System.String,System.Object,System.Boolean,System.Int32,gdio.plugin.serializer.ICustomSerializer)')
  - [Tap(position,tapCount,frameCount,timeout)](#M-gdio-unity_api-v2-CoApiClient-Tap-gdio-common-objects-Vector2,System-Int32,System-UInt64,System-Int32- 'gdio.unity_api.v2.CoApiClient.Tap(gdio.common.objects.Vector2,System.Int32,System.UInt64,System.Int32)')
  - [Tap(x,y,tapCount,frameCount,timeout)](#M-gdio-unity_api-v2-CoApiClient-Tap-System-Single,System-Single,System-Int32,System-UInt64,System-Int32- 'gdio.unity_api.v2.CoApiClient.Tap(System.Single,System.Single,System.Int32,System.UInt64,System.Int32)')
  - [TapObject(hierarchyPath,tapCount,frameCount,timeout)](#M-gdio-unity_api-v2-CoApiClient-TapObject-System-String,System-Int32,System-UInt64,System-Int32- 'gdio.unity_api.v2.CoApiClient.TapObject(System.String,System.Int32,System.UInt64,System.Int32)')
  - [TouchInput(startPosition,destinationPosition,fingerId,tapCount,frameCount,waitForEmptyInput,radius,pressure,altitudeAngle,azmulthAngle,maximumPossiblePressure,timeout)](#M-gdio-unity_api-v2-CoApiClient-TouchInput-gdio-common-objects-Vector2,gdio-common-objects-Vector2,System-Int32,System-Int32,System-UInt64,System-Boolean,System-Single,System-Single,System-Single,System-Single,System-Single,System-Int32- 'gdio.unity_api.v2.CoApiClient.TouchInput(gdio.common.objects.Vector2,gdio.common.objects.Vector2,System.Int32,System.Int32,System.UInt64,System.Boolean,System.Single,System.Single,System.Single,System.Single,System.Single,System.Int32)')
  - [TouchInput(x1,y1,x2,y2,fingerId,tapCount,frameCount,waitForEmptyInput,radius,pressure,altitudeAngle,azmulthAngle,maximumPossiblePressure,timeout)](#M-gdio-unity_api-v2-CoApiClient-TouchInput-System-Single,System-Single,System-Single,System-Single,System-Int32,System-Int32,System-UInt64,System-Boolean,System-Single,System-Single,System-Single,System-Single,System-Single,System-Int32- 'gdio.unity_api.v2.CoApiClient.TouchInput(System.Single,System.Single,System.Single,System.Single,System.Int32,System.Int32,System.UInt64,System.Boolean,System.Single,System.Single,System.Single,System.Single,System.Single,System.Int32)')
  - [UnregisterCollisionMonitor(hierarchyPath,timeout)](#M-gdio-unity_api-v2-CoApiClient-UnregisterCollisionMonitor-System-String,System-Int32- 'gdio.unity_api.v2.CoApiClient.UnregisterCollisionMonitor(System.String,System.Int32)')
  - [Wait(waitMaxSeconds)](#M-gdio-unity_api-v2-CoApiClient-Wait-System-Single- 'gdio.unity_api.v2.CoApiClient.Wait(System.Single)')
  - [WaitForCollisionEvent(eventId,timeout)](#M-gdio-unity_api-v2-CoApiClient-WaitForCollisionEvent-System-String,System-Int32- 'gdio.unity_api.v2.CoApiClient.WaitForCollisionEvent(System.String,System.Int32)')
  - [WaitForCollisionEvent<T>(eventId,timeout)](#M-gdio-unity_api-v2-CoApiClient-WaitForCollisionEvent<T>-System-String,System-Int32- 'gdio.unity_api.v2.CoApiClient.WaitForCollisionEvent<T>(System.String,System.Int32)')
  - [WaitForEmptyInput(timeout)](#M-gdio-unity_api-v2-CoApiClient-WaitForEmptyInput-System-Int32- 'gdio.unity_api.v2.CoApiClient.WaitForEmptyInput(System.Int32)')
  - [WaitForFixedUpdate()](#M-gdio-unity_api-v2-CoApiClient-WaitForFixedUpdate 'gdio.unity_api.v2.CoApiClient.WaitForFixedUpdate')
  - [WaitForObject(hierarchyPath,timeout)](#M-gdio-unity_api-v2-CoApiClient-WaitForObject-System-String,System-Int32- 'gdio.unity_api.v2.CoApiClient.WaitForObject(System.String,System.Int32)')
  - [WaitForObjectValue(hierarchyPath,fieldOrPropertyName,value,waitForObject,timeout,valueSerializer)](#M-gdio-unity_api-v2-CoApiClient-WaitForObjectValue-System-String,System-String,System-Object,System-Boolean,System-Int32,gdio-plugin-serializer-ICustomSerializer- 'gdio.unity_api.v2.CoApiClient.WaitForObjectValue(System.String,System.String,System.Object,System.Boolean,System.Int32,gdio.plugin.serializer.ICustomSerializer)')

<a name='T-gdio-unity_api-v2-ApiClient'></a>
## ApiClient `type`

##### Namespace

gdio.unity_api.v2

##### Summary

GameDriver.io Unity API Client class.

<a name='M-gdio-unity_api-v2-ApiClient-#ctor'></a>
### #ctor() `constructor`

##### Summary

GameDriver.io Unity API Client class constructor.

##### Parameters

This constructor has no parameters.

<a name='F-gdio-unity_api-v2-ApiClient-AUTOPLAY_DEFAULT_PORT'></a>
### AUTOPLAY_DEFAULT_PORT `constants`

##### Summary

The default AUTOPLAY port to use when searching for running games.  This port is configured in the Unity preferences.

<a name='F-gdio-unity_api-v2-ApiClient-AUTOPLAY_ENABLED'></a>
### AUTOPLAY_ENABLED `constants`

##### Summary

NOT IN USE.

<a name='F-gdio-unity_api-v2-ApiClient-AUTOPLAY_RECEIVE_PORT'></a>
### AUTOPLAY_RECEIVE_PORT `constants`

##### Summary

The port to listen for responses from the AutoPlay plugin running in Unity.  Due to loopback limitations, this port must be different than the [AUTOPLAY_DEFAULT_PORT](#F-gdio-unity_api-v2-ApiClient-AUTOPLAY_DEFAULT_PORT 'gdio.unity_api.v2.ApiClient.AUTOPLAY_DEFAULT_PORT')

<a name='F-gdio-unity_api-v2-ApiClient-THROW_EXCEPTIONS'></a>
### THROW_EXCEPTIONS `constants`

##### Summary

If TRUE, the API will throw exceptions instead of logging errors and where applicable returning false/NULL.  The default is FALSE.

<a name='M-gdio-unity_api-v2-ApiClient-AxisPress-System-String,System-Single,System-UInt64,System-Int32-'></a>
### AxisPress(axisId,value,numberOfFrames,timeout) `method`

##### Summary

Use this function to send arbitrary button states to the game. Defaults to LEFT ALT/CTRL/SHIFT/WINDOWS(COMMAND)

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| axisId | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | Axis input to press.  Name as defined in the Input Manager (Old) |
| value | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | Value of change on the axis (-1, +1) |
| numberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press and hold the axis for. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Press the down, left, up, then right keys in sequence
            api.AxisPress("Horizontal1", 100);
            api.Wait(300);
            api.AxisPress("Vertical1", 100);
            api.Wait(300);
            
```

<a name='M-gdio-unity_api-v2-ApiClient-ButtonPress-System-String,System-UInt64,System-Int32-'></a>
### ButtonPress(buttonId,numberOfFrames,timeout) `method`

##### Summary

Use this function to send arbitrary button states to the game. Defaults to LEFT ALT/CTRL/SHIFT/WINDOWS(COMMAND)

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | Button input to press.  Name as defined in the Input Manager (Old) |
| numberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press and hold the button for. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Press the down, left, up, then right keys in sequence
            api.ButtonPress("Fire1", 100);
            api.Wait(300);
            api.ButtonPress("Fire2", 100);
            api.Wait(300);
            
```

<a name='M-gdio-unity_api-v2-ApiClient-CallMethod-System-String,System-String,System-Object[],System-Int32-'></a>
### CallMethod(hierarchyPath,methodName,arguments,timeout) `method`

##### Summary

Use this function to execute a [Void](https://docs.microsoft.com/en-us/dotnet/api/System.Void 'System.Void') method on an object.

##### Returns

Returns a boolean based on the successful execution of the return type void, method.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the object that the script component is attached to. |
| methodName | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The name of the method to call. |
| arguments | [System.Object[]](https://docs.microsoft.com/en-us/dotnet/api/System.Object[] 'System.Object[]') | An array of objects to pass as arguments to the method. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the request was processed. |

##### Example

```
api.CallMethod("//*[@name='Canvas']/fn:component('CustomScript')",
                "CustomMethod", new string[] { "string:The Test was run on " + DateTime.Now.ToShortDateString() });
```

<a name='M-gdio-unity_api-v2-ApiClient-CallMethod<T>-System-String,System-String,System-Object[],System-Int32-'></a>
### CallMethod<T>(hierarchyPath,methodName,arguments,timeout) `method`

##### Summary

Use this function to execute a method on an object.

##### Returns

Returns a deserialized object of type T. If T and the type of the returned object don't match, an exception will be thrown.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the object that the script component is attached to. |
| methodName | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The name of the method to call. |
| arguments | [System.Object[]](https://docs.microsoft.com/en-us/dotnet/api/System.Object[] 'System.Object[]') | An array of objects to pass as arguments to the method. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the request was processed. |

##### Example

```
api.CallMethod&lt;int&gt;("//*[@name='Canvas']/fn:component('CustomScript')", "DoMath", new object[] { 1, 2 });
```

<a name='M-gdio-unity_api-v2-ApiClient-CaptureScreenshot-System-String,System-Boolean,System-Boolean,System-Int32-'></a>
### CaptureScreenshot(filename,storeInGameFolder,overwriteExisting,timeout) `method`

##### Summary

Use this function to capture a screenshot of the Game under test.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| filename | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The filename, and path, of the screen capture. |
| storeInGameFolder | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | If true, this won't transfer the screen capture back to the client and instead will save it on the device where the game is running. |
| overwriteExisting | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | If true, the operation will overwrite the file if it already exists. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the CaptureScreenshot request was processed. |

##### Example

```
api.CaptureScreenshot(@"c:\temp\screen1.png", false, true);
```

<a name='M-gdio-unity_api-v2-ApiClient-Click-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,System-Int32-'></a>
### Click(buttonId,position,clickFrameCount,timeout) `method`

##### Summary

Use this function to perform in-game mouse-clicks.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| position | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The [Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') position to perform the mouse click. |
| clickFrameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to click the specific position. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the Click request was processed.  Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

##### Example

```
api.Click(MouseButtons.LEFT, new Vector2 (0, 0), 30, 30); //Clicks the left mouse button at 0,0 for 30 frames
```

<a name='M-gdio-unity_api-v2-ApiClient-Click-gdio-common-objects-MouseButtons,System-Single,System-Single,System-UInt64,System-Int32-'></a>
### Click(buttonId,x,y,clickFrameCount,timeout) `method`

##### Summary

Use this function to perform in-game mouse-clicks.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| x | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The X coordinate of the game to click in Screen space. |
| y | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The Y coordinate of the game to click in Screen space. |
| clickFrameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to click the specific position. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the Click request was processed.  Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

##### Example

```
api.Click(MouseButtons.LEFT, 0, 0, 30, 30); //Clicks the left mouse button at 0,0 for 30 frames
```

<a name='M-gdio-unity_api-v2-ApiClient-ClickEx-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32-'></a>
### ClickEx(buttonId,position,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout) `method`

##### Summary

Use this function to perform in-game mouse-clicks combined with key press operations.  The total frame count of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| position | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The [Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') position to perform the mouse click. |
| clickFrameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to click the specific position. |
| keys | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') keys to press during the click operation. |
| keysNumberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press the keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| modifiers | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') modifier keys to press during the click operation. |
| modifiersNumberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press the modifier keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| delayAfterModifiersMsec | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | Total time in milliseconds to wait after pressing modifier keys, before clicking the object.  This is needed when a delay is required to register the modifier keys have been pressed in game.
If this delay is longer than that of the frame count for all of the key presses and click operations, the resulting behavior may not be what the user intends. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the ClickEx request was processed.  Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

##### Example

```
//Clicks the left mouse button at 0,0 for 30 frames while holding the left-shift key for 3 frames, and the C key for 5 frames.
            api.ClickEx(MouseButtons.LEFT, new Vector2(0, 0), 30, new KeyCode[] { KeyCode.C }, 5, new KeyCode[] { KeyCode.LeftShift }, 3, 500, 30);
            
```

<a name='M-gdio-unity_api-v2-ApiClient-ClickEx-gdio-common-objects-MouseButtons,System-Single,System-Single,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32-'></a>
### ClickEx(buttonId,x,y,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout) `method`

##### Summary

Use this function to perform in game mouse-clicks combined with key press operations.  The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| x | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The X coordinate of the game to click in Screen space. |
| y | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The Y coordinate of the game to click in Screen space. |
| clickFrameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to click the specific position. |
| keys | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') keys to press during the click operation. |
| keysNumberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press the keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| modifiers | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') modifier keys to press during the click operation. |
| modifiersNumberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press the modifier keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| delayAfterModifiersMsec | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | Total time in milliseconds to wait after pressing modifier keys, before clicking the object.  This is needed when a delay is required to register the modifier keys have been pressed in the game.
If this delay is longer than that of the frame count for all of the key presses and click operations, the resulting behavior may not be what the user intends. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the ClickEx request was processed.  Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

##### Example

```
//Clicks the left mouse button at 0,0 for 30 frames while holding the left-shift key for 3 frames, and the C key for 5 frames.
            api.ClickEx(MouseButtons.LEFT, 0, 0, 30,
                new KeyCode[] { KeyCode.C }, 5,
                new KeyCode[] { KeyCode.LeftShift }, 3,
                500, 30);
```

<a name='M-gdio-unity_api-v2-ApiClient-ClickObject-gdio-common-objects-MouseButtons,System-String,System-UInt64,System-Int32-'></a>
### ClickObject(buttonId,hierarchyPath,frameCount,timeout) `method`

##### Summary

Use this function to interact with an in-game object using mouse-clicks.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the GameObject to perform a click on. |
| frameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to click the specific object. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of frames to hold the keys down before clicking. Total press frame count is keyFrames + frames.  Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

##### Example

```
//Locates and clicks the first object with the name "Cube" for 30 frames using the left mouse button.
            api.ClickObject(MouseButtons.LEFT,
                "//*[@name='Cube']", 30, 30);
```

<a name='M-gdio-unity_api-v2-ApiClient-ClickObjectEx-gdio-common-objects-MouseButtons,System-String,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32-'></a>
### ClickObjectEx(buttonId,hierarchyPath,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout) `method`

##### Summary

Use this function to interact with an in-game object using mouse-clicks combined with key press operations.  The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the GameObject to perform a click on. |
| clickFrameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to click the specific object. |
| keys | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') keys to press during the click operation. |
| keysNumberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press the keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| modifiers | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') modifier keys to press during the click operation. |
| modifiersNumberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press the modifier keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| delayAfterModifiersMsec | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | Total time in milliseconds to wait after pressing modifier keys, before clicking the object.  This is needed when a delay is required to register the modifier keys have been pressed in the game.
If this delay is longer than that of the frame count for all of the key presses and click operations, the resulting behavior may not be what the user intends. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the ClickObjectEx request was processed.  Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

##### Example

```
//Locates and clicks the first object with the name "Cube" for 30 frames with the left mouse button while holding the left-shift key for 3 frames, and the left-CTRL key for 5 frames.
            api.ClickObjectEx(MouseButtons.LEFT,
                "//*[@name='Cube']", 30,
                new KeyCode[] { KeyCode.LeftControl }, 5,
                new KeyCode[] { KeyCode.LeftShift }, 3,
                500, 30);
```

<a name='M-gdio-unity_api-v2-ApiClient-Connect-System-String,System-Int32,System-Boolean,System-Int32,System-Boolean-'></a>
### Connect(hostname,port,autoplay,timeout,autoPortResolution) `method`

##### Summary

Use this function to connect to a Unity game with GameDriver Agent configured and active.  This function can connect to the Unity editor or a Standalone deployment of a game.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hostname | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The hostname of the machine running the game. |
| port | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The configured port that the GameDriver agent is configured to use. |
| autoplay | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | Autoplay allows you to automatically start a game in the Unity editor without manual intervention. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The amount of time in seconds to wait for connectivity to establish with the game. |
| autoPortResolution | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | Auto port resolution allows for the Unity editor or Standalone game to report what port it is using for the GameDriver agent. |

##### Example

```
//Connects to a local instance of the Unity editor with the default port of 19734 configured and starts Play mode automatically.
            api.Connect("localhost");
            
            //Connects to an instance of Unity running on the machine with IP address 10.0.0.2, port 19191, where the Unity editor is already in Play mode OR the standalone game is running.
            api.Connect("10.0.0.20", 19191, false, 60);
```

<a name='M-gdio-unity_api-v2-ApiClient-Connect-System-String,System-String,System-Int32,System-Boolean,System-Int32,System-Boolean-'></a>
### Connect(hostname,regex_MatchGamePath,port,autoplay,timeout,autoPortResolution) `method`

##### Summary

Use this function to connect to a Unity game with GameDriver Agent configured and active.  This function can connect to the Unity editor or a Standalone deployment of a game.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hostname | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The hostname of the machine running the game. |
| regex_MatchGamePath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | This parameter is a regular expression that will attempt to match a specfic game via its Application.DataPath if you have multiple games running. |
| port | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The configured port that the GameDriver agent is configured to use. |
| autoplay | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | Autoplay allows you to automatically start a game in the Unity editor without manual intervention. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The amount of time in seconds to wait for connectivity to establish with the game. |
| autoPortResolution | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | Auto port resolution allows for the Unity editor or Standalone game to report what port it is using for the GameDriver agent. |

##### Example

```
//Connects to any running instance of the Unity editor on the local network (broadcast) with the project name of "myunitygame".
             api.Connect("*", ".*?myunitygame.**");
            
             //Connects to any running instance of the Unity editor on the local machine with the project name of "myunitygame".
             api.Connect("localhost", ".*?myunitygame.*");
            
             //Connects to any running instance of the Unity editor on the local network.
             api.Connect("*");
```

<a name='M-gdio-unity_api-v2-ApiClient-DisableHooks-gdio-unity_api-v2-HookingObject,System-Int32-'></a>
### DisableHooks(hookObject,timeout) `method`

##### Summary

Disable input hooks in the game.

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hookObject | [gdio.unity_api.v2.HookingObject](#T-gdio-unity_api-v2-HookingObject 'gdio.unity_api.v2.HookingObject') | The type of input hook to disable. See [HookingObject](#T-gdio-unity_api-v2-HookingObject 'gdio.unity_api.v2.HookingObject') |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
api.DisableHooks(HookingObject.ALL);
```

<a name='M-gdio-unity_api-v2-ApiClient-DisbleObjectCaching-System-Int32-'></a>
### DisbleObjectCaching(timeout) `method`

##### Summary

Disable the use of object caching when doing HierarchyPath object resolution.

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
api.DisableObjectCaching();
```

<a name='M-gdio-unity_api-v2-ApiClient-Disconnect'></a>
### Disconnect() `method`

##### Summary

Use this function to disconnect the API client from the Game.

##### Parameters

This method has no parameters.

##### Example

```
api.Disconnect();
```

<a name='M-gdio-unity_api-v2-ApiClient-DoubleClick-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,System-Int32-'></a>
### DoubleClick(buttonId,position,clickFrameCount,timeout) `method`

##### Summary

Use this function to perform in-game mouse double-clicks.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the double click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| position | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The Vector2 location to double click in Screen space. |
| clickFrameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to double click the specific position. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the Click request was processed.  Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

##### Example

```
//Double-clicks the left mouse button at position 0, 0 on the screen over a duration of 30 frames.
            api.DoubleClick(MouseButtons.LEFT, new Vector2(0, 0), 30, 30);
```

<a name='M-gdio-unity_api-v2-ApiClient-DoubleClick-gdio-common-objects-MouseButtons,System-Single,System-Single,System-UInt64,System-Int32-'></a>
### DoubleClick(buttonId,x,y,clickFrameCount,timeout) `method`

##### Summary

Use this function to perform in-game mouse double-clicks.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the double click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| x | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The X coordinate of the game to double click in Screen space. |
| y | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The Y coordinate of the game to double click in Screen space. |
| clickFrameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to click the specific location. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the Click request was processed.  Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

##### Example

```
//Double-clicks the left mouse button at position 0, 0 on the screen over a duration of 30 frames.
            api.DoubleClick(MouseButtons.LEFT, 0, 0, 30, 30);
```

<a name='M-gdio-unity_api-v2-ApiClient-DoubleClickEx-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32-'></a>
### DoubleClickEx(buttonId,position,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout) `method`

##### Summary

Use this function to perform in game mouse double clicks combined with key press operations.  The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| position | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The Vector2 position of where to double click in Screen space. |
| clickFrameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to click the specific position. |
| keys | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') keys to press during the click operation. |
| keysNumberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press the keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| modifiers | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') modifier keys to press during the click operation. |
| modifiersNumberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press the modifier keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| delayAfterModifiersMsec | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | Total time in milliseconds to wait after pressing modifier keys, before clicking the object.  This is needed when a delay is required to register the modifier keys have been pressed in the game.
If this delay is longer than the frame count for all the key presses and click operation that the behavior of the result may not be what the user intends. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the ClickEx request was processed.  Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

##### Example

```
//Double-clicks the left mouse button at the position 0, 0 for 30 frames with the left mouse button while holding the left-shift key for 3 frames, and the left-CTRL key for 5 frames.
            api.DoubleClickEx(MouseButtons.LEFT, new Vector2 (0, 0), 30,
                new KeyCode[] { KeyCode.LeftControl }, 5,
                new KeyCode[] { KeyCode.LeftShift }, 3,
                500, 30);
```

<a name='M-gdio-unity_api-v2-ApiClient-DoubleClickEx-gdio-common-objects-MouseButtons,System-Single,System-Single,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32-'></a>
### DoubleClickEx(buttonId,x,y,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout) `method`

##### Summary

Use this function to perform in game mouse double clicks combined with key press operations.  The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| x | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The X coordinate of the game to double click in Screen space. |
| y | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The Y coordinate of the game to double click in Screen space. |
| clickFrameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to click the specific position. |
| keys | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') keys to press during the click operation. |
| keysNumberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press the keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| modifiers | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') modifier keys to press during the click operation. |
| modifiersNumberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press the modifier keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| delayAfterModifiersMsec | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | Total time in milliseconds to wait after pressing modifier keys, before clicking the object.  This is needed when a delay is required to register the modifier keys have been pressed in the game.
If this delay is longer than the frame count for all the key presses and click operation that the behavior of the result may not be what the user intends. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the ClickEx request was processed.  Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

##### Example

```
//Double-clicks the left mouse button at the position 0, 0 for 30 frames with the left mouse button while holding the left-shift key for 3 frames, and the left-CTRL key for 5 frames.
            api.DoubleClickEx(MouseButtons.LEFT, 0, 0, 30,
                new KeyCode[] { KeyCode.LeftControl }, 5,
                new KeyCode[] { KeyCode.LeftShift }, 3,
                500, 30);
```

<a name='M-gdio-unity_api-v2-ApiClient-DoubleClickObject-gdio-common-objects-MouseButtons,System-String,System-UInt64,System-Int32-'></a>
### DoubleClickObject(buttonId,hierarchyPath,frameCount,timeout) `method`

##### Summary

Use this function to interact with an object in game using a mouse double-click.

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the double click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the GameObject to perform a double click on. |
| frameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to double-click the specific object. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the DoubleClickObject request was processed.  Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

##### Example

```
//Locates and double-clicks the first object with the name "Cube" over a period of 30 frames using the left mouse button.
            api.DoubleClickObject(MouseButtons.LEFT,
                "//*[@name='Cube']", 30, 30);
```

<a name='M-gdio-unity_api-v2-ApiClient-DoubleClickObjectEx-gdio-common-objects-MouseButtons,System-String,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32-'></a>
### DoubleClickObjectEx(buttonId,hierarchyPath,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout) `method`

##### Summary

Use this function to interact with an object in game using a mouse double-click, combinated with key press operations.  The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the double click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the GameObject to perform a double-click on. |
| clickFrameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to double-click the specific object. |
| keys | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') keys to press during the click operation. |
| keysNumberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press the keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| modifiers | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') modifier keys to press during the click operation. |
| modifiersNumberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press the modifier keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| delayAfterModifiersMsec | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | Total time in milliseconds to wait after pressing modifier keys, before clicking the object.  This is needed when a delay is required to register the modifier keys have been pressed in the game.
If this delay is longer than the frame count for all the key presses and click operation that the behavior of the result may not be what the user intends. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the DoubleClickObjectEx request was processed.  Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

##### Example

```
//Locates and clicks the first object with the name "Cube" for 30 frames with the left mouse button while holding the left-shift key for 3 frames, and the left-CTRL key for 5 frames.
            api.DoubleClickObjectEx(MouseButtons.LEFT,
                "//*[@name='Cube']", 30,
                new KeyCode[] { KeyCode.LeftControl }, 5,
                new KeyCode[] { KeyCode.LeftShift }, 3,
                500, 30);
```

<a name='M-gdio-unity_api-v2-ApiClient-EnableHooks-gdio-unity_api-v2-HookingObject,System-Int32-'></a>
### EnableHooks(hookObject,timeout) `method`

##### Summary

Enable input hooks in the game, which is required to perform various input types during replay.

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hookObject | [gdio.unity_api.v2.HookingObject](#T-gdio-unity_api-v2-HookingObject 'gdio.unity_api.v2.HookingObject') | The type of input hook to enable. See [HookingObject](#T-gdio-unity_api-v2-HookingObject 'gdio.unity_api.v2.HookingObject') |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
api.EnableHooks(HookingObject.ALL);
```

<a name='M-gdio-unity_api-v2-ApiClient-EnableObjectCaching-System-Int32-'></a>
### EnableObjectCaching(timeout) `method`

##### Summary

Enable the use of object caching when performing HierarchyPath object resolution.  Object caching is per HierarchyPath stored in a [IDictionary](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.IDictionary 'System.Collections.IDictionary'). If a matching HierarchyPath is already in the dictionary, then the stored object is returned.
The only way to update a cached reference is for the reference to be garbage collected or flush the cache with [FlushObjectLookupCache](#M-gdio-unity_api-v2-ApiClient-FlushObjectLookupCache-System-Int32- 'gdio.unity_api.v2.ApiClient.FlushObjectLookupCache(System.Int32)').

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
api.EnableObjectCaching();
```

<a name='M-gdio-unity_api-v2-ApiClient-FlushObjectLookupCache-System-Int32-'></a>
### FlushObjectLookupCache(timeout) `method`

##### Summary

If object caching is enabled, this method will request that the agent flush the cache being held for all object lookups.

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
api.FlushObjectLookupCache();
```

<a name='M-gdio-unity_api-v2-ApiClient-GetConnectedGameDetails'></a>
### GetConnectedGameDetails() `method`

##### Summary

This method returns the details of the game that the API client is connected to.

##### Returns

[GameConnectionDetails](#T-gdio-unity_api-v2-GameConnectionDetails 'gdio.unity_api.v2.GameConnectionDetails')

##### Parameters

This method has no parameters.

<a name='M-gdio-unity_api-v2-ApiClient-GetLastFPS'></a>
### GetLastFPS() `method`

##### Summary

This method returns the last frames per second that the API client has recieved from the GameDriver agent.

##### Returns

The last published FPS as a double.

##### Parameters

This method has no parameters.

##### Example

```
//Can be used as input for time-sensitive functions such as input.
            //For example, this will press the Down key for roughly 1 second:
            api.KeyPress(new KeyCode[] { KeyCode.DownArrow }, (ulong)api.GetLastFPS());
            
```

<a name='M-gdio-unity_api-v2-ApiClient-GetNextCollisionEvent<T>-System-String-'></a>
### GetNextCollisionEvent<T>(eventId) `method`

##### Summary

Collision events are stored in a FIFO queue.  Calling this method returns the next collision event that was returned.

##### Returns



##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| eventId | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The eventId returned from [RegisterCollisionMonitor](#M-gdio-unity_api-v2-ApiClient-RegisterCollisionMonitor-System-String,System-Int32- 'gdio.unity_api.v2.ApiClient.RegisterCollisionMonitor(System.String,System.Int32)') |

##### Generic Types

| Name | Description |
| ---- | ----------- |
| T |  |

<a name='M-gdio-unity_api-v2-ApiClient-GetObjectDistance-System-String,System-String,System-Int32-'></a>
### GetObjectDistance(objectA_HierarchyPath,objectB_HierarchyPath,timeout) `method`

##### Summary

This method returns the distance of two objects using vector subtraction.

##### Returns

Returns the distance between the two objects as a float.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| objectA_HierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the first GameObject. |
| objectB_HierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchYpath for the second GameObject. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
// CubeA.Transform = Vector3(1, 2, 3)
            // CubeB.Transform = Vector3(6, 5, 4)
            d = api.GetObjectDistance("//*[@name = 'CubeA']", "//*[@name = 'CubeB']");
            Console.WriteLine(d.ToString()); // prints -5.0,-3.0,-1.0
```

<a name='M-gdio-unity_api-v2-ApiClient-GetObjectFieldValue<T>-System-String,System-Int32-'></a>
### GetObjectFieldValue<T>(hierarchyPath,timeout) `method`

##### Summary

This method returns the field or property value of an object.

##### Returns

Returns an object of type T for the value or throws an [Exception](https://docs.microsoft.com/en-us/dotnet/api/System.Exception 'System.Exception') on error.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath of the object and field/property to be inspected. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Generic Types

| Name | Description |
| ---- | ----------- |
| T | The [Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type') of the field or property to be inspected. |

##### Example

// Searches for an object named 'HiddenCube' which is invisible in the scene, and checks whether the "Active" checkbox is enabled.

```
bool invisCube = api.GetObjectFieldValue&lt;bool&gt;("//*[@name='HiddenCube']/fn:component('UnityEngine.Behaviour')/@isActiveAndEnabled");
Assert.IsTrue(invisCube == false, "The invisible cube isn't active"); //Passes if the object is Active in the scene
```

<a name='M-gdio-unity_api-v2-ApiClient-GetObjectFieldValue<T>-System-String,System-String,System-Int32-'></a>
### GetObjectFieldValue<T>(hierarchyPath,fieldOrPropertyName,timeout) `method`

##### Summary

This method returns the field or property value of an object.

##### Returns

Returns an object of type T for the value or throws an [Exception](https://docs.microsoft.com/en-us/dotnet/api/System.Exception 'System.Exception') on error.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath of the object and field/property to be inspected. |
| fieldOrPropertyName | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The field/property name to retreieve the value for/ |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Generic Types

| Name | Description |
| ---- | ----------- |
| T | The [Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type') of the field or property to be inspected. |

##### Example

// Searches for an object named 'HiddenCube' which is invisible in the scene, and checks whether the "Active" checkbox is enabled.

```
bool invisCube = api.GetObjectFieldValue&lt;bool&gt;("//*[@name='HiddenCube']/fn:component('UnityEngine.Behaviour')", "isActiveAndEnabled");
Assert.IsTrue(invisCube == false, "The invisible cube isn't active"); //Passes if the object is Active in the scene
```

<a name='M-gdio-unity_api-v2-ApiClient-GetObjectList-System-Int32-'></a>
### GetObjectList(timeout) `method`

##### Summary

This method returns of a list of all GameObjects as returned by [](#!-UnityEngine-GameObject-FindObjectsOfType-Type- 'UnityEngine.GameObject.FindObjectsOfType(Type)'), where Type is UnityEngine.GameObject./>

##### Returns

This method returns a [IList](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.IList 'System.Collections.IList') of [LiteGameObject](#T-gdio-common-objects-LiteGameObject 'gdio.common.objects.LiteGameObject').  LiteGameObject is a slimmer representation of UnityEngine.GameObject

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

//Print a list of the scene objects

```
 System.Collections.Generic.List&lt;LiteGameObject&gt; objects = api.GetObjectList();
 //Test whether the list is null
 Assert.IsNotNull(objects, "GetObjectList failed!");
 //Print a full object list
 foreach (var obj in objects)
 {
     Console.WriteLine("Object Name: " + obj.Name);
     Console.WriteLine("Object Tag: " + obj.Tag);
     Console.WriteLine("Object Position: " + obj.Position);
     Console.WriteLine($"Object Rotation (w): {obj.Rotation.w}, (x): {obj.Rotation.x}, (y): {obj.Rotation.x}, (z): {obj.Rotation.z}");
 }
 
```

<a name='M-gdio-unity_api-v2-ApiClient-GetObjectPosition-System-String,gdio-common-objects-CoordinateConversion,System-String,System-Int32-'></a>
### GetObjectPosition(objectHierarchyPath,cordSpace,cameraHierarchyPath,timeout) `method`

##### Summary

Return the position of a specific object.

##### Returns

The Vector3 position of the specific object.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| objectHierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath of the object to return the position of. |
| cordSpace | [gdio.common.objects.CoordinateConversion](#T-gdio-common-objects-CoordinateConversion 'gdio.common.objects.CoordinateConversion') | The coorindate space conversion to perform on the position before returning it. See [CoordinateConversion](#T-gdio-common-objects-CoordinateConversion 'gdio.common.objects.CoordinateConversion') for more information. |
| cameraHierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchPath to the Camera GameObject to use.  The default is string.Empty, which uses Camera.main/> |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
// spot is set to the Vector3 value of the object position on screen
           Vector3 spot = api.GetObjectPosition("//*[@name = 'Player prefab(Clone)']",
               CoordinateConversion.WorldToScreenPoint);
```

<a name='M-gdio-unity_api-v2-ApiClient-GetSceneName-System-Int32-'></a>
### GetSceneName(timeout) `method`

##### Summary

Return the name of the current active scene.

##### Returns

The name of the scene as a string.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
string activeScene = api.GetSceneName();
```

<a name='M-gdio-unity_api-v2-ApiClient-GetVersionsString'></a>
### GetVersionsString() `method`

##### Summary

Returns the GameDriver component versions in this build.

##### Parameters

This method has no parameters.

<a name='M-gdio-unity_api-v2-ApiClient-KeyPress-gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32-'></a>
### KeyPress(keys,numberOfFrames,modifiers,modifierNumberOfFrames,delayAfterModifiersMsec,timeout) `method`

##### Summary

Use this function to send arbitrary button states to the game. Defaults to LEFT ALT/CTRL/SHIFT/WINDOWS(COMMAND)

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| keys | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of keys([KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode')) to press. |
| numberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press and hold the keys for. |
| modifiers | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of modifiers()[KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') to press. |
| modifierNumberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to hold the modifiers down for, before pressing the keys. |
| delayAfterModifiersMsec | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The delay to wait between holding the modifies and pressing the keys. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
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

<a name='M-gdio-unity_api-v2-ApiClient-Launch-System-String,System-String-'></a>
### Launch(filename,arguments) `method`

##### Summary

Use this function to launch the Unity game build from an executable. In order to automate execution, games should be set to automatically start at the desired screen resolution and require no additional external dialogs to start. These can typically be set in Unity under Build Settings > Resolution, Other Settings, etc...

##### Returns

Returns true if the API successfully launches the game.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| filename | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The path to the executable. In Windows, this should follow the standard “C:\folder\subfolder\filename.exe” convention. |
| arguments | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | Command line arguments to pass to the executable. |

<a name='M-gdio-unity_api-v2-ApiClient-LoadScene-System-String,System-Int32-'></a>
### LoadScene(sceneName,timeout) `method`

##### Summary

This method loads the scene, defined by the scene name passed as an argument.

##### Returns

TRUE if the request was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| sceneName | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The name of the scene to load |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Loads the FinalBoss scene
            api.LoadScene("FinalBoss");
```

<a name='M-gdio-unity_api-v2-ApiClient-MouseDrag-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,gdio-common-objects-Vector2,System-Boolean,System-Int32-'></a>
### MouseDrag(button,destination,frameCount,origin,waitForEmptyInput,timeout) `method`

##### Summary

Perform a mouse drag operation.

##### Returns

TRUE if the requests was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| button | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button, [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'), to perform the drag operation with. |
| destination | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The destination vector to drag the mouse to. |
| frameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames taken to complete the drag operation. |
| origin | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The origin to start the drag operation.  If null, the mouse drag operation will begin at the current position of Input.mousePosition. |
| waitForEmptyInput | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | Wait for the empty input event to be returned from the agent before returning from the method call. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. If waitForEmptyInput is set to TRUE, then the method call will wait the timeout allotment to recieve the event. |

##### Example

```
//Drags the left mouse button to the position 180, 0 on the screen over 30 frames
            api.MouseDrag(MouseButtons.LEFT, new Vector2(180, 0), 30, start, true);
```

<a name='M-gdio-unity_api-v2-ApiClient-MouseMoveToObject-System-String,System-UInt64,System-Boolean,System-Boolean,System-Int32-'></a>
### MouseMoveToObject(objectHierarchyPath,frameCount,waitForObject,waitForEmptyInput,timeout) `method`

##### Summary

Move the mouse to the center of a specific object, identified by the HierarchyPath.

##### Returns

TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| objectHierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath to move the mouse pointer to. |
| frameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to compelte the mouse move over. |
| waitForObject | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | If TRUE, wait for the object to exist so that mouse move can complete successfully. |
| waitForEmptyInput | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | Wait for the empty input event to be returned from the GameDriver agent, before returning from the method. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent.  If waitForEmptyInput is TRUE, then the method call will wait the timeout alotment to recieve the event. |

##### Example

```
//Moves the mouse to the center of the object named "Cylinder" over 300 frames
            api.MouseMoveToObject("//*[@name='Cylinder']", 300, true, true);
```

<a name='M-gdio-unity_api-v2-ApiClient-MoveMouseToPoint-gdio-common-objects-Vector2,System-UInt64,gdio-common-objects-Vector2,System-Boolean,System-Int32-'></a>
### MoveMouseToPoint(destination,frameCount,origin,waitForEmptyInput,timeout) `method`

##### Summary

Move the mouse to the destination vector.

##### Returns

TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| destination | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | Destination vector to move the mouse to. |
| frameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to complete the operaiton over. |
| origin | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The origin to start the mouse move operation.  If null, the mouse move operation will begin at the current position of Input.mousePosition. |
| waitForEmptyInput | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | Wait for the empty input event to be returned from the GameDriver agent, before returning from the method. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent.  If waitForEmptyInput is TRUE, then the method call will wait the timeout alotment to recieve the event. |

##### Example

```
//First get the position of an object named "Cube" on screen
             Vector3 cubePos = api.GetObjectPosition("//*[@name='Cube']", CoordinateConversion.WorldToScreenPoint);
            
             //Take the x,y values of the on-screen object
             Vector2 cubePos2 = new Vector2(cubePos.x, cubePos.y);
             
             //Move the mouse to the cube on-screen position over 30 frames
             api.MoveMouseToPoint(cubePos2, (ulong) api.GetLastFPS());
```

<a name='M-gdio-unity_api-v2-ApiClient-NavAgentMoveToPoint-System-String,gdio-common-objects-Vector3,System-Boolean,System-Int32-'></a>
### NavAgentMoveToPoint(navAgentHierarchyPath,destination,waitForMoveToComplete,timeout) `method`

##### Summary

Move a NavAgent to a destination point.

##### Returns

TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| navAgentHierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath to the NavAgent. |
| destination | [gdio.common.objects.Vector3](#T-gdio-common-objects-Vector3 'gdio.common.objects.Vector3') | The destination vector to move to. |
| waitForMoveToComplete | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | Wait for the NavAgent move-to operation to complete before the method returns. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Moves the 1st object named "Ellen" to position 20, 0, 20 on the NavMesh
            api.NavAgentMoveToPoint("//*[@name='Ellen']", new Vector3(20, 0, 20));
```

<a name='M-gdio-unity_api-v2-ApiClient-Raycast-gdio-common-objects-Vector3,System-String,System-Int32-'></a>
### Raycast(raycastPoint,cameraHierarchyPath,timeout) `method`

##### Summary

Perform a Raycast to a point to find out what is in that position.

##### Returns

Returns an array of [RaycastResult](#T-gdio-common-objects-RaycastResult 'gdio.common.objects.RaycastResult').

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| raycastPoint | [gdio.common.objects.Vector3](#T-gdio-common-objects-Vector3 'gdio.common.objects.Vector3') | The vector to perform a raycast to. |
| cameraHierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the  UnityEngine.Camera to use as a Raycast reference.  If the Camera is string.Empty, the Camera.main is used |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
// Racast to an object named "Ellen"
             RaycastResult[] rr = api.Raycast(api.GetObjectPosition("//*[@name='Ellen']"));
             
             foreach (var res in rr)
             {
                 Console.WriteLine(res);
             }
            
             // Output
             // [RaycastResult]
             // Type: Physics
             // Tag: Untagged
             // Name: Plane
             // HasButton: False
             // Point: (-5.217863, 0, -0.5770187)
             // Type Name: UnityEngine.GameObject
             
             
```

<a name='M-gdio-unity_api-v2-ApiClient-RegisterCollisionMonitor-System-String,System-Int32-'></a>
### RegisterCollisionMonitor(hierarchyPath,timeout) `method`

##### Summary

Register a collision monitor to recieve collision events on an object.

##### Returns

String returned is the event identifier

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the object to rotate. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
api.RegisterCollisionMonitor("//*[@name='Cylinder']");
```

<a name='M-gdio-unity_api-v2-ApiClient-RotateObject-System-String,gdio-common-objects-Quaternion,System-Boolean,System-Int32-'></a>
### RotateObject(hierarchyPath,quaternion,waitForObject,timeout) `method`

##### Summary

Rotate an object defined by the HierarchyPath and rotated by a Quaternion. for more information.

##### Returns

TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the object to rotate. |
| quaternion | [gdio.common.objects.Quaternion](#T-gdio-common-objects-Quaternion 'gdio.common.objects.Quaternion') | The quaternion value to manipulate the object. |
| waitForObject | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | Wait for the object to exist if it doesn't. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
api.RotateObject("//*[@name='Cylinder']", new Quaternion(0, 0, 2, 2), true);
```

<a name='M-gdio-unity_api-v2-ApiClient-RotateObject-System-String,gdio-common-objects-Vector3,gdio-common-objects-Space,System-Boolean,System-Int32-'></a>
### RotateObject(hierarchyPath,eulers,relativeTo,waitForObject,timeout) `method`

##### Summary

Rotate an object defined by the HierarchyPath and rotated by Eulers. for more information.

##### Returns

TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the object to rotate. |
| eulers | [gdio.common.objects.Vector3](#T-gdio-common-objects-Vector3 'gdio.common.objects.Vector3') | The Eulers vector to manipulate the object. |
| relativeTo | [gdio.common.objects.Space](#T-gdio-common-objects-Space 'gdio.common.objects.Space') | The [Space](#T-gdio-common-objects-Space 'gdio.common.objects.Space') to perform the rotation relative to. |
| waitForObject | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | Wait for the object to exist if it doesn't. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Rotates an object with the name "Cylinder" by 30 degrees on the y axis.
            api.RotateObject("//*[@name='Cylinder']", new Vector3(0, 30, 0), Space.Self, true);
```

<a name='M-gdio-unity_api-v2-ApiClient-RotateObject-System-String,System-Single,System-Single,System-Single,gdio-common-objects-Space,System-Boolean,System-Int32-'></a>
### RotateObject(hierarchyPath,xAngle,yAngle,zAngle,relativeTo,waitForObject,timeout) `method`

##### Summary

Rotate an object defined by the HierarchyPath and rotated by the x, y, and z angles relative to the Space

##### Returns

TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the object to rotate. |
| xAngle | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The X angle value to rotate. |
| yAngle | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The Y angle value to rotate. |
| zAngle | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The Z angle value to rotate. |
| relativeTo | [gdio.common.objects.Space](#T-gdio-common-objects-Space 'gdio.common.objects.Space') | The [Space](#T-gdio-common-objects-Space 'gdio.common.objects.Space') to perform the rotation relative to. |
| waitForObject | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | Wait for the object to exist if it doesn't. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Rotates an object with the name "Cylinder" by 20 degrees on the z axis
            api.RotateObject("//*[@name='Cylinder']", 0, 0, 20);
```

<a name='M-gdio-unity_api-v2-ApiClient-RotateObject-System-String,gdio-common-objects-Vector3,System-Single,gdio-common-objects-Space,System-Boolean,System-Int32-'></a>
### RotateObject(hierarchyPath,axis,angle,relativeTo,waitForObject,timeout) `method`

##### Summary

Rotate an object defined by the HierarchyPath and rotated by the axis and angle, relative to the Space

##### Returns

TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the object to rotate. |
| axis | [gdio.common.objects.Vector3](#T-gdio-common-objects-Vector3 'gdio.common.objects.Vector3') |  |
| angle | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') |  |
| relativeTo | [gdio.common.objects.Space](#T-gdio-common-objects-Space 'gdio.common.objects.Space') | The [Space](#T-gdio-common-objects-Space 'gdio.common.objects.Space') to perform the rotation relative to. |
| waitForObject | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | Wait for the object to exist if it doesn't. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Will rotate an object named "Cylinder" on all 3 axis by 45-degrees
            api.RotateObject("//*[@name='Cylinder']", new Vector3(0, 0, 0), 45);
```

<a name='M-gdio-unity_api-v2-ApiClient-SetInputFieldText-System-String,System-String,System-Boolean,System-Int32-'></a>
### SetInputFieldText(hierarchyPath,value,waitForObject,timeout) `method`

##### Summary

Set the text of an InputField or TMP_InputField

##### Returns

TRUE if the GameDriver agent was able to successfully set the InputField text.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath to the InputField or TMP_InputField. |
| value | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The text value to set in the field. |
| waitForObject | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | If TRUE, wait for the object to exist if it doesn't. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The time to wait for the object to exist. |

##### Example

```
//Sets the text field component attached to the "TextMeshPro InputField" object with the tag "FilterInputTxt" to the value of "America"
            api.SetInputFieldText("//FilterInputTxt[@name='TextMeshPro InputField']", "America");
```

<a name='M-gdio-unity_api-v2-ApiClient-SetObjectFieldValue-System-String,System-String,System-Object,System-Boolean,System-Int32-'></a>
### SetObjectFieldValue(hierarchyPath,fieldOrPropertyName,value,waitForObject,timeout,valueSerializer) `method`

##### Summary

Set the field or property of an object.

##### Returns

TRUE if the field/property was successfully set to the value.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath to the object to set the field/property value. |
| fieldOrPropertyName | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The field or property name to set the value of. |
| value | [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') | The value to set for the field/property. |
| waitForObject | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | If TRUE, wait for the object to exist if it doesn't. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The time to wait for the object to exist. |

##### Example

```
//Sets the text field component attached to the "TextMeshPro InputField" object with the tag "FilterInputTxt" to the value of "Asia"
            api.SetObjectFieldValue("/Untagged[@name='Canvas']/FilterInputTxt[@name='TextMeshPro InputField']/fn:component('TMPro.TMP_InputField')", "text", "string:Asia");
```

<a name='M-gdio-unity_api-v2-ApiClient-Tap-gdio-common-objects-Vector2,System-Int32,System-UInt64,System-Int32-'></a>
### Tap(position,tapCount,frameCount,timeout) `method`

##### Summary

Tap the handheld device at the defined position.

##### Returns

TRUE if the GameDriver agent was able to process the request successfully.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| position | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The vector position to tap the device screen. |
| tapCount | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of taps that should be registered. |
| frameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to complete the tap input over. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Performs a single tap at position 0, 0 for 10 frames
            api.Tap(new Vector2(0, 0), 1, 10); 
```

<a name='M-gdio-unity_api-v2-ApiClient-Tap-System-Single,System-Single,System-Int32,System-UInt64,System-Int32-'></a>
### Tap(x,y,tapCount,frameCount,timeout) `method`

##### Summary

Tap the handheld device at the defined position.

##### Returns

TRUE if the GameDriver agent was able to process the request successfully.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| x | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The X coordinate of the position to tap the device screen. |
| y | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The Y coordinate position to tap the device screen. |
| tapCount | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of taps that should be registered. |
| frameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to complete the tap input over. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Performs a single tap at position 0, 0 for 10 frames
            api.Tap(0, 0, 1, 10);
```

<a name='M-gdio-unity_api-v2-ApiClient-TapObject-System-String,System-Int32,System-UInt64,System-Int32-'></a>
### TapObject(hierarchyPath,tapCount,frameCount,timeout) `method`

##### Summary

Tap an object.

##### Returns

TRUE if the GameDriver agent was able to process the request successfully.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath of the object to tap. |
| tapCount | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of taps that should be registered. |
| frameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to complete the tap input over. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Performs a single tap on an object with the name "Cube"
            api.TapObject("//*[@name='Cube']", 1, 10);
```

<a name='M-gdio-unity_api-v2-ApiClient-TouchInput-gdio-common-objects-Vector2,gdio-common-objects-Vector2,System-Int32,System-Int32,System-UInt64,System-Boolean,System-Single,System-Single,System-Single,System-Single,System-Single,System-Int32-'></a>
### TouchInput(startPosition,destinationPosition,fingerId,tapCount,frameCount,waitForEmptyInput,radius,pressure,altitudeAngle,azmulthAngle,maximumPossiblePressure,timeout) `method`

##### Summary

Send a raw TouchInput event to the game.

##### Returns

TRUE if the GameDriver agent was able to process the request successfully.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| startPosition | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | Vector position of the start of the touch input. |
| destinationPosition | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | Vector destination position of where the touch input ends. |
| fingerId | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The finder id of the touch input. |
| tapCount | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of taps that should be registered. |
| frameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to complete the tap input over. |
| waitForEmptyInput | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | If TRUE, wait for the Empty Input event to be broadcast before returning from the method. |
| radius | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The radius of the touch input. |
| pressure | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The pressure of the touch input. |
| altitudeAngle | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The altitude angle of the touch input. |
| azmulthAngle | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The azmulth ange of the touch input. |
| maximumPossiblePressure | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The maximum possible pressure for the touch input. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Performs a single touch input from 0,0 to 100, 100 with a single "finger" over a duration of 50 frames
            api.TouchInput(new Vector2(0, 0), new Vector2(100, 100), 0, 1, 50);
```

<a name='M-gdio-unity_api-v2-ApiClient-TouchInput-System-Single,System-Single,System-Single,System-Single,System-Int32,System-Int32,System-UInt64,System-Boolean,System-Single,System-Single,System-Single,System-Single,System-Single,System-Int32-'></a>
### TouchInput(x1,y1,x2,y2,fingerId,tapCount,frameCount,waitForEmptyInput,radius,pressure,altitudeAngle,azmulthAngle,maximumPossiblePressure,timeout) `method`

##### Summary

Send a raw TouchInput event to the game.

##### Returns

TRUE if the GameDriver agent was able to process the request successfully.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| x1 | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The X coordinate of the start position. |
| y1 | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The Y coordinate of the start position. |
| x2 | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The X coordinate of the end position. |
| y2 | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The Y coordinate of the end position. |
| fingerId | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The finder id of the touch input. |
| tapCount | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of taps that should be registered. |
| frameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to complete the tap input over. |
| waitForEmptyInput | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | If TRUE, wait for the Empty Input event to be broadcast before returning from the method. |
| radius | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The radius of the touch input. |
| pressure | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The pressure of the touch input. |
| altitudeAngle | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The altitude angle of the touch input. |
| azmulthAngle | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The azmulth ange of the touch input. |
| maximumPossiblePressure | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The maximum possible pressure for the touch input. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Performs a single touch input from 0,0 to 100, 100 with a single "finger" over a duration of 50 frames
            api.TouchInput(0, 0, 100, 100, 0, 1, 50);
```

<a name='M-gdio-unity_api-v2-ApiClient-UnregisterCollisionMonitor-System-String,System-Int32-'></a>
### UnregisterCollisionMonitor(hierarchyPath,timeout) `method`

##### Summary

Unregister the monitoring of collision events on a GameObject that has been previously registered for monitoring.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') |  |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') |  |

<a name='M-gdio-unity_api-v2-ApiClient-Wait-System-Int32-'></a>
### Wait(milliSeconds) `method`

##### Summary

Client side Wait or Pause.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| milliSeconds | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of milliseconds to wait. |

##### Example

```
api.Wait(3000); //Waits 3 seconds before continuing
```

<a name='M-gdio-unity_api-v2-ApiClient-WaitForCollisionEvent-System-String,System-Int32-'></a>
### WaitForCollisionEvent(eventId,timeout) `method`

##### Summary

Wait for a collision event to fire on an element that is being monitored for collisions.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| eventId | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The eventId received from the [RegisterCollisionMonitor](#M-gdio-unity_api-v2-ApiClient-RegisterCollisionMonitor-System-String,System-Int32- 'gdio.unity_api.v2.ApiClient.RegisterCollisionMonitor(System.String,System.Int32)') call. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a collision event to be fired. |

##### Example

```
api.WaitForCollisionEvent(eventId);
```

<a name='M-gdio-unity_api-v2-ApiClient-WaitForCollisionEvent<T>-System-String,System-Int32-'></a>
### WaitForCollisionEvent<T>(eventId,timeout) `method`

##### Summary

Wait for a collision event to fire on an element that is being monitored for collisions. If the method has been called before, there is the potential that another event was recieved before waiting on the event again.  
Check with [GetNextCollisionEvent<T>](#M-gdio-unity_api-v2-ApiClient-GetNextCollisionEvent<T>-System-String- 'gdio.unity_api.v2.ApiClient.GetNextCollisionEvent<T>(System.String)') to see if it returns null to see if an event was missed.

##### Returns

The collision messages. TODO: Return a translated collisionInfo object

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| eventId | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The eventId received from the [RegisterCollisionMonitor](#M-gdio-unity_api-v2-ApiClient-RegisterCollisionMonitor-System-String,System-Int32- 'gdio.unity_api.v2.ApiClient.RegisterCollisionMonitor(System.String,System.Int32)') call. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a collision event to be fired. |

##### Example

```
api.WaitForCollisionEvent{object}(eventId);
```

<a name='M-gdio-unity_api-v2-ApiClient-WaitForEmptyInput-System-Int32-'></a>
### WaitForEmptyInput(timeout) `method`

##### Summary

Wait for an Empty Input event to be received.

##### Returns



##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The time to wait for the event. |

<a name='M-gdio-unity_api-v2-ApiClient-WaitForObject-System-String,System-Int32-'></a>
### WaitForObject(hierarchyPath,timeout) `method`

##### Summary

Wait for an object to exist.

##### Returns

TRUE if the object exists within the alloted timeout.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath of the object. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The amount of time to wait for the object to exist. |

##### Example

```
api.WaitForObject("//*[@name='Cube']"); //Waits for an object named "Cube" to exist
```

<a name='M-gdio-unity_api-v2-ApiClient-WaitForObjectValue-System-String,System-String,System-Object,System-Boolean,System-Int32-'></a>
### WaitForObjectValue(hierarchyPath,fieldOrPropertyName,value,waitForObject,timeout,valueSerializer) `method`

##### Summary

Wait for an object to exist and have a specific value for a specified field/property.

##### Returns

TRUE if the object exists with the specified value in the alloted timeout.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath to the object. |
| fieldOrPropertyName | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The field/property name for inspection. |
| value | [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') | The value to wait for. |
| waitForObject | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | If TRUE, wait for the object to exist if it doesn't. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The amount of time to wait for the object to exist with the specified value. |

##### Example

```
//Waits for the value of the TextMeshProUGUI input field with the name "Text" to be "America"
            api.WaitForObjectValue("//*[@name='Text']/fn:component('TMPro.TextMeshProUGUI')", "text", "America");
```

<a name='T-gdio-unity_api-v2-CoApiClient'></a>
## CoApiClient `type`

##### Namespace

gdio.unity_api.v2

<a name='M-gdio-unity_api-v2-CoApiClient-CallMethod<T>-System-String,System-String,System-Object[],System-Int32-'></a>
### CallMethod<T>(hierarchyPath,methodName,arguments,timeout) `method`

##### Summary

Use this function to execute a method on an object.

##### Returns

Returns a deserialized object of type T. If T and the type of the returned object don't match, an exception will be thrown.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the object that the script component is attached to. |
| methodName | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The name of the method to call. |
| arguments | [System.Object[]](https://docs.microsoft.com/en-us/dotnet/api/System.Object[] 'System.Object[]') | An array of objects to pass as arguments to the method. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the request was processed. |

##### Example

```
api.CallMethod&lt;int&gt;("//*[@name='Canvas']/fn:component('CustomScript')", "DoMath", new object[] { 1, 2 });
```

<a name='M-gdio-unity_api-v2-CoApiClient-CaptureScreenshot-System-String,System-Boolean,System-Boolean,System-Int32-'></a>
### CaptureScreenshot(filename,storeInGameFolder,overwriteExisting,timeout) `method`

##### Summary

Use this function to capture a screenshot of the Game under test.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| filename | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The filename, and path, of the screen capture. |
| storeInGameFolder | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | If true, this won't transfer the screen capture back to the client and instead will save it on the device where the game is running. |
| overwriteExisting | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | If true, the operation will overwrite the file if it already exists. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the CaptureScreenshot request was processed. |

##### Example

```
api.CaptureScreenshot(@"c:\temp\screen1.png", false, true);
```

<a name='M-gdio-unity_api-v2-CoApiClient-Click-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,System-Int32-'></a>
### Click(buttonId,position,clickFrameCount,timeout) `method`

##### Summary

Use this function to perform in-game mouse-clicks.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| position | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The [Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') position to perform the mouse click. |
| clickFrameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to click the specific position. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the Click request was processed.  Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

##### Example

```
api.Click(MouseButtons.LEFT, new Vector2 (0, 0), 30, 30); //Clicks the left mouse button at 0,0 for 30 frames
```

<a name='M-gdio-unity_api-v2-CoApiClient-Click-gdio-common-objects-MouseButtons,System-Single,System-Single,System-UInt64,System-Int32-'></a>
### Click(buttonId,x,y,clickFrameCount,timeout) `method`

##### Summary

Use this function to perform in-game mouse-clicks.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| x | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The X coordinate of the game to click in Screen space. |
| y | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The Y coordinate of the game to click in Screen space. |
| clickFrameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to click the specific position. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the Click request was processed.  Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

##### Example

```
api.Click(MouseButtons.LEFT, 0, 0, 30, 30); //Clicks the left mouse button at 0,0 for 30 frames
```

<a name='M-gdio-unity_api-v2-CoApiClient-ClickEx-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32-'></a>
### ClickEx(buttonId,position,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout) `method`

##### Summary

Use this function to perform in-game mouse-clicks combined with key press operations.  The total frame count of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| position | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The [Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') position to perform the mouse click. |
| clickFrameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to click the specific position. |
| keys | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') keys to press during the click operation. |
| keysNumberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press the keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| modifiers | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') modifier keys to press during the click operation. |
| modifiersNumberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press the modifier keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| delayAfterModifiersMsec | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | Total time in milliseconds to wait after pressing modifier keys, before clicking the object.  This is needed when a delay is required to register the modifier keys have been pressed in game.
If this delay is longer than that of the frame count for all of the key presses and click operations, the resulting behavior may not be what the user intends. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the ClickEx request was processed.  Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

##### Example

```
//Clicks the left mouse button at 0,0 for 30 frames while holding the left-shift key for 3 frames, and the C key for 5 frames.
            api.ClickEx(MouseButtons.LEFT, new Vector2(0, 0), 30, new KeyCode[] { KeyCode.C }, 5, new KeyCode[] { KeyCode.LeftShift }, 3, 500, 30);
            
```

<a name='M-gdio-unity_api-v2-CoApiClient-ClickEx-gdio-common-objects-MouseButtons,System-Single,System-Single,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32-'></a>
### ClickEx(buttonId,x,y,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout) `method`

##### Summary

Use this function to perform in game mouse-clicks combined with key press operations.  The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| x | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The X coordinate of the game to click in Screen space. |
| y | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The Y coordinate of the game to click in Screen space. |
| clickFrameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to click the specific position. |
| keys | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') keys to press during the click operation. |
| keysNumberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press the keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| modifiers | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') modifier keys to press during the click operation. |
| modifiersNumberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press the modifier keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| delayAfterModifiersMsec | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | Total time in milliseconds to wait after pressing modifier keys, before clicking the object.  This is needed when a delay is required to register the modifier keys have been pressed in the game.
If this delay is longer than that of the frame count for all of the key presses and click operations, the resulting behavior may not be what the user intends. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the ClickEx request was processed.  Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

##### Example

```
//Clicks the left mouse button at 0,0 for 30 frames while holding the left-shift key for 3 frames, and the C key for 5 frames.
            api.ClickEx(MouseButtons.LEFT, 0, 0, 30,
                new KeyCode[] { KeyCode.C }, 5,
                new KeyCode[] { KeyCode.LeftShift }, 3,
                500, 30);
```

<a name='M-gdio-unity_api-v2-CoApiClient-ClickObject-gdio-common-objects-MouseButtons,System-String,System-UInt64,System-Int32-'></a>
### ClickObject(buttonId,hierarchyPath,frameCount,timeout) `method`

##### Summary

Use this function to interact with an in-game object using mouse-clicks.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the GameObject to perform a click on. |
| frameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to click the specific object. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of frames to hold the keys down before clicking. Total press frame count is keyFrames + frames.  Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

##### Example

```
//Locates and clicks the first object with the name "Cube" for 30 frames using the left mouse button.
            api.ClickObject(MouseButtons.LEFT,
                "//*[@name='Cube']", 30, 30);
```

<a name='M-gdio-unity_api-v2-CoApiClient-ClickObjectEx-gdio-common-objects-MouseButtons,System-String,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32-'></a>
### ClickObjectEx(buttonId,hierarchyPath,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout) `method`

##### Summary

Use this function to interact with an in-game object using mouse-clicks combined with key press operations.  The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the GameObject to perform a click on. |
| clickFrameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to click the specific object. |
| keys | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') keys to press during the click operation. |
| keysNumberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press the keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| modifiers | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') modifier keys to press during the click operation. |
| modifiersNumberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press the modifier keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| delayAfterModifiersMsec | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | Total time in milliseconds to wait after pressing modifier keys, before clicking the object.  This is needed when a delay is required to register the modifier keys have been pressed in the game.
If this delay is longer than that of the frame count for all of the key presses and click operations, the resulting behavior may not be what the user intends. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a response that the ClickObjectEx request was processed.  Input requests process asynchronously, so a response does NOT imply the input operation has completed. |

##### Example

```
//Locates and clicks the first object with the name "Cube" for 30 frames with the left mouse button while holding the left-shift key for 3 frames, and the left-CTRL key for 5 frames.
            api.ClickObjectEx(MouseButtons.LEFT,
                "//*[@name='Cube']", 30,
                new KeyCode[] { KeyCode.LeftControl }, 5,
                new KeyCode[] { KeyCode.LeftShift }, 3,
                500, 30);
```

<a name='M-gdio-unity_api-v2-CoApiClient-Connect-System-String,System-Int32,System-Int32-'></a>
### Connect(hostname,port,timeout) `method`

##### Summary

Use this function to connect to a Unity game with GameDriver Agent configured and active.  This function can connect to the UnityEditor or a Standalone deployment of a game.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hostname | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The hostname of the machine running the game. |
| port | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The configured port that the GameDriver agent is configured to use. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The amount of time in seconds to wait for connectivity to establish with the game. |

<a name='M-gdio-unity_api-v2-CoApiClient-DisableHooks-gdio-unity_api-v2-HookingObject,System-Int32-'></a>
### DisableHooks(hookObject,timeout) `method`

##### Summary

Disable input hooks in the game.

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hookObject | [gdio.unity_api.v2.HookingObject](#T-gdio-unity_api-v2-HookingObject 'gdio.unity_api.v2.HookingObject') | The type of input hook to disable. See [HookingObject](#T-gdio-unity_api-v2-HookingObject 'gdio.unity_api.v2.HookingObject') |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
api.DisableHooks(HookingObject.ALL);
```

<a name='M-gdio-unity_api-v2-CoApiClient-EnableHooks-gdio-unity_api-v2-HookingObject,System-Int32-'></a>
### EnableHooks(hookObject,timeout) `method`

##### Summary

Enable input hooks in the game, which is required to perform various input types during replay.

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hookObject | [gdio.unity_api.v2.HookingObject](#T-gdio-unity_api-v2-HookingObject 'gdio.unity_api.v2.HookingObject') | The type of input hook to enable. See [HookingObject](#T-gdio-unity_api-v2-HookingObject 'gdio.unity_api.v2.HookingObject') |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
api.EnableHooks(HookingObject.ALL);
```

<a name='M-gdio-unity_api-v2-CoApiClient-EnableObjectCaching-System-Int32-'></a>
### EnableObjectCaching(timeout) `method`

##### Summary

Enable the use of object caching when performing HierarchyPath object resolution.  Object caching is per HierarchyPath stored in a [IDictionary](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.IDictionary 'System.Collections.IDictionary'). If a matching HierarchyPath is already in the dictionary, then the stored object is returned.
The only way to update a cached reference is for the reference to be garbage collected or flush the cache with [FlushObjectLookupCache](#M-gdio-unity_api-v2-ApiClient-FlushObjectLookupCache-System-Int32- 'gdio.unity_api.v2.ApiClient.FlushObjectLookupCache(System.Int32)').

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
api.EnableObjectCaching();
```

<a name='M-gdio-unity_api-v2-CoApiClient-FlushObjectLookupCache-System-Int32-'></a>
### FlushObjectLookupCache(timeout) `method`

##### Summary

If object caching is enabled, this method will request that the agent flush the cache being held for all object lookups.

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
api.FlushObjectLookupCache();
```

<a name='M-gdio-unity_api-v2-CoApiClient-GetLastFPS'></a>
### GetLastFPS() `method`

##### Summary

This method returns the last frames per second that the API client has recieved from the GameDriver agent.

##### Returns

The last published FPS as a double.

##### Parameters

This method has no parameters.

##### Example

```
//Can be used as input for time-sensitive functions such as input.
            //For example, this will press the Down key for roughly 1 second:
            api.KeyPress(new KeyCode[] { KeyCode.DownArrow }, (ulong)api.GetLastFPS());
            
```

<a name='M-gdio-unity_api-v2-CoApiClient-GetNextCollisionEvent<T>-System-String-'></a>
### GetNextCollisionEvent<T>(eventId) `method`

##### Summary

Collision events are stored in a FIFO queue.  Calling this method returns the next collision event that was returned.

##### Returns



##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| eventId | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The eventId returned from [RegisterCollisionMonitor](#M-gdio-unity_api-v2-CoApiClient-RegisterCollisionMonitor-System-String,System-Int32- 'gdio.unity_api.v2.CoApiClient.RegisterCollisionMonitor(System.String,System.Int32)') |

##### Generic Types

| Name | Description |
| ---- | ----------- |
| T |  |

<a name='M-gdio-unity_api-v2-CoApiClient-GetObjectDistance-System-String,System-String,System-Int32-'></a>
### GetObjectDistance(objectA_HierarchyPath,objectB_HierarchyPath,timeout) `method`

##### Summary

This method returns the distance of two objects using vector subtraction.

##### Returns

Returns the distance between the two objects as a float.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| objectA_HierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the first GameObject. |
| objectB_HierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchYpath for the second GameObject. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
// CubeA.Transform = Vector3(1, 2, 3)
            // CubeB.Transform = Vector3(6, 5, 4)
            d = api.GetObjectDistance("//*[@name = 'CubeA']", "//*[@name = 'CubeB']");
            Console.WriteLine(d.ToString()); // prints -5.0,-3.0,-1.0
```

<a name='M-gdio-unity_api-v2-CoApiClient-GetObjectFieldValue<T>-System-String,System-Int32-'></a>
### GetObjectFieldValue<T>(hierarchyPath,timeout) `method`

##### Summary

This method returns the field or property value of an object.

##### Returns

Returns an object of type T for the value or throws an [Exception](https://docs.microsoft.com/en-us/dotnet/api/System.Exception 'System.Exception') on error.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath of the object and field/property to be inspected. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Generic Types

| Name | Description |
| ---- | ----------- |
| T | The [Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type') of the field or property to be inspected. |

##### Example

// Searches for an object named 'HiddenCube' which is invisible in the scene, and checks whether the "Active" checkbox is enabled.

```
bool invisCube = api.GetObjectFieldValue&lt;bool&gt;("//*[@name='HiddenCube']/fn:component('UnityEngine.Behaviour')/@isActiveAndEnabled");
Assert.IsTrue(invisCube == false, "The invisible cube isn't active"); //Passes if the object is Active in the scene
```

<a name='M-gdio-unity_api-v2-CoApiClient-GetObjectFieldValue<T>-System-String,System-String,System-Int32-'></a>
### GetObjectFieldValue<T>(hierarchyPath,fieldOrPropertyName,timeout) `method`

##### Summary

This method returns the field or property value of an object.

##### Returns

Returns an object of type T for the value or throws an [Exception](https://docs.microsoft.com/en-us/dotnet/api/System.Exception 'System.Exception') on error.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath of the object and field/property to be inspected. |
| fieldOrPropertyName | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The field/property name to retreieve the value for/ |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Generic Types

| Name | Description |
| ---- | ----------- |
| T | The [Type](https://docs.microsoft.com/en-us/dotnet/api/System.Type 'System.Type') of the field or property to be inspected. |

##### Example

// Searches for an object named 'HiddenCube' which is invisible in the scene, and checks whether the "Active" checkbox is enabled.

```
bool invisCube = api.GetObjectFieldValue&lt;bool&gt;("//*[@name='HiddenCube']/fn:component('UnityEngine.Behaviour')", "isActiveAndEnabled");
Assert.IsTrue(invisCube == false, "The invisible cube isn't active"); //Passes if the object is Active in the scene
```

<a name='M-gdio-unity_api-v2-CoApiClient-GetObjectList-System-Int32-'></a>
### GetObjectList(timeout) `method`

##### Summary

This method returns of a list of all GameObjects as returned by [](#!-UnityEngine-GameObject-FindObjectsOfType-Type- 'UnityEngine.GameObject.FindObjectsOfType(Type)'), where Type is UnityEngine.GameObject./>

##### Returns

This method returns a [IList](https://docs.microsoft.com/en-us/dotnet/api/System.Collections.IList 'System.Collections.IList') of [LiteGameObject](#T-gdio-common-objects-LiteGameObject 'gdio.common.objects.LiteGameObject').  LiteGameObject is a slimmer representation of UnityEngine.GameObject

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

//Print a list of the scene objects

```
 System.Collections.Generic.List&lt;LiteGameObject&gt; objects = api.GetObjectList();
 //Test whether the list is null
 Assert.IsNotNull(objects, "GetObjectList failed!");
 //Print a full object list
 foreach (var obj in objects)
 {
     Console.WriteLine("Object Name: " + obj.Name);
     Console.WriteLine("Object Tag: " + obj.Tag);
     Console.WriteLine("Object Position: " + obj.Position);
     Console.WriteLine($"Object Rotation (w): {obj.Rotation.w}, (x): {obj.Rotation.x}, (y): {obj.Rotation.x}, (z): {obj.Rotation.z}");
 }
 
```

<a name='M-gdio-unity_api-v2-CoApiClient-GetObjectPosition-System-String,gdio-common-objects-CoordinateConversion,System-String,System-Int32-'></a>
### GetObjectPosition(objectHierarchyPath,cordSpace,cameraHierarchyPath,timeout) `method`

##### Summary

Return the position of a specific object.

##### Returns

The Vector3 position of the specific object.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| objectHierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath of the object to return the position of. |
| cordSpace | [gdio.common.objects.CoordinateConversion](#T-gdio-common-objects-CoordinateConversion 'gdio.common.objects.CoordinateConversion') | The coorindate space conversion to perform on the position before returning it. See [CoordinateConversion](#T-gdio-common-objects-CoordinateConversion 'gdio.common.objects.CoordinateConversion') for more information. |
| cameraHierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchPath to the Camera GameObject to use.  The default is string.Empty, which uses Camera.main/> |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
// spot is set to the Vector3 value of the object position on screen
           Vector3 spot = api.GetObjectPosition("//*[@name = 'Player prefab(Clone)']",
               CoordinateConversion.WorldToScreenPoint);
```

<a name='M-gdio-unity_api-v2-CoApiClient-GetSceneName-System-Int32-'></a>
### GetSceneName(timeout) `method`

##### Summary

Return the name of the current active scene.

##### Returns

The name of the scene as a string.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
string activeScene = api.GetSceneName();
```

<a name='M-gdio-unity_api-v2-CoApiClient-GetVersionsString'></a>
### GetVersionsString() `method`

##### Summary

Returns the GameDriver component versions in this build.

##### Parameters

This method has no parameters.

<a name='M-gdio-unity_api-v2-CoApiClient-KeyPress-gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32-'></a>
### KeyPress(keys,numberOfFrames,modifiers,modifierNumberOfFrames,delayAfterModifiersMsec,timeout) `method`

##### Summary

Use this function to send arbitrary button states to the game. Defaults to LEFT ALT/CTRL/SHIFT/WINDOWS(COMMAND)

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| keys | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of keys([KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode')) to press. |
| numberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to press and hold the keys for. |
| modifiers | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of modifiers()[KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') to press. |
| modifierNumberOfFrames | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to hold the modifiers down for, before pressing the keys. |
| delayAfterModifiersMsec | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The delay to wait between holding the modifies and pressing the keys. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
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

<a name='M-gdio-unity_api-v2-CoApiClient-LoadScene-System-String,System-Int32-'></a>
### LoadScene(sceneName,timeout) `method`

##### Summary

This method loads the scene, defined by the scene name passed as an argument.

##### Returns

TRUE if the request was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| sceneName | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The name of the scene to load |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Loads the FinalBoss scene
            api.LoadScene("FinalBoss");
```

<a name='M-gdio-unity_api-v2-CoApiClient-MouseDrag-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,gdio-common-objects-Vector2,System-Boolean,System-Int32-'></a>
### MouseDrag(button,destination,frameCount,origin,waitForEmptyInput,timeout) `method`

##### Summary

Perform a mouse drag operation.

##### Returns

TRUE if the requests was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| button | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button, [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'), to perform the drag operation with. |
| destination | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The destination vector to drag the mouse to. |
| frameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames taken to complete the drag operation. |
| origin | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The origin to start the drag operation.  If null, the mouse drag operation will begin at the current position of Input.mousePosition. |
| waitForEmptyInput | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | Wait for the empty input event to be returned from the agent before returning from the method call. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. If waitForEmptyInput is set to TRUE, then the method call will wait the timeout allotment to recieve the event. |

##### Example

```
//Drags the left mouse button to the position 180, 0 on the screen over 30 frames
            api.MouseDrag(MouseButtons.LEFT, new Vector2(180, 0), 30, start, true);
```

<a name='M-gdio-unity_api-v2-CoApiClient-MouseMoveToObject-System-String,System-UInt64,System-Boolean,System-Boolean,System-Int32-'></a>
### MouseMoveToObject(objectHierarchyPath,frameCount,waitForObject,waitForEmptyInput,timeout) `method`

##### Summary

Move the mouse to the center of a specific object, identified by the HierarchyPath.

##### Returns

TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| objectHierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath to move the mouse pointer to. |
| frameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to compelte the mouse move over. |
| waitForObject | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | If TRUE, wait for the object to exist so that mouse move can complete successfully. |
| waitForEmptyInput | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | Wait for the empty input event to be returned from the GameDriver agent, before returning from the method. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent.  If waitForEmptyInput is TRUE, then the method call will wait the timeout alotment to recieve the event. |

##### Example

```
//Moves the mouse to the center of the object named "Cylinder" over 300 frames
            api.MouseMoveToObject("//*[@name='Cylinder']", 300, true, true);
```

<a name='M-gdio-unity_api-v2-CoApiClient-MoveMouseToPoint-gdio-common-objects-Vector2,System-UInt64,gdio-common-objects-Vector2,System-Boolean,System-Int32-'></a>
### MoveMouseToPoint(destination,frameCount,origin,waitForEmptyInput,timeout) `method`

##### Summary

Move the mouse to the destination vector.

##### Returns

TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| destination | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | Destination vector to move the mouse to. |
| frameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to complete the operaiton over. |
| origin | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The origin to start the mouse move operation.  If null, the mouse move operation will begin at the current position of Input.mousePosition. |
| waitForEmptyInput | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | Wait for the empty input event to be returned from the GameDriver agent, before returning from the method. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent.  If waitForEmptyInput is TRUE, then the method call will wait the timeout alotment to recieve the event. |

##### Example

```
//First get the position of an object named "Cube" on screen
             Vector3 cubePos = api.GetObjectPosition("//*[@name='Cube']", CoordinateConversion.WorldToScreenPoint);
            
             //Take the x,y values of the on-screen object
             Vector2 cubePos2 = new Vector2(cubePos.x, cubePos.y);
             
             //Move the mouse to the cube on-screen position over 30 frames
             api.MoveMouseToPoint(cubePos2, (ulong) api.GetLastFPS());
```

<a name='M-gdio-unity_api-v2-CoApiClient-NavAgentMoveToPoint-System-String,gdio-common-objects-Vector3,System-Boolean,System-Int32-'></a>
### NavAgentMoveToPoint(navAgentHierarchyPath,destination,waitForMoveToComplete,timeout) `method`

##### Summary

Move a NavAgent to a destination point.

##### Returns

TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| navAgentHierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath to the NavAgent. |
| destination | [gdio.common.objects.Vector3](#T-gdio-common-objects-Vector3 'gdio.common.objects.Vector3') | The destination vector to move to. |
| waitForMoveToComplete | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | Wait for the NavAgent move-to operation to complete before the method returns. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Moves the 1st object named "Ellen" to position 20, 0, 20 on the NavMesh
            api.NavAgentMoveToPoint("//*[@name='Ellen']", new Vector3(20, 0, 20));
```

<a name='M-gdio-unity_api-v2-CoApiClient-Raycast-gdio-common-objects-Vector3,System-String,System-Int32-'></a>
### Raycast(raycastPoint,cameraHierarchyPath,timeout) `method`

##### Summary

Perform a Raycast to a point to find out what is in that position.

##### Returns

Returns an array of [RaycastResult](#T-gdio-common-objects-RaycastResult 'gdio.common.objects.RaycastResult').

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| raycastPoint | [gdio.common.objects.Vector3](#T-gdio-common-objects-Vector3 'gdio.common.objects.Vector3') | The vector to perform a raycast to. |
| cameraHierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the  UnityEngine.Camera to use as a Raycast reference.  If the Camera is string.Empty, the Camera.main is used |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
// Racast to an object named "Ellen"
             RaycastResult[] rr = api.Raycast(api.GetObjectPosition("//*[@name='Ellen']"));
             
             foreach (var res in rr)
             {
                 Console.WriteLine(res);
             }
            
             // Output
             // [RaycastResult]
             // Type: Physics
             // Tag: Untagged
             // Name: Plane
             // HasButton: False
             // Point: (-5.217863, 0, -0.5770187)
             // Type Name: UnityEngine.GameObject
             
             
```

<a name='M-gdio-unity_api-v2-CoApiClient-RegisterCollisionMonitor-System-String,System-Int32-'></a>
### RegisterCollisionMonitor(hierarchyPath,timeout) `method`

##### Summary

Register a collision monitor to recieve collision events on an object.

##### Returns

String returned is the event identifier

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the object to rotate. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
api.RegisterCollisionMonitor("//*[@name='Cylinder']");
```

<a name='M-gdio-unity_api-v2-CoApiClient-RotateObject-System-String,gdio-common-objects-Quaternion,System-Boolean,System-Int32-'></a>
### RotateObject(hierarchyPath,quaternion,waitForObject,timeout) `method`

##### Summary

Rotate an object defined by the HierarchyPath and rotated by a Quaternion. for more information.

##### Returns

TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the object to rotate. |
| quaternion | [gdio.common.objects.Quaternion](#T-gdio-common-objects-Quaternion 'gdio.common.objects.Quaternion') | The quaternion value to manipulate the object. |
| waitForObject | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | Wait for the object to exist if it doesn't. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
api.RotateObject("//*[@name='Cylinder']", new Quaternion(0, 0, 2, 2), true);
```

<a name='M-gdio-unity_api-v2-CoApiClient-RotateObject-System-String,gdio-common-objects-Vector3,gdio-common-objects-Space,System-Boolean,System-Int32-'></a>
### RotateObject(hierarchyPath,eulers,relativeTo,waitForObject,timeout) `method`

##### Summary

Rotate an object defined by the HierarchyPath and rotated by Eulers. for more information.

##### Returns

TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the object to rotate. |
| eulers | [gdio.common.objects.Vector3](#T-gdio-common-objects-Vector3 'gdio.common.objects.Vector3') | The Eulers vector to manipulate the object. |
| relativeTo | [gdio.common.objects.Space](#T-gdio-common-objects-Space 'gdio.common.objects.Space') | The [Space](#T-gdio-common-objects-Space 'gdio.common.objects.Space') to perform the rotation relative to. |
| waitForObject | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | Wait for the object to exist if it doesn't. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Rotates an object with the name "Cylinder" by 30 degrees on the y axis.
            api.RotateObject("//*[@name='Cylinder']", new Vector3(0, 30, 0), Space.Self, true);
```

<a name='M-gdio-unity_api-v2-CoApiClient-RotateObject-System-String,System-Single,System-Single,System-Single,gdio-common-objects-Space,System-Boolean,System-Int32-'></a>
### RotateObject(hierarchyPath,xAngle,yAngle,zAngle,relativeTo,waitForObject,timeout) `method`

##### Summary

Rotate an object defined by the HierarchyPath and rotated by the x, y, and z angles relative to the Space

##### Returns

TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the object to rotate. |
| xAngle | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The X angle value to rotate. |
| yAngle | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The Y angle value to rotate. |
| zAngle | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The Z angle value to rotate. |
| relativeTo | [gdio.common.objects.Space](#T-gdio-common-objects-Space 'gdio.common.objects.Space') | The [Space](#T-gdio-common-objects-Space 'gdio.common.objects.Space') to perform the rotation relative to. |
| waitForObject | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | Wait for the object to exist if it doesn't. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Rotates an object with the name "Cylinder" by 20 degrees on the z axis
            api.RotateObject("//*[@name='Cylinder']", 0, 0, 20);
```

<a name='M-gdio-unity_api-v2-CoApiClient-RotateObject-System-String,gdio-common-objects-Vector3,System-Single,gdio-common-objects-Space,System-Boolean,System-Int32-'></a>
### RotateObject(hierarchyPath,axis,angle,relativeTo,waitForObject,timeout) `method`

##### Summary

Rotate an object defined by the HierarchyPath and rotated by the axis and angle, relative to the Space

##### Returns

TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath for the object to rotate. |
| axis | [gdio.common.objects.Vector3](#T-gdio-common-objects-Vector3 'gdio.common.objects.Vector3') |  |
| angle | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') |  |
| relativeTo | [gdio.common.objects.Space](#T-gdio-common-objects-Space 'gdio.common.objects.Space') | The [Space](#T-gdio-common-objects-Space 'gdio.common.objects.Space') to perform the rotation relative to. |
| waitForObject | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | Wait for the object to exist if it doesn't. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Will rotate an object named "Cylinder" on all 3 axis by 45-degrees
            api.RotateObject("//*[@name='Cylinder']", new Vector3(0, 0, 0), 45);
```

<a name='M-gdio-unity_api-v2-CoApiClient-SetInputFieldText-System-String,System-String,System-Boolean,System-Int32-'></a>
### SetInputFieldText(hierarchyPath,value,waitForObject,timeout) `method`

##### Summary

Set the text of an InputField or TMP_InputField

##### Returns

TRUE if the GameDriver agent was able to successfully set the InputField text.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath to the InputField or TMP_InputField. |
| value | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The text value to set in the field. |
| waitForObject | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | If TRUE, wait for the object to exist if it doesn't. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The time to wait for the object to exist. |

##### Example

```
//Sets the text field component attached to the "TextMeshPro InputField" object with the tag "FilterInputTxt" to the value of "America"
            api.SetInputFieldText("//FilterInputTxt[@name='TextMeshPro InputField']", "America");
```

<a name='M-gdio-unity_api-v2-CoApiClient-SetObjectFieldValue-System-String,System-String,System-Object,System-Boolean,System-Int32,gdio-plugin-serializer-ICustomSerializer-'></a>
### SetObjectFieldValue(hierarchyPath,fieldOrPropertyName,value,waitForObject,timeout,valueSerializer) `method`

##### Summary

Set the field or property of an object.

##### Returns

TRUE if the field/property was successfully set to the value.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath to the object to set the field/property value. |
| fieldOrPropertyName | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The field or property name to set the value of. |
| value | [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') | The value to set for the field/property. |
| waitForObject | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | If TRUE, wait for the object to exist if it doesn't. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The time to wait for the object to exist. |
| valueSerializer | [gdio.plugin.serializer.ICustomSerializer](#T-gdio-plugin-serializer-ICustomSerializer 'gdio.plugin.serializer.ICustomSerializer') | The [ICustomSerializer](#T-gdio-plugin-serializer-ICustomSerializer 'gdio.plugin.serializer.ICustomSerializer') used to serialize the value.  This is only required if a a custom class of object is being used. |

##### Example

```
//Sets the text field component attached to the "TextMeshPro InputField" object with the tag "FilterInputTxt" to the value of "Asia"
            api.SetObjectFieldValue("/Untagged[@name='Canvas']/FilterInputTxt[@name='TextMeshPro InputField']/fn:component('TMPro.TMP_InputField')", "text", "string:Asia");
```

<a name='M-gdio-unity_api-v2-CoApiClient-Tap-gdio-common-objects-Vector2,System-Int32,System-UInt64,System-Int32-'></a>
### Tap(position,tapCount,frameCount,timeout) `method`

##### Summary

Tap the handheld device at the defined position.

##### Returns

TRUE if the GameDriver agent was able to process the request successfully.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| position | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The vector position to tap the device screen. |
| tapCount | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of taps that should be registered. |
| frameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to complete the tap input over. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Performs a single tap at position 0, 0 for 10 frames
            api.Tap(new Vector2(0, 0), 1, 10); 
```

<a name='M-gdio-unity_api-v2-CoApiClient-Tap-System-Single,System-Single,System-Int32,System-UInt64,System-Int32-'></a>
### Tap(x,y,tapCount,frameCount,timeout) `method`

##### Summary

Tap the handheld device at the defined position.

##### Returns

TRUE if the GameDriver agent was able to process the request successfully.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| x | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The X coordinate of the position to tap the device screen. |
| y | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The Y coordinate position to tap the device screen. |
| tapCount | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of taps that should be registered. |
| frameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to complete the tap input over. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Performs a single tap at position 0, 0 for 10 frames
            api.Tap(0, 0, 1, 10);
```

<a name='M-gdio-unity_api-v2-CoApiClient-TapObject-System-String,System-Int32,System-UInt64,System-Int32-'></a>
### TapObject(hierarchyPath,tapCount,frameCount,timeout) `method`

##### Summary

Tap an object.

##### Returns

TRUE if the GameDriver agent was able to process the request successfully.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath of the object to tap. |
| tapCount | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of taps that should be registered. |
| frameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to complete the tap input over. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Performs a single tap on an object with the name "Cube"
            api.TapObject("//*[@name='Cube']", 1, 10);
```

<a name='M-gdio-unity_api-v2-CoApiClient-TouchInput-gdio-common-objects-Vector2,gdio-common-objects-Vector2,System-Int32,System-Int32,System-UInt64,System-Boolean,System-Single,System-Single,System-Single,System-Single,System-Single,System-Int32-'></a>
### TouchInput(startPosition,destinationPosition,fingerId,tapCount,frameCount,waitForEmptyInput,radius,pressure,altitudeAngle,azmulthAngle,maximumPossiblePressure,timeout) `method`

##### Summary

Send a raw TouchInput event to the game.

##### Returns

TRUE if the GameDriver agent was able to process the request successfully.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| startPosition | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | Vector position of the start of the touch input. |
| destinationPosition | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | Vector destination position of where the touch input ends. |
| fingerId | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The finder id of the touch input. |
| tapCount | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of taps that should be registered. |
| frameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to complete the tap input over. |
| waitForEmptyInput | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | If TRUE, wait for the Empty Input event to be broadcast before returning from the method. |
| radius | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The radius of the touch input. |
| pressure | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The pressure of the touch input. |
| altitudeAngle | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The altitude angle of the touch input. |
| azmulthAngle | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The azmulth ange of the touch input. |
| maximumPossiblePressure | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The maximum possible pressure for the touch input. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Performs a single touch input from 0,0 to 100, 100 with a single "finger" over a duration of 50 frames
            api.TouchInput(new Vector2(0, 0), new Vector2(100, 100), 0, 1, 50);
```

<a name='M-gdio-unity_api-v2-CoApiClient-TouchInput-System-Single,System-Single,System-Single,System-Single,System-Int32,System-Int32,System-UInt64,System-Boolean,System-Single,System-Single,System-Single,System-Single,System-Single,System-Int32-'></a>
### TouchInput(x1,y1,x2,y2,fingerId,tapCount,frameCount,waitForEmptyInput,radius,pressure,altitudeAngle,azmulthAngle,maximumPossiblePressure,timeout) `method`

##### Summary

Send a raw TouchInput event to the game.

##### Returns

TRUE if the GameDriver agent was able to process the request successfully.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| x1 | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The X coordinate of the start position. |
| y1 | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The Y coordinate of the start position. |
| x2 | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The X coordinate of the end position. |
| y2 | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The Y coordinate of the end position. |
| fingerId | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The finder id of the touch input. |
| tapCount | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of taps that should be registered. |
| frameCount | [System.UInt64](https://docs.microsoft.com/en-us/dotnet/api/System.UInt64 'System.UInt64') | The number of frames to complete the tap input over. |
| waitForEmptyInput | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | If TRUE, wait for the Empty Input event to be broadcast before returning from the method. |
| radius | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The radius of the touch input. |
| pressure | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The pressure of the touch input. |
| altitudeAngle | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The altitude angle of the touch input. |
| azmulthAngle | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The azmulth ange of the touch input. |
| maximumPossiblePressure | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') | The maximum possible pressure for the touch input. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Example

```
//Performs a single touch input from 0,0 to 100, 100 with a single "finger" over a duration of 50 frames
            api.TouchInput(0, 0, 100, 100, 0, 1, 50);
```

<a name='M-gdio-unity_api-v2-CoApiClient-UnregisterCollisionMonitor-System-String,System-Int32-'></a>
### UnregisterCollisionMonitor(hierarchyPath,timeout) `method`

##### Summary

Unregister the monitoring of collision events on a GameObject that has been previously registered for monitoring.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') |  |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') |  |

<a name='M-gdio-unity_api-v2-CoApiClient-Wait-System-Single-'></a>
### Wait(waitMaxSeconds) `method`

##### Summary

Wait for a fixed period of seconds.

##### Returns



##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| waitMaxSeconds | [System.Single](https://docs.microsoft.com/en-us/dotnet/api/System.Single 'System.Single') |  |

<a name='M-gdio-unity_api-v2-CoApiClient-WaitForCollisionEvent-System-String,System-Int32-'></a>
### WaitForCollisionEvent(eventId,timeout) `method`

##### Summary

Wait for a collision event to fire on an element that is being monitored for collisions.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| eventId | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The eventId received from the [RegisterCollisionMonitor](#M-gdio-unity_api-v2-CoApiClient-RegisterCollisionMonitor-System-String,System-Int32- 'gdio.unity_api.v2.CoApiClient.RegisterCollisionMonitor(System.String,System.Int32)') call. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a collision event to be fired. |

##### Example

```
api.WaitForCollisionEvent(eventId);
```

<a name='M-gdio-unity_api-v2-CoApiClient-WaitForCollisionEvent<T>-System-String,System-Int32-'></a>
### WaitForCollisionEvent<T>(eventId,timeout) `method`

##### Summary

Wait for a collision event to fire on an element that is being monitored for collisions. If the method has been called before, there is the potential that another event was recieved before waiting on the event again.  
Check with [GetNextCollisionEvent<T>](#M-gdio-unity_api-v2-CoApiClient-GetNextCollisionEvent<T>-System-String- 'gdio.unity_api.v2.CoApiClient.GetNextCollisionEvent<T>(System.String)') to see if it returns null to see if an event was missed.

##### Returns

The collision messages. TODO: Return a translated collisionInfo object

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| eventId | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The eventId received from the [RegisterCollisionMonitor](#M-gdio-unity_api-v2-CoApiClient-RegisterCollisionMonitor-System-String,System-Int32- 'gdio.unity_api.v2.CoApiClient.RegisterCollisionMonitor(System.String,System.Int32)') call. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The number of seconds to wait for a collision event to be fired. |

##### Example

```
api.WaitForCollisionEvent{object}(eventId);
```

<a name='M-gdio-unity_api-v2-CoApiClient-WaitForEmptyInput-System-Int32-'></a>
### WaitForEmptyInput(timeout) `method`

##### Summary

Wait for an Empty Input event to be received.

##### Returns



##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The time to wait for the event. |

<a name='M-gdio-unity_api-v2-CoApiClient-WaitForFixedUpdate'></a>
### WaitForFixedUpdate() `method`

##### Summary

Wait for a fixed update in the UnityEngine game loop.

##### Returns



##### Parameters

This method has no parameters.

<a name='M-gdio-unity_api-v2-CoApiClient-WaitForObject-System-String,System-Int32-'></a>
### WaitForObject(hierarchyPath,timeout) `method`

##### Summary

Wait for an object to exist.

##### Returns

Returns TRUE if the object exists within the alloted timeout.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath of the object. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The amount of time to wait for the object to exist. |

<a name='M-gdio-unity_api-v2-CoApiClient-WaitForObjectValue-System-String,System-String,System-Object,System-Boolean,System-Int32,gdio-plugin-serializer-ICustomSerializer-'></a>
### WaitForObjectValue(hierarchyPath,fieldOrPropertyName,value,waitForObject,timeout,valueSerializer) `method`

##### Summary

Wait for an object to exist and have a specific value for a specified field/property.

##### Returns

TRUE if the object exists with the specified value in the alloted timeout.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The HierarchyPath to the object. |
| fieldOrPropertyName | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') | The field/property name for inspection. |
| value | [System.Object](https://docs.microsoft.com/en-us/dotnet/api/System.Object 'System.Object') | The value to wait for. |
| waitForObject | [System.Boolean](https://docs.microsoft.com/en-us/dotnet/api/System.Boolean 'System.Boolean') | If TRUE, wait for the object to exist if it doesn't. |
| timeout | [System.Int32](https://docs.microsoft.com/en-us/dotnet/api/System.Int32 'System.Int32') | The amount of time to wait for the object to exist with the specified value. |
| valueSerializer | [gdio.plugin.serializer.ICustomSerializer](#T-gdio-plugin-serializer-ICustomSerializer 'gdio.plugin.serializer.ICustomSerializer') | The [ICustomSerializer](#T-gdio-plugin-serializer-ICustomSerializer 'gdio.plugin.serializer.ICustomSerializer') used to serialize the value.  This is only required if a a custom class of object is being used. |

##### Example

```
//Waits for the value of the TextMeshProUGUI input field with the name "Text" to be "America"
            api.WaitForObjectValue("//*[@name='Text']/fn:component('TMPro.TextMeshProUGUI')", "text", "America");
```

<a name='T-gdio-unity_api-utilities-ScreenCapture'></a>
## ScreenCapture `type`

##### Namespace

gdio.unity_api.utilities

##### Summary

Provides functions to capture the entire screen, or a particular window, and save it to a file.

<a name='M-gdio-unity_api-utilities-ScreenCapture-CaptureScreen'></a>
### CaptureScreen() `method`

##### Summary

Creates an Image object containing a screen shot of the entire desktop

##### Returns



##### Parameters

This method has no parameters.

<a name='M-gdio-unity_api-utilities-ScreenCapture-CaptureScreenToFile-System-String,System-Drawing-Imaging-ImageFormat-'></a>
### CaptureScreenToFile(filename,format) `method`

##### Summary

Captures a screen shot of the entire desktop, and saves it to a file

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| filename | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') |  |
| format | [System.Drawing.Imaging.ImageFormat](https://docs.microsoft.com/en-us/dotnet/api/System.Drawing.Imaging.ImageFormat 'System.Drawing.Imaging.ImageFormat') |  |

<a name='M-gdio-unity_api-utilities-ScreenCapture-CaptureWindow-System-IntPtr-'></a>
### CaptureWindow(handle) `method`

##### Summary

Creates an Image object containing a screen shot of a specific window

##### Returns



##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| handle | [System.IntPtr](https://docs.microsoft.com/en-us/dotnet/api/System.IntPtr 'System.IntPtr') | The handle to the window. (In windows forms, this is obtained by the Handle property) |

<a name='M-gdio-unity_api-utilities-ScreenCapture-CaptureWindowToFile-System-IntPtr,System-String,System-Drawing-Imaging-ImageFormat-'></a>
### CaptureWindowToFile(handle,filename,format) `method`

##### Summary

Captures a screen shot of a specific window, and saves it to a file

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| handle | [System.IntPtr](https://docs.microsoft.com/en-us/dotnet/api/System.IntPtr 'System.IntPtr') |  |
| filename | [System.String](https://docs.microsoft.com/en-us/dotnet/api/System.String 'System.String') |  |
| format | [System.Drawing.Imaging.ImageFormat](https://docs.microsoft.com/en-us/dotnet/api/System.Drawing.Imaging.ImageFormat 'System.Drawing.Imaging.ImageFormat') |  |

<a name='T-gdio-unity_api-utilities-ScreenCapture-User32'></a>
## User32 `type`

##### Namespace

gdio.unity_api.utilities.ScreenCapture

##### Summary

Helper class containing User32 API functions
