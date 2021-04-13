# gdio.unity_api.doc
Documentation for the GameDriver Unity API
<a name='assembly'></a>
# gdio.unity_api

## Contents

- [ApiClient](#T-gdio-unity_api-v2-ApiClient 'gdio.unity_api.v2.ApiClient')
  - [#ctor()](#M-gdio-unity_api-v2-ApiClient-#ctor 'gdio.unity_api.v2.ApiClient.#ctor')
  - [AUTOPLAY_DEFAULT_PORT](#F-gdio-unity_api-v2-ApiClient-AUTOPLAY_DEFAULT_PORT 'gdio.unity_api.v2.ApiClient.AUTOPLAY_DEFAULT_PORT')
  - [AUTOPLAY_ENABLED](#F-gdio-unity_api-v2-ApiClient-AUTOPLAY_ENABLED 'gdio.unity_api.v2.ApiClient.AUTOPLAY_ENABLED')
  - [AUTOPLAY_RECEIVE_PORT](#F-gdio-unity_api-v2-ApiClient-AUTOPLAY_RECEIVE_PORT 'gdio.unity_api.v2.ApiClient.AUTOPLAY_RECEIVE_PORT')
  - [THROW_EXCEPTIONS](#F-gdio-unity_api-v2-ApiClient-THROW_EXCEPTIONS 'gdio.unity_api.v2.ApiClient.THROW_EXCEPTIONS')
  - [CallMethod(hierarchyPath,methodName,arguments,timeout)](#M-gdio-unity_api-v2-ApiClient-CallMethod-System-String,System-String,System-Object[],System-Int32- 'gdio.unity_api.v2.ApiClient.CallMethod(System.String,System.String,System.Object[],System.Int32)')
  - [CallMethod\`\`1(hierarchyPath,methodName,arguments,timeout)](#M-gdio-unity_api-v2-ApiClient-CallMethod``1-System-String,System-String,System-Object[],System-Int32- 'gdio.unity_api.v2.ApiClient.CallMethod``1(System.String,System.String,System.Object[],System.Int32)')
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
  - [GetObjectDistance(objectA_HierarchyPath,objectB_HierarchyPath,timeout)](#M-gdio-unity_api-v2-ApiClient-GetObjectDistance-System-String,System-String,System-Int32- 'gdio.unity_api.v2.ApiClient.GetObjectDistance(System.String,System.String,System.Int32)')
  - [GetObjectFieldValue\`\`1(hierarchyPath,timeout)](#M-gdio-unity_api-v2-ApiClient-GetObjectFieldValue``1-System-String,System-Int32- 'gdio.unity_api.v2.ApiClient.GetObjectFieldValue``1(System.String,System.Int32)')
  - [GetObjectList(timeout)](#M-gdio-unity_api-v2-ApiClient-GetObjectList-System-Int32- 'gdio.unity_api.v2.ApiClient.GetObjectList(System.Int32)')
  - [GetObjectPosition(objectHierarchyPath,cordSpace,cameraHierarchyPath,timeout)](#M-gdio-unity_api-v2-ApiClient-GetObjectPosition-System-String,gdio-common-objects-CoordinateConversion,System-String,System-Int32- 'gdio.unity_api.v2.ApiClient.GetObjectPosition(System.String,gdio.common.objects.CoordinateConversion,System.String,System.Int32)')
  - [GetSceneName(timeout)](#M-gdio-unity_api-v2-ApiClient-GetSceneName-System-Int32- 'gdio.unity_api.v2.ApiClient.GetSceneName(System.Int32)')
  - [GetVersionsString()](#M-gdio-unity_api-v2-ApiClient-GetVersionsString 'gdio.unity_api.v2.ApiClient.GetVersionsString')
  - [KeyPress(keys,numberOfFrames,modifiers,modifierNumberOfFrames,delayAfterModifiersMsec,timeout)](#M-gdio-unity_api-v2-ApiClient-KeyPress-gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32- 'gdio.unity_api.v2.ApiClient.KeyPress(gdio.unity_api.KeyCode[],System.UInt64,gdio.unity_api.KeyCode[],System.UInt64,System.Int32,System.Int32)')
  - [LoadScene(sceneName,timeout)](#M-gdio-unity_api-v2-ApiClient-LoadScene-System-String,System-Int32- 'gdio.unity_api.v2.ApiClient.LoadScene(System.String,System.Int32)')
  - [MouseDrag(button,destination,frameCount,origin,waitForEmptyInput,timeout)](#M-gdio-unity_api-v2-ApiClient-MouseDrag-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,gdio-common-objects-Vector2,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.MouseDrag(gdio.common.objects.MouseButtons,gdio.common.objects.Vector2,System.UInt64,gdio.common.objects.Vector2,System.Boolean,System.Int32)')
  - [MouseMoveToObject(objectHierarchyPath,frameCount,waitForObject,waitForEmptyInput,timeout)](#M-gdio-unity_api-v2-ApiClient-MouseMoveToObject-System-String,System-UInt64,System-Boolean,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.MouseMoveToObject(System.String,System.UInt64,System.Boolean,System.Boolean,System.Int32)')
  - [MoveMouseToPoint(desintation,frameCount,origin,waitForEmptyInput,timeout)](#M-gdio-unity_api-v2-ApiClient-MoveMouseToPoint-gdio-common-objects-Vector2,System-UInt64,gdio-common-objects-Vector2,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.MoveMouseToPoint(gdio.common.objects.Vector2,System.UInt64,gdio.common.objects.Vector2,System.Boolean,System.Int32)')
  - [NavAgentMoveToPoint(navAgentHierarchyPath,desintation,waitForMoveToComplete,timeout)](#M-gdio-unity_api-v2-ApiClient-NavAgentMoveToPoint-System-String,gdio-common-objects-Vector3,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.NavAgentMoveToPoint(System.String,gdio.common.objects.Vector3,System.Boolean,System.Int32)')
  - [Raycast(raycastPoint,cameraHierarchyPath,timeout)](#M-gdio-unity_api-v2-ApiClient-Raycast-gdio-common-objects-Vector3,System-String,System-Int32- 'gdio.unity_api.v2.ApiClient.Raycast(gdio.common.objects.Vector3,System.String,System.Int32)')
  - [RotateObject(hierarchyPath,quaternion,waitForObject,timeout)](#M-gdio-unity_api-v2-ApiClient-RotateObject-System-String,gdio-common-objects-Quaternion,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.RotateObject(System.String,gdio.common.objects.Quaternion,System.Boolean,System.Int32)')
  - [RotateObject(hierarchyPath,eulers,relativeTo,waitForObject,timeout)](#M-gdio-unity_api-v2-ApiClient-RotateObject-System-String,gdio-common-objects-Vector3,gdio-common-objects-Space,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.RotateObject(System.String,gdio.common.objects.Vector3,gdio.common.objects.Space,System.Boolean,System.Int32)')
  - [RotateObject(hierarchyPath,xAngle,yAngle,zAngle,relativeTo,waitForObject,timeout)](#M-gdio-unity_api-v2-ApiClient-RotateObject-System-String,System-Single,System-Single,System-Single,gdio-common-objects-Space,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.RotateObject(System.String,System.Single,System.Single,System.Single,gdio.common.objects.Space,System.Boolean,System.Int32)')
  - [RotateObject(hierarchyPath,axis,angle,relativeTo,waitForObject,timeout)](#M-gdio-unity_api-v2-ApiClient-RotateObject-System-String,gdio-common-objects-Vector3,System-Single,gdio-common-objects-Space,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.RotateObject(System.String,gdio.common.objects.Vector3,System.Single,gdio.common.objects.Space,System.Boolean,System.Int32)')
  - [SetInputFieldText(hierarchyPath,value,waitForObject,timeout)](#M-gdio-unity_api-v2-ApiClient-SetInputFieldText-System-String,System-String,System-Boolean,System-Int32- 'gdio.unity_api.v2.ApiClient.SetInputFieldText(System.String,System.String,System.Boolean,System.Int32)')
  - [SetObjectFieldValue(hierarchyPath,fieldOrPropertyName,value,waitForObject,timeout,valueSerializer)](#M-gdio-unity_api-v2-ApiClient-SetObjectFieldValue-System-String,System-String,System-Object,System-Boolean,System-Int32,gdio-plugin-serializer-ICustomSerializer- 'gdio.unity_api.v2.ApiClient.SetObjectFieldValue(System.String,System.String,System.Object,System.Boolean,System.Int32,gdio.plugin.serializer.ICustomSerializer)')
  - [Tap(position,tapCount,frameCount,timeout)](#M-gdio-unity_api-v2-ApiClient-Tap-gdio-common-objects-Vector2,System-Int32,System-UInt64,System-Int32- 'gdio.unity_api.v2.ApiClient.Tap(gdio.common.objects.Vector2,System.Int32,System.UInt64,System.Int32)')
  - [Tap(x,y,tapCount,frameCount,timeout)](#M-gdio-unity_api-v2-ApiClient-Tap-System-Single,System-Single,System-Int32,System-UInt64,System-Int32- 'gdio.unity_api.v2.ApiClient.Tap(System.Single,System.Single,System.Int32,System.UInt64,System.Int32)')
  - [TapObject(hierarchyPath,tapCount,frameCount,timeout)](#M-gdio-unity_api-v2-ApiClient-TapObject-System-String,System-Int32,System-UInt64,System-Int32- 'gdio.unity_api.v2.ApiClient.TapObject(System.String,System.Int32,System.UInt64,System.Int32)')
  - [TouchInput(startPosition,destinationPosition,fingerId,tapCount,frameCount,waitForEmptyInput,radius,pressure,altitudeAngle,azmulthAngle,maximumPossiblePressure,timeout)](#M-gdio-unity_api-v2-ApiClient-TouchInput-gdio-common-objects-Vector2,gdio-common-objects-Vector2,System-Int32,System-Int32,System-UInt64,System-Boolean,System-Single,System-Single,System-Single,System-Single,System-Single,System-Int32- 'gdio.unity_api.v2.ApiClient.TouchInput(gdio.common.objects.Vector2,gdio.common.objects.Vector2,System.Int32,System.Int32,System.UInt64,System.Boolean,System.Single,System.Single,System.Single,System.Single,System.Single,System.Int32)')
  - [TouchInput(x1,y1,x2,y2,fingerId,tapCount,frameCount,waitForEmptyInput,radius,pressure,altitudeAngle,azmulthAngle,maximumPossiblePressure,timeout)](#M-gdio-unity_api-v2-ApiClient-TouchInput-System-Single,System-Single,System-Single,System-Single,System-Int32,System-Int32,System-UInt64,System-Boolean,System-Single,System-Single,System-Single,System-Single,System-Single,System-Int32- 'gdio.unity_api.v2.ApiClient.TouchInput(System.Single,System.Single,System.Single,System.Single,System.Int32,System.Int32,System.UInt64,System.Boolean,System.Single,System.Single,System.Single,System.Single,System.Single,System.Int32)')
  - [Wait(milliSeconds)](#M-gdio-unity_api-v2-ApiClient-Wait-System-Int32- 'gdio.unity_api.v2.ApiClient.Wait(System.Int32)')
  - [WaitForObject(hierarchyPath,timeout)](#M-gdio-unity_api-v2-ApiClient-WaitForObject-System-String,System-Int32- 'gdio.unity_api.v2.ApiClient.WaitForObject(System.String,System.Int32)')
  - [WaitForObjectValue(hierarchyPath,fieldOrPropertyName,value,waitForObject,timeout,valueSerializer)](#M-gdio-unity_api-v2-ApiClient-WaitForObjectValue-System-String,System-String,System-Object,System-Boolean,System-Int32,gdio-plugin-serializer-ICustomSerializer- 'gdio.unity_api.v2.ApiClient.WaitForObjectValue(System.String,System.String,System.Object,System.Boolean,System.Int32,gdio.plugin.serializer.ICustomSerializer)')
- [GDI32](#T-gdio-unity_api-utilities-ScreenCapture-GDI32 'gdio.unity_api.utilities.ScreenCapture.GDI32')
- [GameConnectionDetails](#T-gdio-unity_api-v2-GameConnectionDetails 'gdio.unity_api.v2.GameConnectionDetails')
  - [Addr](#F-gdio-unity_api-v2-GameConnectionDetails-Addr 'gdio.unity_api.v2.GameConnectionDetails.Addr')
  - [GamePath](#F-gdio-unity_api-v2-GameConnectionDetails-GamePath 'gdio.unity_api.v2.GameConnectionDetails.GamePath')
  - [IsEditor](#F-gdio-unity_api-v2-GameConnectionDetails-IsEditor 'gdio.unity_api.v2.GameConnectionDetails.IsEditor')
  - [IsStandalone](#F-gdio-unity_api-v2-GameConnectionDetails-IsStandalone 'gdio.unity_api.v2.GameConnectionDetails.IsStandalone')
  - [Platform](#F-gdio-unity_api-v2-GameConnectionDetails-Platform 'gdio.unity_api.v2.GameConnectionDetails.Platform')
  - [Port](#F-gdio-unity_api-v2-GameConnectionDetails-Port 'gdio.unity_api.v2.GameConnectionDetails.Port')
- [HookingObject](#T-gdio-unity_api-v2-HookingObject 'gdio.unity_api.v2.HookingObject')
  - [ALL](#F-gdio-unity_api-v2-HookingObject-ALL 'gdio.unity_api.v2.HookingObject.ALL')
  - [GAMEPAD](#F-gdio-unity_api-v2-HookingObject-GAMEPAD 'gdio.unity_api.v2.HookingObject.GAMEPAD')
  - [KEYBOARD](#F-gdio-unity_api-v2-HookingObject-KEYBOARD 'gdio.unity_api.v2.HookingObject.KEYBOARD')
  - [MOUSE](#F-gdio-unity_api-v2-HookingObject-MOUSE 'gdio.unity_api.v2.HookingObject.MOUSE')
  - [TOUCHINPUT](#F-gdio-unity_api-v2-HookingObject-TOUCHINPUT 'gdio.unity_api.v2.HookingObject.TOUCHINPUT')
- [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode')
  - [A](#F-gdio-unity_api-KeyCode-A 'gdio.unity_api.KeyCode.A')
  - [Alpha0](#F-gdio-unity_api-KeyCode-Alpha0 'gdio.unity_api.KeyCode.Alpha0')
  - [Alpha1](#F-gdio-unity_api-KeyCode-Alpha1 'gdio.unity_api.KeyCode.Alpha1')
  - [Alpha2](#F-gdio-unity_api-KeyCode-Alpha2 'gdio.unity_api.KeyCode.Alpha2')
  - [Alpha3](#F-gdio-unity_api-KeyCode-Alpha3 'gdio.unity_api.KeyCode.Alpha3')
  - [Alpha4](#F-gdio-unity_api-KeyCode-Alpha4 'gdio.unity_api.KeyCode.Alpha4')
  - [Alpha5](#F-gdio-unity_api-KeyCode-Alpha5 'gdio.unity_api.KeyCode.Alpha5')
  - [Alpha6](#F-gdio-unity_api-KeyCode-Alpha6 'gdio.unity_api.KeyCode.Alpha6')
  - [Alpha7](#F-gdio-unity_api-KeyCode-Alpha7 'gdio.unity_api.KeyCode.Alpha7')
  - [Alpha8](#F-gdio-unity_api-KeyCode-Alpha8 'gdio.unity_api.KeyCode.Alpha8')
  - [Alpha9](#F-gdio-unity_api-KeyCode-Alpha9 'gdio.unity_api.KeyCode.Alpha9')
  - [AltGr](#F-gdio-unity_api-KeyCode-AltGr 'gdio.unity_api.KeyCode.AltGr')
  - [Ampersand](#F-gdio-unity_api-KeyCode-Ampersand 'gdio.unity_api.KeyCode.Ampersand')
  - [Asterisk](#F-gdio-unity_api-KeyCode-Asterisk 'gdio.unity_api.KeyCode.Asterisk')
  - [At](#F-gdio-unity_api-KeyCode-At 'gdio.unity_api.KeyCode.At')
  - [B](#F-gdio-unity_api-KeyCode-B 'gdio.unity_api.KeyCode.B')
  - [BackQuote](#F-gdio-unity_api-KeyCode-BackQuote 'gdio.unity_api.KeyCode.BackQuote')
  - [Backslash](#F-gdio-unity_api-KeyCode-Backslash 'gdio.unity_api.KeyCode.Backslash')
  - [Backspace](#F-gdio-unity_api-KeyCode-Backspace 'gdio.unity_api.KeyCode.Backspace')
  - [Break](#F-gdio-unity_api-KeyCode-Break 'gdio.unity_api.KeyCode.Break')
  - [C](#F-gdio-unity_api-KeyCode-C 'gdio.unity_api.KeyCode.C')
  - [CapsLock](#F-gdio-unity_api-KeyCode-CapsLock 'gdio.unity_api.KeyCode.CapsLock')
  - [Caret](#F-gdio-unity_api-KeyCode-Caret 'gdio.unity_api.KeyCode.Caret')
  - [Clear](#F-gdio-unity_api-KeyCode-Clear 'gdio.unity_api.KeyCode.Clear')
  - [Colon](#F-gdio-unity_api-KeyCode-Colon 'gdio.unity_api.KeyCode.Colon')
  - [Comma](#F-gdio-unity_api-KeyCode-Comma 'gdio.unity_api.KeyCode.Comma')
  - [D](#F-gdio-unity_api-KeyCode-D 'gdio.unity_api.KeyCode.D')
  - [Delete](#F-gdio-unity_api-KeyCode-Delete 'gdio.unity_api.KeyCode.Delete')
  - [Dollar](#F-gdio-unity_api-KeyCode-Dollar 'gdio.unity_api.KeyCode.Dollar')
  - [DoubleQuote](#F-gdio-unity_api-KeyCode-DoubleQuote 'gdio.unity_api.KeyCode.DoubleQuote')
  - [DownArrow](#F-gdio-unity_api-KeyCode-DownArrow 'gdio.unity_api.KeyCode.DownArrow')
  - [E](#F-gdio-unity_api-KeyCode-E 'gdio.unity_api.KeyCode.E')
  - [End](#F-gdio-unity_api-KeyCode-End 'gdio.unity_api.KeyCode.End')
  - [Equals](#F-gdio-unity_api-KeyCode-Equals 'gdio.unity_api.KeyCode.Equals')
  - [Escape](#F-gdio-unity_api-KeyCode-Escape 'gdio.unity_api.KeyCode.Escape')
  - [Exclaim](#F-gdio-unity_api-KeyCode-Exclaim 'gdio.unity_api.KeyCode.Exclaim')
  - [F](#F-gdio-unity_api-KeyCode-F 'gdio.unity_api.KeyCode.F')
  - [F1](#F-gdio-unity_api-KeyCode-F1 'gdio.unity_api.KeyCode.F1')
  - [F10](#F-gdio-unity_api-KeyCode-F10 'gdio.unity_api.KeyCode.F10')
  - [F11](#F-gdio-unity_api-KeyCode-F11 'gdio.unity_api.KeyCode.F11')
  - [F12](#F-gdio-unity_api-KeyCode-F12 'gdio.unity_api.KeyCode.F12')
  - [F13](#F-gdio-unity_api-KeyCode-F13 'gdio.unity_api.KeyCode.F13')
  - [F14](#F-gdio-unity_api-KeyCode-F14 'gdio.unity_api.KeyCode.F14')
  - [F15](#F-gdio-unity_api-KeyCode-F15 'gdio.unity_api.KeyCode.F15')
  - [F2](#F-gdio-unity_api-KeyCode-F2 'gdio.unity_api.KeyCode.F2')
  - [F3](#F-gdio-unity_api-KeyCode-F3 'gdio.unity_api.KeyCode.F3')
  - [F4](#F-gdio-unity_api-KeyCode-F4 'gdio.unity_api.KeyCode.F4')
  - [F5](#F-gdio-unity_api-KeyCode-F5 'gdio.unity_api.KeyCode.F5')
  - [F6](#F-gdio-unity_api-KeyCode-F6 'gdio.unity_api.KeyCode.F6')
  - [F7](#F-gdio-unity_api-KeyCode-F7 'gdio.unity_api.KeyCode.F7')
  - [F8](#F-gdio-unity_api-KeyCode-F8 'gdio.unity_api.KeyCode.F8')
  - [F9](#F-gdio-unity_api-KeyCode-F9 'gdio.unity_api.KeyCode.F9')
  - [G](#F-gdio-unity_api-KeyCode-G 'gdio.unity_api.KeyCode.G')
  - [Greater](#F-gdio-unity_api-KeyCode-Greater 'gdio.unity_api.KeyCode.Greater')
  - [H](#F-gdio-unity_api-KeyCode-H 'gdio.unity_api.KeyCode.H')
  - [Hash](#F-gdio-unity_api-KeyCode-Hash 'gdio.unity_api.KeyCode.Hash')
  - [Help](#F-gdio-unity_api-KeyCode-Help 'gdio.unity_api.KeyCode.Help')
  - [Home](#F-gdio-unity_api-KeyCode-Home 'gdio.unity_api.KeyCode.Home')
  - [I](#F-gdio-unity_api-KeyCode-I 'gdio.unity_api.KeyCode.I')
  - [Insert](#F-gdio-unity_api-KeyCode-Insert 'gdio.unity_api.KeyCode.Insert')
  - [J](#F-gdio-unity_api-KeyCode-J 'gdio.unity_api.KeyCode.J')
  - [Joystick1Button0](#F-gdio-unity_api-KeyCode-Joystick1Button0 'gdio.unity_api.KeyCode.Joystick1Button0')
  - [Joystick1Button1](#F-gdio-unity_api-KeyCode-Joystick1Button1 'gdio.unity_api.KeyCode.Joystick1Button1')
  - [Joystick1Button10](#F-gdio-unity_api-KeyCode-Joystick1Button10 'gdio.unity_api.KeyCode.Joystick1Button10')
  - [Joystick1Button11](#F-gdio-unity_api-KeyCode-Joystick1Button11 'gdio.unity_api.KeyCode.Joystick1Button11')
  - [Joystick1Button12](#F-gdio-unity_api-KeyCode-Joystick1Button12 'gdio.unity_api.KeyCode.Joystick1Button12')
  - [Joystick1Button13](#F-gdio-unity_api-KeyCode-Joystick1Button13 'gdio.unity_api.KeyCode.Joystick1Button13')
  - [Joystick1Button14](#F-gdio-unity_api-KeyCode-Joystick1Button14 'gdio.unity_api.KeyCode.Joystick1Button14')
  - [Joystick1Button15](#F-gdio-unity_api-KeyCode-Joystick1Button15 'gdio.unity_api.KeyCode.Joystick1Button15')
  - [Joystick1Button16](#F-gdio-unity_api-KeyCode-Joystick1Button16 'gdio.unity_api.KeyCode.Joystick1Button16')
  - [Joystick1Button17](#F-gdio-unity_api-KeyCode-Joystick1Button17 'gdio.unity_api.KeyCode.Joystick1Button17')
  - [Joystick1Button18](#F-gdio-unity_api-KeyCode-Joystick1Button18 'gdio.unity_api.KeyCode.Joystick1Button18')
  - [Joystick1Button19](#F-gdio-unity_api-KeyCode-Joystick1Button19 'gdio.unity_api.KeyCode.Joystick1Button19')
  - [Joystick1Button2](#F-gdio-unity_api-KeyCode-Joystick1Button2 'gdio.unity_api.KeyCode.Joystick1Button2')
  - [Joystick1Button3](#F-gdio-unity_api-KeyCode-Joystick1Button3 'gdio.unity_api.KeyCode.Joystick1Button3')
  - [Joystick1Button4](#F-gdio-unity_api-KeyCode-Joystick1Button4 'gdio.unity_api.KeyCode.Joystick1Button4')
  - [Joystick1Button5](#F-gdio-unity_api-KeyCode-Joystick1Button5 'gdio.unity_api.KeyCode.Joystick1Button5')
  - [Joystick1Button6](#F-gdio-unity_api-KeyCode-Joystick1Button6 'gdio.unity_api.KeyCode.Joystick1Button6')
  - [Joystick1Button7](#F-gdio-unity_api-KeyCode-Joystick1Button7 'gdio.unity_api.KeyCode.Joystick1Button7')
  - [Joystick1Button8](#F-gdio-unity_api-KeyCode-Joystick1Button8 'gdio.unity_api.KeyCode.Joystick1Button8')
  - [Joystick1Button9](#F-gdio-unity_api-KeyCode-Joystick1Button9 'gdio.unity_api.KeyCode.Joystick1Button9')
  - [Joystick2Button0](#F-gdio-unity_api-KeyCode-Joystick2Button0 'gdio.unity_api.KeyCode.Joystick2Button0')
  - [Joystick2Button1](#F-gdio-unity_api-KeyCode-Joystick2Button1 'gdio.unity_api.KeyCode.Joystick2Button1')
  - [Joystick2Button10](#F-gdio-unity_api-KeyCode-Joystick2Button10 'gdio.unity_api.KeyCode.Joystick2Button10')
  - [Joystick2Button11](#F-gdio-unity_api-KeyCode-Joystick2Button11 'gdio.unity_api.KeyCode.Joystick2Button11')
  - [Joystick2Button12](#F-gdio-unity_api-KeyCode-Joystick2Button12 'gdio.unity_api.KeyCode.Joystick2Button12')
  - [Joystick2Button13](#F-gdio-unity_api-KeyCode-Joystick2Button13 'gdio.unity_api.KeyCode.Joystick2Button13')
  - [Joystick2Button14](#F-gdio-unity_api-KeyCode-Joystick2Button14 'gdio.unity_api.KeyCode.Joystick2Button14')
  - [Joystick2Button15](#F-gdio-unity_api-KeyCode-Joystick2Button15 'gdio.unity_api.KeyCode.Joystick2Button15')
  - [Joystick2Button16](#F-gdio-unity_api-KeyCode-Joystick2Button16 'gdio.unity_api.KeyCode.Joystick2Button16')
  - [Joystick2Button17](#F-gdio-unity_api-KeyCode-Joystick2Button17 'gdio.unity_api.KeyCode.Joystick2Button17')
  - [Joystick2Button18](#F-gdio-unity_api-KeyCode-Joystick2Button18 'gdio.unity_api.KeyCode.Joystick2Button18')
  - [Joystick2Button19](#F-gdio-unity_api-KeyCode-Joystick2Button19 'gdio.unity_api.KeyCode.Joystick2Button19')
  - [Joystick2Button2](#F-gdio-unity_api-KeyCode-Joystick2Button2 'gdio.unity_api.KeyCode.Joystick2Button2')
  - [Joystick2Button3](#F-gdio-unity_api-KeyCode-Joystick2Button3 'gdio.unity_api.KeyCode.Joystick2Button3')
  - [Joystick2Button4](#F-gdio-unity_api-KeyCode-Joystick2Button4 'gdio.unity_api.KeyCode.Joystick2Button4')
  - [Joystick2Button5](#F-gdio-unity_api-KeyCode-Joystick2Button5 'gdio.unity_api.KeyCode.Joystick2Button5')
  - [Joystick2Button6](#F-gdio-unity_api-KeyCode-Joystick2Button6 'gdio.unity_api.KeyCode.Joystick2Button6')
  - [Joystick2Button7](#F-gdio-unity_api-KeyCode-Joystick2Button7 'gdio.unity_api.KeyCode.Joystick2Button7')
  - [Joystick2Button8](#F-gdio-unity_api-KeyCode-Joystick2Button8 'gdio.unity_api.KeyCode.Joystick2Button8')
  - [Joystick2Button9](#F-gdio-unity_api-KeyCode-Joystick2Button9 'gdio.unity_api.KeyCode.Joystick2Button9')
  - [Joystick3Button0](#F-gdio-unity_api-KeyCode-Joystick3Button0 'gdio.unity_api.KeyCode.Joystick3Button0')
  - [Joystick3Button1](#F-gdio-unity_api-KeyCode-Joystick3Button1 'gdio.unity_api.KeyCode.Joystick3Button1')
  - [Joystick3Button10](#F-gdio-unity_api-KeyCode-Joystick3Button10 'gdio.unity_api.KeyCode.Joystick3Button10')
  - [Joystick3Button11](#F-gdio-unity_api-KeyCode-Joystick3Button11 'gdio.unity_api.KeyCode.Joystick3Button11')
  - [Joystick3Button12](#F-gdio-unity_api-KeyCode-Joystick3Button12 'gdio.unity_api.KeyCode.Joystick3Button12')
  - [Joystick3Button13](#F-gdio-unity_api-KeyCode-Joystick3Button13 'gdio.unity_api.KeyCode.Joystick3Button13')
  - [Joystick3Button14](#F-gdio-unity_api-KeyCode-Joystick3Button14 'gdio.unity_api.KeyCode.Joystick3Button14')
  - [Joystick3Button15](#F-gdio-unity_api-KeyCode-Joystick3Button15 'gdio.unity_api.KeyCode.Joystick3Button15')
  - [Joystick3Button16](#F-gdio-unity_api-KeyCode-Joystick3Button16 'gdio.unity_api.KeyCode.Joystick3Button16')
  - [Joystick3Button17](#F-gdio-unity_api-KeyCode-Joystick3Button17 'gdio.unity_api.KeyCode.Joystick3Button17')
  - [Joystick3Button18](#F-gdio-unity_api-KeyCode-Joystick3Button18 'gdio.unity_api.KeyCode.Joystick3Button18')
  - [Joystick3Button19](#F-gdio-unity_api-KeyCode-Joystick3Button19 'gdio.unity_api.KeyCode.Joystick3Button19')
  - [Joystick3Button2](#F-gdio-unity_api-KeyCode-Joystick3Button2 'gdio.unity_api.KeyCode.Joystick3Button2')
  - [Joystick3Button3](#F-gdio-unity_api-KeyCode-Joystick3Button3 'gdio.unity_api.KeyCode.Joystick3Button3')
  - [Joystick3Button4](#F-gdio-unity_api-KeyCode-Joystick3Button4 'gdio.unity_api.KeyCode.Joystick3Button4')
  - [Joystick3Button5](#F-gdio-unity_api-KeyCode-Joystick3Button5 'gdio.unity_api.KeyCode.Joystick3Button5')
  - [Joystick3Button6](#F-gdio-unity_api-KeyCode-Joystick3Button6 'gdio.unity_api.KeyCode.Joystick3Button6')
  - [Joystick3Button7](#F-gdio-unity_api-KeyCode-Joystick3Button7 'gdio.unity_api.KeyCode.Joystick3Button7')
  - [Joystick3Button8](#F-gdio-unity_api-KeyCode-Joystick3Button8 'gdio.unity_api.KeyCode.Joystick3Button8')
  - [Joystick3Button9](#F-gdio-unity_api-KeyCode-Joystick3Button9 'gdio.unity_api.KeyCode.Joystick3Button9')
  - [Joystick4Button0](#F-gdio-unity_api-KeyCode-Joystick4Button0 'gdio.unity_api.KeyCode.Joystick4Button0')
  - [Joystick4Button1](#F-gdio-unity_api-KeyCode-Joystick4Button1 'gdio.unity_api.KeyCode.Joystick4Button1')
  - [Joystick4Button10](#F-gdio-unity_api-KeyCode-Joystick4Button10 'gdio.unity_api.KeyCode.Joystick4Button10')
  - [Joystick4Button11](#F-gdio-unity_api-KeyCode-Joystick4Button11 'gdio.unity_api.KeyCode.Joystick4Button11')
  - [Joystick4Button12](#F-gdio-unity_api-KeyCode-Joystick4Button12 'gdio.unity_api.KeyCode.Joystick4Button12')
  - [Joystick4Button13](#F-gdio-unity_api-KeyCode-Joystick4Button13 'gdio.unity_api.KeyCode.Joystick4Button13')
  - [Joystick4Button14](#F-gdio-unity_api-KeyCode-Joystick4Button14 'gdio.unity_api.KeyCode.Joystick4Button14')
  - [Joystick4Button15](#F-gdio-unity_api-KeyCode-Joystick4Button15 'gdio.unity_api.KeyCode.Joystick4Button15')
  - [Joystick4Button16](#F-gdio-unity_api-KeyCode-Joystick4Button16 'gdio.unity_api.KeyCode.Joystick4Button16')
  - [Joystick4Button17](#F-gdio-unity_api-KeyCode-Joystick4Button17 'gdio.unity_api.KeyCode.Joystick4Button17')
  - [Joystick4Button18](#F-gdio-unity_api-KeyCode-Joystick4Button18 'gdio.unity_api.KeyCode.Joystick4Button18')
  - [Joystick4Button19](#F-gdio-unity_api-KeyCode-Joystick4Button19 'gdio.unity_api.KeyCode.Joystick4Button19')
  - [Joystick4Button2](#F-gdio-unity_api-KeyCode-Joystick4Button2 'gdio.unity_api.KeyCode.Joystick4Button2')
  - [Joystick4Button3](#F-gdio-unity_api-KeyCode-Joystick4Button3 'gdio.unity_api.KeyCode.Joystick4Button3')
  - [Joystick4Button4](#F-gdio-unity_api-KeyCode-Joystick4Button4 'gdio.unity_api.KeyCode.Joystick4Button4')
  - [Joystick4Button5](#F-gdio-unity_api-KeyCode-Joystick4Button5 'gdio.unity_api.KeyCode.Joystick4Button5')
  - [Joystick4Button6](#F-gdio-unity_api-KeyCode-Joystick4Button6 'gdio.unity_api.KeyCode.Joystick4Button6')
  - [Joystick4Button7](#F-gdio-unity_api-KeyCode-Joystick4Button7 'gdio.unity_api.KeyCode.Joystick4Button7')
  - [Joystick4Button8](#F-gdio-unity_api-KeyCode-Joystick4Button8 'gdio.unity_api.KeyCode.Joystick4Button8')
  - [Joystick4Button9](#F-gdio-unity_api-KeyCode-Joystick4Button9 'gdio.unity_api.KeyCode.Joystick4Button9')
  - [Joystick5Button0](#F-gdio-unity_api-KeyCode-Joystick5Button0 'gdio.unity_api.KeyCode.Joystick5Button0')
  - [Joystick5Button1](#F-gdio-unity_api-KeyCode-Joystick5Button1 'gdio.unity_api.KeyCode.Joystick5Button1')
  - [Joystick5Button10](#F-gdio-unity_api-KeyCode-Joystick5Button10 'gdio.unity_api.KeyCode.Joystick5Button10')
  - [Joystick5Button11](#F-gdio-unity_api-KeyCode-Joystick5Button11 'gdio.unity_api.KeyCode.Joystick5Button11')
  - [Joystick5Button12](#F-gdio-unity_api-KeyCode-Joystick5Button12 'gdio.unity_api.KeyCode.Joystick5Button12')
  - [Joystick5Button13](#F-gdio-unity_api-KeyCode-Joystick5Button13 'gdio.unity_api.KeyCode.Joystick5Button13')
  - [Joystick5Button14](#F-gdio-unity_api-KeyCode-Joystick5Button14 'gdio.unity_api.KeyCode.Joystick5Button14')
  - [Joystick5Button15](#F-gdio-unity_api-KeyCode-Joystick5Button15 'gdio.unity_api.KeyCode.Joystick5Button15')
  - [Joystick5Button16](#F-gdio-unity_api-KeyCode-Joystick5Button16 'gdio.unity_api.KeyCode.Joystick5Button16')
  - [Joystick5Button17](#F-gdio-unity_api-KeyCode-Joystick5Button17 'gdio.unity_api.KeyCode.Joystick5Button17')
  - [Joystick5Button18](#F-gdio-unity_api-KeyCode-Joystick5Button18 'gdio.unity_api.KeyCode.Joystick5Button18')
  - [Joystick5Button19](#F-gdio-unity_api-KeyCode-Joystick5Button19 'gdio.unity_api.KeyCode.Joystick5Button19')
  - [Joystick5Button2](#F-gdio-unity_api-KeyCode-Joystick5Button2 'gdio.unity_api.KeyCode.Joystick5Button2')
  - [Joystick5Button3](#F-gdio-unity_api-KeyCode-Joystick5Button3 'gdio.unity_api.KeyCode.Joystick5Button3')
  - [Joystick5Button4](#F-gdio-unity_api-KeyCode-Joystick5Button4 'gdio.unity_api.KeyCode.Joystick5Button4')
  - [Joystick5Button5](#F-gdio-unity_api-KeyCode-Joystick5Button5 'gdio.unity_api.KeyCode.Joystick5Button5')
  - [Joystick5Button6](#F-gdio-unity_api-KeyCode-Joystick5Button6 'gdio.unity_api.KeyCode.Joystick5Button6')
  - [Joystick5Button7](#F-gdio-unity_api-KeyCode-Joystick5Button7 'gdio.unity_api.KeyCode.Joystick5Button7')
  - [Joystick5Button8](#F-gdio-unity_api-KeyCode-Joystick5Button8 'gdio.unity_api.KeyCode.Joystick5Button8')
  - [Joystick5Button9](#F-gdio-unity_api-KeyCode-Joystick5Button9 'gdio.unity_api.KeyCode.Joystick5Button9')
  - [Joystick6Button0](#F-gdio-unity_api-KeyCode-Joystick6Button0 'gdio.unity_api.KeyCode.Joystick6Button0')
  - [Joystick6Button1](#F-gdio-unity_api-KeyCode-Joystick6Button1 'gdio.unity_api.KeyCode.Joystick6Button1')
  - [Joystick6Button10](#F-gdio-unity_api-KeyCode-Joystick6Button10 'gdio.unity_api.KeyCode.Joystick6Button10')
  - [Joystick6Button11](#F-gdio-unity_api-KeyCode-Joystick6Button11 'gdio.unity_api.KeyCode.Joystick6Button11')
  - [Joystick6Button12](#F-gdio-unity_api-KeyCode-Joystick6Button12 'gdio.unity_api.KeyCode.Joystick6Button12')
  - [Joystick6Button13](#F-gdio-unity_api-KeyCode-Joystick6Button13 'gdio.unity_api.KeyCode.Joystick6Button13')
  - [Joystick6Button14](#F-gdio-unity_api-KeyCode-Joystick6Button14 'gdio.unity_api.KeyCode.Joystick6Button14')
  - [Joystick6Button15](#F-gdio-unity_api-KeyCode-Joystick6Button15 'gdio.unity_api.KeyCode.Joystick6Button15')
  - [Joystick6Button16](#F-gdio-unity_api-KeyCode-Joystick6Button16 'gdio.unity_api.KeyCode.Joystick6Button16')
  - [Joystick6Button17](#F-gdio-unity_api-KeyCode-Joystick6Button17 'gdio.unity_api.KeyCode.Joystick6Button17')
  - [Joystick6Button18](#F-gdio-unity_api-KeyCode-Joystick6Button18 'gdio.unity_api.KeyCode.Joystick6Button18')
  - [Joystick6Button19](#F-gdio-unity_api-KeyCode-Joystick6Button19 'gdio.unity_api.KeyCode.Joystick6Button19')
  - [Joystick6Button2](#F-gdio-unity_api-KeyCode-Joystick6Button2 'gdio.unity_api.KeyCode.Joystick6Button2')
  - [Joystick6Button3](#F-gdio-unity_api-KeyCode-Joystick6Button3 'gdio.unity_api.KeyCode.Joystick6Button3')
  - [Joystick6Button4](#F-gdio-unity_api-KeyCode-Joystick6Button4 'gdio.unity_api.KeyCode.Joystick6Button4')
  - [Joystick6Button5](#F-gdio-unity_api-KeyCode-Joystick6Button5 'gdio.unity_api.KeyCode.Joystick6Button5')
  - [Joystick6Button6](#F-gdio-unity_api-KeyCode-Joystick6Button6 'gdio.unity_api.KeyCode.Joystick6Button6')
  - [Joystick6Button7](#F-gdio-unity_api-KeyCode-Joystick6Button7 'gdio.unity_api.KeyCode.Joystick6Button7')
  - [Joystick6Button8](#F-gdio-unity_api-KeyCode-Joystick6Button8 'gdio.unity_api.KeyCode.Joystick6Button8')
  - [Joystick6Button9](#F-gdio-unity_api-KeyCode-Joystick6Button9 'gdio.unity_api.KeyCode.Joystick6Button9')
  - [Joystick7Button0](#F-gdio-unity_api-KeyCode-Joystick7Button0 'gdio.unity_api.KeyCode.Joystick7Button0')
  - [Joystick7Button1](#F-gdio-unity_api-KeyCode-Joystick7Button1 'gdio.unity_api.KeyCode.Joystick7Button1')
  - [Joystick7Button10](#F-gdio-unity_api-KeyCode-Joystick7Button10 'gdio.unity_api.KeyCode.Joystick7Button10')
  - [Joystick7Button11](#F-gdio-unity_api-KeyCode-Joystick7Button11 'gdio.unity_api.KeyCode.Joystick7Button11')
  - [Joystick7Button12](#F-gdio-unity_api-KeyCode-Joystick7Button12 'gdio.unity_api.KeyCode.Joystick7Button12')
  - [Joystick7Button13](#F-gdio-unity_api-KeyCode-Joystick7Button13 'gdio.unity_api.KeyCode.Joystick7Button13')
  - [Joystick7Button14](#F-gdio-unity_api-KeyCode-Joystick7Button14 'gdio.unity_api.KeyCode.Joystick7Button14')
  - [Joystick7Button15](#F-gdio-unity_api-KeyCode-Joystick7Button15 'gdio.unity_api.KeyCode.Joystick7Button15')
  - [Joystick7Button16](#F-gdio-unity_api-KeyCode-Joystick7Button16 'gdio.unity_api.KeyCode.Joystick7Button16')
  - [Joystick7Button17](#F-gdio-unity_api-KeyCode-Joystick7Button17 'gdio.unity_api.KeyCode.Joystick7Button17')
  - [Joystick7Button18](#F-gdio-unity_api-KeyCode-Joystick7Button18 'gdio.unity_api.KeyCode.Joystick7Button18')
  - [Joystick7Button19](#F-gdio-unity_api-KeyCode-Joystick7Button19 'gdio.unity_api.KeyCode.Joystick7Button19')
  - [Joystick7Button2](#F-gdio-unity_api-KeyCode-Joystick7Button2 'gdio.unity_api.KeyCode.Joystick7Button2')
  - [Joystick7Button3](#F-gdio-unity_api-KeyCode-Joystick7Button3 'gdio.unity_api.KeyCode.Joystick7Button3')
  - [Joystick7Button4](#F-gdio-unity_api-KeyCode-Joystick7Button4 'gdio.unity_api.KeyCode.Joystick7Button4')
  - [Joystick7Button5](#F-gdio-unity_api-KeyCode-Joystick7Button5 'gdio.unity_api.KeyCode.Joystick7Button5')
  - [Joystick7Button6](#F-gdio-unity_api-KeyCode-Joystick7Button6 'gdio.unity_api.KeyCode.Joystick7Button6')
  - [Joystick7Button7](#F-gdio-unity_api-KeyCode-Joystick7Button7 'gdio.unity_api.KeyCode.Joystick7Button7')
  - [Joystick7Button8](#F-gdio-unity_api-KeyCode-Joystick7Button8 'gdio.unity_api.KeyCode.Joystick7Button8')
  - [Joystick7Button9](#F-gdio-unity_api-KeyCode-Joystick7Button9 'gdio.unity_api.KeyCode.Joystick7Button9')
  - [Joystick8Button0](#F-gdio-unity_api-KeyCode-Joystick8Button0 'gdio.unity_api.KeyCode.Joystick8Button0')
  - [Joystick8Button1](#F-gdio-unity_api-KeyCode-Joystick8Button1 'gdio.unity_api.KeyCode.Joystick8Button1')
  - [Joystick8Button10](#F-gdio-unity_api-KeyCode-Joystick8Button10 'gdio.unity_api.KeyCode.Joystick8Button10')
  - [Joystick8Button11](#F-gdio-unity_api-KeyCode-Joystick8Button11 'gdio.unity_api.KeyCode.Joystick8Button11')
  - [Joystick8Button12](#F-gdio-unity_api-KeyCode-Joystick8Button12 'gdio.unity_api.KeyCode.Joystick8Button12')
  - [Joystick8Button13](#F-gdio-unity_api-KeyCode-Joystick8Button13 'gdio.unity_api.KeyCode.Joystick8Button13')
  - [Joystick8Button14](#F-gdio-unity_api-KeyCode-Joystick8Button14 'gdio.unity_api.KeyCode.Joystick8Button14')
  - [Joystick8Button15](#F-gdio-unity_api-KeyCode-Joystick8Button15 'gdio.unity_api.KeyCode.Joystick8Button15')
  - [Joystick8Button16](#F-gdio-unity_api-KeyCode-Joystick8Button16 'gdio.unity_api.KeyCode.Joystick8Button16')
  - [Joystick8Button17](#F-gdio-unity_api-KeyCode-Joystick8Button17 'gdio.unity_api.KeyCode.Joystick8Button17')
  - [Joystick8Button18](#F-gdio-unity_api-KeyCode-Joystick8Button18 'gdio.unity_api.KeyCode.Joystick8Button18')
  - [Joystick8Button19](#F-gdio-unity_api-KeyCode-Joystick8Button19 'gdio.unity_api.KeyCode.Joystick8Button19')
  - [Joystick8Button2](#F-gdio-unity_api-KeyCode-Joystick8Button2 'gdio.unity_api.KeyCode.Joystick8Button2')
  - [Joystick8Button3](#F-gdio-unity_api-KeyCode-Joystick8Button3 'gdio.unity_api.KeyCode.Joystick8Button3')
  - [Joystick8Button4](#F-gdio-unity_api-KeyCode-Joystick8Button4 'gdio.unity_api.KeyCode.Joystick8Button4')
  - [Joystick8Button5](#F-gdio-unity_api-KeyCode-Joystick8Button5 'gdio.unity_api.KeyCode.Joystick8Button5')
  - [Joystick8Button6](#F-gdio-unity_api-KeyCode-Joystick8Button6 'gdio.unity_api.KeyCode.Joystick8Button6')
  - [Joystick8Button7](#F-gdio-unity_api-KeyCode-Joystick8Button7 'gdio.unity_api.KeyCode.Joystick8Button7')
  - [Joystick8Button8](#F-gdio-unity_api-KeyCode-Joystick8Button8 'gdio.unity_api.KeyCode.Joystick8Button8')
  - [Joystick8Button9](#F-gdio-unity_api-KeyCode-Joystick8Button9 'gdio.unity_api.KeyCode.Joystick8Button9')
  - [JoystickButton0](#F-gdio-unity_api-KeyCode-JoystickButton0 'gdio.unity_api.KeyCode.JoystickButton0')
  - [JoystickButton1](#F-gdio-unity_api-KeyCode-JoystickButton1 'gdio.unity_api.KeyCode.JoystickButton1')
  - [JoystickButton10](#F-gdio-unity_api-KeyCode-JoystickButton10 'gdio.unity_api.KeyCode.JoystickButton10')
  - [JoystickButton11](#F-gdio-unity_api-KeyCode-JoystickButton11 'gdio.unity_api.KeyCode.JoystickButton11')
  - [JoystickButton12](#F-gdio-unity_api-KeyCode-JoystickButton12 'gdio.unity_api.KeyCode.JoystickButton12')
  - [JoystickButton13](#F-gdio-unity_api-KeyCode-JoystickButton13 'gdio.unity_api.KeyCode.JoystickButton13')
  - [JoystickButton14](#F-gdio-unity_api-KeyCode-JoystickButton14 'gdio.unity_api.KeyCode.JoystickButton14')
  - [JoystickButton15](#F-gdio-unity_api-KeyCode-JoystickButton15 'gdio.unity_api.KeyCode.JoystickButton15')
  - [JoystickButton16](#F-gdio-unity_api-KeyCode-JoystickButton16 'gdio.unity_api.KeyCode.JoystickButton16')
  - [JoystickButton17](#F-gdio-unity_api-KeyCode-JoystickButton17 'gdio.unity_api.KeyCode.JoystickButton17')
  - [JoystickButton18](#F-gdio-unity_api-KeyCode-JoystickButton18 'gdio.unity_api.KeyCode.JoystickButton18')
  - [JoystickButton19](#F-gdio-unity_api-KeyCode-JoystickButton19 'gdio.unity_api.KeyCode.JoystickButton19')
  - [JoystickButton2](#F-gdio-unity_api-KeyCode-JoystickButton2 'gdio.unity_api.KeyCode.JoystickButton2')
  - [JoystickButton3](#F-gdio-unity_api-KeyCode-JoystickButton3 'gdio.unity_api.KeyCode.JoystickButton3')
  - [JoystickButton4](#F-gdio-unity_api-KeyCode-JoystickButton4 'gdio.unity_api.KeyCode.JoystickButton4')
  - [JoystickButton5](#F-gdio-unity_api-KeyCode-JoystickButton5 'gdio.unity_api.KeyCode.JoystickButton5')
  - [JoystickButton6](#F-gdio-unity_api-KeyCode-JoystickButton6 'gdio.unity_api.KeyCode.JoystickButton6')
  - [JoystickButton7](#F-gdio-unity_api-KeyCode-JoystickButton7 'gdio.unity_api.KeyCode.JoystickButton7')
  - [JoystickButton8](#F-gdio-unity_api-KeyCode-JoystickButton8 'gdio.unity_api.KeyCode.JoystickButton8')
  - [JoystickButton9](#F-gdio-unity_api-KeyCode-JoystickButton9 'gdio.unity_api.KeyCode.JoystickButton9')
  - [K](#F-gdio-unity_api-KeyCode-K 'gdio.unity_api.KeyCode.K')
  - [Keypad0](#F-gdio-unity_api-KeyCode-Keypad0 'gdio.unity_api.KeyCode.Keypad0')
  - [Keypad1](#F-gdio-unity_api-KeyCode-Keypad1 'gdio.unity_api.KeyCode.Keypad1')
  - [Keypad2](#F-gdio-unity_api-KeyCode-Keypad2 'gdio.unity_api.KeyCode.Keypad2')
  - [Keypad3](#F-gdio-unity_api-KeyCode-Keypad3 'gdio.unity_api.KeyCode.Keypad3')
  - [Keypad4](#F-gdio-unity_api-KeyCode-Keypad4 'gdio.unity_api.KeyCode.Keypad4')
  - [Keypad5](#F-gdio-unity_api-KeyCode-Keypad5 'gdio.unity_api.KeyCode.Keypad5')
  - [Keypad6](#F-gdio-unity_api-KeyCode-Keypad6 'gdio.unity_api.KeyCode.Keypad6')
  - [Keypad7](#F-gdio-unity_api-KeyCode-Keypad7 'gdio.unity_api.KeyCode.Keypad7')
  - [Keypad8](#F-gdio-unity_api-KeyCode-Keypad8 'gdio.unity_api.KeyCode.Keypad8')
  - [Keypad9](#F-gdio-unity_api-KeyCode-Keypad9 'gdio.unity_api.KeyCode.Keypad9')
  - [KeypadDivide](#F-gdio-unity_api-KeyCode-KeypadDivide 'gdio.unity_api.KeyCode.KeypadDivide')
  - [KeypadEnter](#F-gdio-unity_api-KeyCode-KeypadEnter 'gdio.unity_api.KeyCode.KeypadEnter')
  - [KeypadEquals](#F-gdio-unity_api-KeyCode-KeypadEquals 'gdio.unity_api.KeyCode.KeypadEquals')
  - [KeypadMinus](#F-gdio-unity_api-KeyCode-KeypadMinus 'gdio.unity_api.KeyCode.KeypadMinus')
  - [KeypadMultiply](#F-gdio-unity_api-KeyCode-KeypadMultiply 'gdio.unity_api.KeyCode.KeypadMultiply')
  - [KeypadPeriod](#F-gdio-unity_api-KeyCode-KeypadPeriod 'gdio.unity_api.KeyCode.KeypadPeriod')
  - [KeypadPlus](#F-gdio-unity_api-KeyCode-KeypadPlus 'gdio.unity_api.KeyCode.KeypadPlus')
  - [L](#F-gdio-unity_api-KeyCode-L 'gdio.unity_api.KeyCode.L')
  - [LeftAlt](#F-gdio-unity_api-KeyCode-LeftAlt 'gdio.unity_api.KeyCode.LeftAlt')
  - [LeftApple](#F-gdio-unity_api-KeyCode-LeftApple 'gdio.unity_api.KeyCode.LeftApple')
  - [LeftArrow](#F-gdio-unity_api-KeyCode-LeftArrow 'gdio.unity_api.KeyCode.LeftArrow')
  - [LeftBracket](#F-gdio-unity_api-KeyCode-LeftBracket 'gdio.unity_api.KeyCode.LeftBracket')
  - [LeftCommand](#F-gdio-unity_api-KeyCode-LeftCommand 'gdio.unity_api.KeyCode.LeftCommand')
  - [LeftControl](#F-gdio-unity_api-KeyCode-LeftControl 'gdio.unity_api.KeyCode.LeftControl')
  - [LeftParen](#F-gdio-unity_api-KeyCode-LeftParen 'gdio.unity_api.KeyCode.LeftParen')
  - [LeftShift](#F-gdio-unity_api-KeyCode-LeftShift 'gdio.unity_api.KeyCode.LeftShift')
  - [LeftWindows](#F-gdio-unity_api-KeyCode-LeftWindows 'gdio.unity_api.KeyCode.LeftWindows')
  - [Less](#F-gdio-unity_api-KeyCode-Less 'gdio.unity_api.KeyCode.Less')
  - [M](#F-gdio-unity_api-KeyCode-M 'gdio.unity_api.KeyCode.M')
  - [Menu](#F-gdio-unity_api-KeyCode-Menu 'gdio.unity_api.KeyCode.Menu')
  - [Minus](#F-gdio-unity_api-KeyCode-Minus 'gdio.unity_api.KeyCode.Minus')
  - [Mouse0](#F-gdio-unity_api-KeyCode-Mouse0 'gdio.unity_api.KeyCode.Mouse0')
  - [Mouse1](#F-gdio-unity_api-KeyCode-Mouse1 'gdio.unity_api.KeyCode.Mouse1')
  - [Mouse2](#F-gdio-unity_api-KeyCode-Mouse2 'gdio.unity_api.KeyCode.Mouse2')
  - [Mouse3](#F-gdio-unity_api-KeyCode-Mouse3 'gdio.unity_api.KeyCode.Mouse3')
  - [Mouse4](#F-gdio-unity_api-KeyCode-Mouse4 'gdio.unity_api.KeyCode.Mouse4')
  - [Mouse5](#F-gdio-unity_api-KeyCode-Mouse5 'gdio.unity_api.KeyCode.Mouse5')
  - [Mouse6](#F-gdio-unity_api-KeyCode-Mouse6 'gdio.unity_api.KeyCode.Mouse6')
  - [N](#F-gdio-unity_api-KeyCode-N 'gdio.unity_api.KeyCode.N')
  - [None](#F-gdio-unity_api-KeyCode-None 'gdio.unity_api.KeyCode.None')
  - [Numlock](#F-gdio-unity_api-KeyCode-Numlock 'gdio.unity_api.KeyCode.Numlock')
  - [O](#F-gdio-unity_api-KeyCode-O 'gdio.unity_api.KeyCode.O')
  - [P](#F-gdio-unity_api-KeyCode-P 'gdio.unity_api.KeyCode.P')
  - [PageDown](#F-gdio-unity_api-KeyCode-PageDown 'gdio.unity_api.KeyCode.PageDown')
  - [PageUp](#F-gdio-unity_api-KeyCode-PageUp 'gdio.unity_api.KeyCode.PageUp')
  - [Pause](#F-gdio-unity_api-KeyCode-Pause 'gdio.unity_api.KeyCode.Pause')
  - [Period](#F-gdio-unity_api-KeyCode-Period 'gdio.unity_api.KeyCode.Period')
  - [Plus](#F-gdio-unity_api-KeyCode-Plus 'gdio.unity_api.KeyCode.Plus')
  - [Print](#F-gdio-unity_api-KeyCode-Print 'gdio.unity_api.KeyCode.Print')
  - [Q](#F-gdio-unity_api-KeyCode-Q 'gdio.unity_api.KeyCode.Q')
  - [Question](#F-gdio-unity_api-KeyCode-Question 'gdio.unity_api.KeyCode.Question')
  - [Quote](#F-gdio-unity_api-KeyCode-Quote 'gdio.unity_api.KeyCode.Quote')
  - [R](#F-gdio-unity_api-KeyCode-R 'gdio.unity_api.KeyCode.R')
  - [Return](#F-gdio-unity_api-KeyCode-Return 'gdio.unity_api.KeyCode.Return')
  - [RightAlt](#F-gdio-unity_api-KeyCode-RightAlt 'gdio.unity_api.KeyCode.RightAlt')
  - [RightApple](#F-gdio-unity_api-KeyCode-RightApple 'gdio.unity_api.KeyCode.RightApple')
  - [RightArrow](#F-gdio-unity_api-KeyCode-RightArrow 'gdio.unity_api.KeyCode.RightArrow')
  - [RightBracket](#F-gdio-unity_api-KeyCode-RightBracket 'gdio.unity_api.KeyCode.RightBracket')
  - [RightCommand](#F-gdio-unity_api-KeyCode-RightCommand 'gdio.unity_api.KeyCode.RightCommand')
  - [RightControl](#F-gdio-unity_api-KeyCode-RightControl 'gdio.unity_api.KeyCode.RightControl')
  - [RightParen](#F-gdio-unity_api-KeyCode-RightParen 'gdio.unity_api.KeyCode.RightParen')
  - [RightShift](#F-gdio-unity_api-KeyCode-RightShift 'gdio.unity_api.KeyCode.RightShift')
  - [RightWindows](#F-gdio-unity_api-KeyCode-RightWindows 'gdio.unity_api.KeyCode.RightWindows')
  - [S](#F-gdio-unity_api-KeyCode-S 'gdio.unity_api.KeyCode.S')
  - [ScrollLock](#F-gdio-unity_api-KeyCode-ScrollLock 'gdio.unity_api.KeyCode.ScrollLock')
  - [Semicolon](#F-gdio-unity_api-KeyCode-Semicolon 'gdio.unity_api.KeyCode.Semicolon')
  - [Slash](#F-gdio-unity_api-KeyCode-Slash 'gdio.unity_api.KeyCode.Slash')
  - [Space](#F-gdio-unity_api-KeyCode-Space 'gdio.unity_api.KeyCode.Space')
  - [SysReq](#F-gdio-unity_api-KeyCode-SysReq 'gdio.unity_api.KeyCode.SysReq')
  - [T](#F-gdio-unity_api-KeyCode-T 'gdio.unity_api.KeyCode.T')
  - [Tab](#F-gdio-unity_api-KeyCode-Tab 'gdio.unity_api.KeyCode.Tab')
  - [U](#F-gdio-unity_api-KeyCode-U 'gdio.unity_api.KeyCode.U')
  - [Underscore](#F-gdio-unity_api-KeyCode-Underscore 'gdio.unity_api.KeyCode.Underscore')
  - [UpArrow](#F-gdio-unity_api-KeyCode-UpArrow 'gdio.unity_api.KeyCode.UpArrow')
  - [V](#F-gdio-unity_api-KeyCode-V 'gdio.unity_api.KeyCode.V')
  - [W](#F-gdio-unity_api-KeyCode-W 'gdio.unity_api.KeyCode.W')
  - [X](#F-gdio-unity_api-KeyCode-X 'gdio.unity_api.KeyCode.X')
  - [Y](#F-gdio-unity_api-KeyCode-Y 'gdio.unity_api.KeyCode.Y')
  - [Z](#F-gdio-unity_api-KeyCode-Z 'gdio.unity_api.KeyCode.Z')
- [ScreenCapture](#T-gdio-unity_api-utilities-ScreenCapture 'gdio.unity_api.utilities.ScreenCapture')
  - [CaptureScreen()](#M-gdio-unity_api-utilities-ScreenCapture-CaptureScreen 'gdio.unity_api.utilities.ScreenCapture.CaptureScreen')
  - [CaptureScreenToFile(filename,format)](#M-gdio-unity_api-utilities-ScreenCapture-CaptureScreenToFile-System-String,System-Drawing-Imaging-ImageFormat- 'gdio.unity_api.utilities.ScreenCapture.CaptureScreenToFile(System.String,System.Drawing.Imaging.ImageFormat)')
  - [CaptureWindow(handle)](#M-gdio-unity_api-utilities-ScreenCapture-CaptureWindow-System-IntPtr- 'gdio.unity_api.utilities.ScreenCapture.CaptureWindow(System.IntPtr)')
  - [CaptureWindowToFile(handle,filename,format)](#M-gdio-unity_api-utilities-ScreenCapture-CaptureWindowToFile-System-IntPtr,System-String,System-Drawing-Imaging-ImageFormat- 'gdio.unity_api.utilities.ScreenCapture.CaptureWindowToFile(System.IntPtr,System.String,System.Drawing.Imaging.ImageFormat)')
- [User32](#T-gdio-unity_api-utilities-ScreenCapture-User32 'gdio.unity_api.utilities.ScreenCapture.User32')

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

The default AUTOPLAY port to use when searching for games running.  This port is configured in the Unity preferences.

<a name='F-gdio-unity_api-v2-ApiClient-AUTOPLAY_ENABLED'></a>
### AUTOPLAY_ENABLED `constants`

##### Summary

NOT IN USE.

<a name='F-gdio-unity_api-v2-ApiClient-AUTOPLAY_RECEIVE_PORT'></a>
### AUTOPLAY_RECEIVE_PORT `constants`

##### Summary

The port to listen for responses from the AutoPlay plugin running in Unity.  Do to loopback limitations, this port must be different than the [AUTOPLAY_DEFAULT_PORT](#F-gdio-unity_api-v2-ApiClient-AUTOPLAY_DEFAULT_PORT 'gdio.unity_api.v2.ApiClient.AUTOPLAY_DEFAULT_PORT')

<a name='F-gdio-unity_api-v2-ApiClient-THROW_EXCEPTIONS'></a>
### THROW_EXCEPTIONS `constants`

##### Summary

If TRUE, the API will throw exceptions instead of logging errors and where applicable returning false/NULL.  The default is FALSE.

<a name='M-gdio-unity_api-v2-ApiClient-CallMethod-System-String,System-String,System-Object[],System-Int32-'></a>
### CallMethod(hierarchyPath,methodName,arguments,timeout) `method`

##### Summary

Use this function to execute a [Void](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Void 'System.Void') method on an object.

##### Returns

Returns a boolean based on the successful execution of the return type void, method.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath for the object, i.e. Script component, to call a method for. |
| methodName | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The name of the method to call |
| arguments | [System.Object[]](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Object[] 'System.Object[]') | An array of objects to pass as arguments to the method |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of seconds to wait for a response that the CaptureScreenshot request was processed. |

<a name='M-gdio-unity_api-v2-ApiClient-CallMethod``1-System-String,System-String,System-Object[],System-Int32-'></a>
### CallMethod\`\`1(hierarchyPath,methodName,arguments,timeout) `method`

##### Summary

Use this function to execute a method on an object.

##### Returns

Returns a deserialized object of type T. If T and the type of the returned object don't match, and exception will be thrown.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath for the object, i.e. Script component, to call a method for. |
| methodName | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The name of the method to call |
| arguments | [System.Object[]](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Object[] 'System.Object[]') | An array of objects to pass as arguments to the method |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of seconds to wait for a response that the CaptureScreenshot request was processed. |

<a name='M-gdio-unity_api-v2-ApiClient-CaptureScreenshot-System-String,System-Boolean,System-Boolean,System-Int32-'></a>
### CaptureScreenshot(filename,storeInGameFolder,overwriteExisting,timeout) `method`

##### Summary

Use this function to capture a screenshot of the Game running.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| filename | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The filename, and path, of the screen capture. |
| storeInGameFolder | [System.Boolean](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Boolean 'System.Boolean') | If true, this won't transfer the screen capture back to the client and instead will save it on the device where the game is running. |
| overwriteExisting | [System.Boolean](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Boolean 'System.Boolean') | If true, the operation will overwrite the file if it already exists. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of seconds to wait for a response that the CaptureScreenshot request was processed. |

<a name='M-gdio-unity_api-v2-ApiClient-Click-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,System-Int32-'></a>
### Click(buttonId,position,clickFrameCount,timeout) `method`

##### Summary

Use this function to interact perform in game mouse-clicks.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| position | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The [Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') position to performa a mouse click. |
| clickFrameCount | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to click the specific object. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of seconds to wait for a response that the Click request was processed.  Input requests process asynchornously, so a response does NOT imply the input operation has completed. |

<a name='M-gdio-unity_api-v2-ApiClient-Click-gdio-common-objects-MouseButtons,System-Single,System-Single,System-UInt64,System-Int32-'></a>
### Click(buttonId,x,y,clickFrameCount,timeout) `method`

##### Summary

Use this function to interact perform in game mouse-clicks.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| x | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The X coordinate of the game to click in Screen space. |
| y | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The Y coordinate of the game to click in Screen space. |
| clickFrameCount | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to click the specific object. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of seconds to wait for a response that the Click request was processed.  Input requests process asynchornously, so a response does NOT imply the input operation has completed. |

<a name='M-gdio-unity_api-v2-ApiClient-ClickEx-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32-'></a>
### ClickEx(buttonId,position,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout) `method`

##### Summary

Use this function to interact perform in game mouse-clicks in combination with key press operations.  The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| position | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The [Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') position to performa a mouse click. |
| clickFrameCount | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to click the specific object. |
| keys | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') keys to press during the click operation. |
| keysNumberOfFrames | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to press the keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| modifiers | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | Ann array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') modifier keys to press during the click operation. |
| modifiersNumberOfFrames | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to press the modifier keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| delayAfterModifiersMsec | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | Total time in milliseconds to wait after pressing modifier keys, before clicking the object.  This is needed when a delay is required to register the modifier keys have been pressed in the game.  If this delay is longer than the frame
count for all the key presses and click operation that the behavior of the result may not be what the user intends. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of seconds to wait for a response that the ClickEx request was processed.  Input requests process asynchornously, so a response does NOT imply the input operation has completed. |

<a name='M-gdio-unity_api-v2-ApiClient-ClickEx-gdio-common-objects-MouseButtons,System-Single,System-Single,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32-'></a>
### ClickEx(buttonId,x,y,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout) `method`

##### Summary

Use this function to interact perform in game mouse-clicks in combination with key press operations.  The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| x | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The X coordinate of the game to click in Screen space. |
| y | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The Y coordinate of the game to click in Screen space. |
| clickFrameCount | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to click the specific object. |
| keys | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') keys to press during the click operation. |
| keysNumberOfFrames | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to press the keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| modifiers | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | Ann array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') modifier keys to press during the click operation. |
| modifiersNumberOfFrames | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to press the modifier keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| delayAfterModifiersMsec | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | Total time in milliseconds to wait after pressing modifier keys, before clicking the object.  This is needed when a delay is required to register the modifier keys have been pressed in the game.  If this delay is longer than the frame
count for all the key presses and click operation that the behavior of the result may not be what the user intends. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of seconds to wait for a response that the ClickEx request was processed.  Input requests process asynchornously, so a response does NOT imply the input operation has completed. |

<a name='M-gdio-unity_api-v2-ApiClient-ClickObject-gdio-common-objects-MouseButtons,System-String,System-UInt64,System-Int32-'></a>
### ClickObject(buttonId,hierarchyPath,frameCount,timeout) `method`

##### Summary

Use this function to interact with an object in game using mouse-clicks.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| hierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath for the GameObject to perform a click on. |
| frameCount | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to click the specific object. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of frames to hold the keys down before clicking. Total press frame count is keyFrames + frames.  Input requests process asynchornously, so a response does NOT imply the input operation has completed. |

<a name='M-gdio-unity_api-v2-ApiClient-ClickObjectEx-gdio-common-objects-MouseButtons,System-String,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32-'></a>
### ClickObjectEx(buttonId,hierarchyPath,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout) `method`

##### Summary

Use this function to interact with an object in game using mouse-clicks in combination with key press operations.  The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| hierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath for the GameObject to perform a click on. |
| clickFrameCount | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to click the specific object. |
| keys | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') keys to press during the click operation. |
| keysNumberOfFrames | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to press the keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| modifiers | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | Ann array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') modifier keys to press during the click operation. |
| modifiersNumberOfFrames | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to press the modifier keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| delayAfterModifiersMsec | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | Total time in milliseconds to wait after pressing modifier keys, before clicking the object.  This is needed when a delay is required to register the modifier keys have been pressed in the game.  If this delay is longer than the frame
count for all the key presses and click operation that the behavior of the result may not be what the user intends. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of seconds to wait for a response that the ClickObjectEx request was processed.  Input requests process asynchornously, so a response does NOT imply the input operation has completed. |

<a name='M-gdio-unity_api-v2-ApiClient-Connect-System-String,System-Int32,System-Boolean,System-Int32,System-Boolean-'></a>
### Connect(hostname,port,autoplay,timeout,autoPortResolution) `method`

##### Summary

Use this function to connect to a Unity game with GameDriver Agent configured and active.  This function can connect to the UnityEditor or a Standalone deployment of a game.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hostname | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The hostname of the machine running the game. |
| port | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The configured port that the GameDriver agent is configured to use. |
| autoplay | [System.Boolean](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Boolean 'System.Boolean') | Autoplay allows you to automatically start a game in the UnityEditor without manual intervention. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The amount of time in seconds to wait for connectivity to establish with the game. |
| autoPortResolution | [System.Boolean](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Boolean 'System.Boolean') | Auto port resolution allows for the UnityEditor or Standalone game to report what port it is using for the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-Connect-System-String,System-String,System-Int32,System-Boolean,System-Int32,System-Boolean-'></a>
### Connect(hostname,regex_MatchGamePath,port,autoplay,timeout,autoPortResolution) `method`

##### Summary

Use this function to connect to a Unity game with GameDriver Agent configured and active.  This function can connect to the UnityEditor or a Standalone deployment of a game.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hostname | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The hostname of the machine running the game. |
| regex_MatchGamePath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | This parameter is a regular expression that will attempt to match a specfic game via its Application.DataPath if you have multiple games running. |
| port | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The configured port that the GameDriver agent is configured to use. |
| autoplay | [System.Boolean](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Boolean 'System.Boolean') | Autoplay allows you to automatically start a game in the UnityEditor without manual intervention. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The amount of time in seconds to wait for connectivity to establish with the game. |
| autoPortResolution | [System.Boolean](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Boolean 'System.Boolean') | Auto port resolution allows for the UnityEditor or Standalone game to report what port it is using for the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-DisableHooks-gdio-unity_api-v2-HookingObject,System-Int32-'></a>
### DisableHooks(hookObject,timeout) `method`

##### Summary

Diable input hooks in the game.

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hookObject | [gdio.unity_api.v2.HookingObject](#T-gdio-unity_api-v2-HookingObject 'gdio.unity_api.v2.HookingObject') | The type of input hook to disable. See [HookingObject](#T-gdio-unity_api-v2-HookingObject 'gdio.unity_api.v2.HookingObject') |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-DisbleObjectCaching-System-Int32-'></a>
### DisbleObjectCaching(timeout) `method`

##### Summary

Diable the use of object caching when doing HierarchyPath object resolution.

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-Disconnect'></a>
### Disconnect() `method`

##### Summary

Use this function to disconnect the API client from the Game.

##### Parameters

This method has no parameters.

<a name='M-gdio-unity_api-v2-ApiClient-DoubleClick-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,System-Int32-'></a>
### DoubleClick(buttonId,position,clickFrameCount,timeout) `method`

##### Summary

Use this function to interact perform in game mouse double clicks.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the double click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| position | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The 2d vector to double click in Screen space. |
| clickFrameCount | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to double click the specific object. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of seconds to wait for a response that the Click request was processed.  Input requests process asynchornously, so a response does NOT imply the input operation has completed. |

<a name='M-gdio-unity_api-v2-ApiClient-DoubleClick-gdio-common-objects-MouseButtons,System-Single,System-Single,System-UInt64,System-Int32-'></a>
### DoubleClick(buttonId,x,y,clickFrameCount,timeout) `method`

##### Summary

Use this function to interact perform in game mouse double clicks.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the double click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| x | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The X coordinate of the game to double click in Screen space. |
| y | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The Y coordinate of the game to double click in Screen space. |
| clickFrameCount | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to click the specific object. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of seconds to wait for a response that the Click request was processed.  Input requests process asynchornously, so a response does NOT imply the input operation has completed. |

<a name='M-gdio-unity_api-v2-ApiClient-DoubleClickEx-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32-'></a>
### DoubleClickEx(buttonId,position,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout) `method`

##### Summary

Use this function to interact perform in game mouse double clicks in combination with key press operations.  The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| position | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The 2d vector of where to double click in Screen space. |
| clickFrameCount | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to click the specific object. |
| keys | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') keys to press during the click operation. |
| keysNumberOfFrames | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to press the keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| modifiers | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | Ann array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') modifier keys to press during the click operation. |
| modifiersNumberOfFrames | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to press the modifier keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| delayAfterModifiersMsec | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | Total time in milliseconds to wait after pressing modifier keys, before clicking the object.  This is needed when a delay is required to register the modifier keys have been pressed in the game.  If this delay is longer than the frame
count for all the key presses and click operation that the behavior of the result may not be what the user intends. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of seconds to wait for a response that the ClickEx request was processed.  Input requests process asynchornously, so a response does NOT imply the input operation has completed. |

<a name='M-gdio-unity_api-v2-ApiClient-DoubleClickEx-gdio-common-objects-MouseButtons,System-Single,System-Single,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32-'></a>
### DoubleClickEx(buttonId,x,y,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout) `method`

##### Summary

Use this function to interact perform in game mouse double clicks in combination with key press operations.  The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| x | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The X coordinate of the game to double click in Screen space. |
| y | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The Y coordinate of the game to double click in Screen space. |
| clickFrameCount | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to click the specific object. |
| keys | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') keys to press during the click operation. |
| keysNumberOfFrames | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to press the keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| modifiers | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | Ann array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') modifier keys to press during the click operation. |
| modifiersNumberOfFrames | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to press the modifier keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| delayAfterModifiersMsec | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | Total time in milliseconds to wait after pressing modifier keys, before clicking the object.  This is needed when a delay is required to register the modifier keys have been pressed in the game.  If this delay is longer than the frame
count for all the key presses and click operation that the behavior of the result may not be what the user intends. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of seconds to wait for a response that the ClickEx request was processed.  Input requests process asynchornously, so a response does NOT imply the input operation has completed. |

<a name='M-gdio-unity_api-v2-ApiClient-DoubleClickObject-gdio-common-objects-MouseButtons,System-String,System-UInt64,System-Int32-'></a>
### DoubleClickObject(buttonId,hierarchyPath,frameCount,timeout) `method`

##### Summary

Use this function to interact with an object in game using a mouse double click.

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the double click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| hierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath for the GameObject to perform a double click on. |
| frameCount | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to double click the specific object. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of frames to hold the keys down before clicking. Total press frame count is keyFrames + frames.  Input requests process asynchornously, so a response does NOT imply the input operation has completed. |

<a name='M-gdio-unity_api-v2-ApiClient-DoubleClickObjectEx-gdio-common-objects-MouseButtons,System-String,System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,gdio-unity_api-KeyCode[],System-UInt64,System-Int32,System-Int32-'></a>
### DoubleClickObjectEx(buttonId,hierarchyPath,clickFrameCount,keys,keysNumberOfFrames,modifiers,modifiersNumberOfFrames,delayAfterModifiersMsec,timeout) `method`

##### Summary

Use this function to interact with an object in game using amouse double click, in combination with key press operations.  The total frame count execution of this operation is clickFrameCount + keysNumberOfFrames + modifiersNumberOfFrames

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| buttonId | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button to use for the double click operation.  See [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'). |
| hierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath for the GameObject to perform a double click on. |
| clickFrameCount | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to click the specific object. |
| keys | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') keys to press during the click operation. |
| keysNumberOfFrames | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to press the keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| modifiers | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | Ann array of [KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') modifier keys to press during the click operation. |
| modifiersNumberOfFrames | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to press the modifier keys parameter down.  This parameter is not additive to the total count and is automatically accumulated by the function call. |
| delayAfterModifiersMsec | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | Total time in milliseconds to wait after pressing modifier keys, before clicking the object.  This is needed when a delay is required to register the modifier keys have been pressed in the game.  If this delay is longer than the frame
count for all the key presses and click operation that the behavior of the result may not be what the user intends. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of seconds to wait for a response that the ClickObjectEx request was processed.  Input requests process asynchornously, so a response does NOT imply the input operation has completed. |

<a name='M-gdio-unity_api-v2-ApiClient-EnableHooks-gdio-unity_api-v2-HookingObject,System-Int32-'></a>
### EnableHooks(hookObject,timeout) `method`

##### Summary

Enable input hooks in the game.

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hookObject | [gdio.unity_api.v2.HookingObject](#T-gdio-unity_api-v2-HookingObject 'gdio.unity_api.v2.HookingObject') | The type of input hook to enable. See [HookingObject](#T-gdio-unity_api-v2-HookingObject 'gdio.unity_api.v2.HookingObject') |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-EnableObjectCaching-System-Int32-'></a>
### EnableObjectCaching(timeout) `method`

##### Summary

Enable the use of object caching when doing HierarchyPath object resolution.  Object caching is per HierarchyPath stored in a [IDictionary](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Collections.IDictionary 'System.Collections.IDictionary'). If a matching HierarchyPath is already in the dictionary, then the stored object is returned.
The only way to update a cached reference is for the reference to be garbage collected or flush the cache with [FlushObjectLookupCache](#M-gdio-unity_api-v2-ApiClient-FlushObjectLookupCache-System-Int32- 'gdio.unity_api.v2.ApiClient.FlushObjectLookupCache(System.Int32)').

##### Returns

TRUE if the GameDriver agent successfully processed the request.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-FlushObjectLookupCache-System-Int32-'></a>
### FlushObjectLookupCache(timeout) `method`

##### Summary

If object caching is enabled, this method will request that the agent flush the cache being held for all object lookups.

##### Returns



##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') |  |

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

<a name='M-gdio-unity_api-v2-ApiClient-GetObjectDistance-System-String,System-String,System-Int32-'></a>
### GetObjectDistance(objectA_HierarchyPath,objectB_HierarchyPath,timeout) `method`

##### Summary

This method returns the distance of two objects.

##### Returns

Returns the disance between the two objects as a float.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| objectA_HierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath for the first GameObject. |
| objectB_HierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchYpath for the second GameObject. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-GetObjectFieldValue``1-System-String,System-Int32-'></a>
### GetObjectFieldValue\`\`1(hierarchyPath,timeout) `method`

##### Summary

This method returns the field or property value of an object.

##### Returns

Returns an object of type T for the value or throws an [Exception](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Exception 'System.Exception') on error.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath of the object and field/property to be inspected. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

##### Generic Types

| Name | Description |
| ---- | ----------- |
| T | The [Type](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Type 'System.Type') of the field or property to be inspected. |

<a name='M-gdio-unity_api-v2-ApiClient-GetObjectList-System-Int32-'></a>
### GetObjectList(timeout) `method`

##### Summary

This method returns of a list of all GameObjects as returned by [](#!-UnityEngine-GameObject-FindObjectsOfType-Type- 'UnityEngine.GameObject.FindObjectsOfType(Type)'), where Type is UnityEngine.GameObject./>

##### Returns

This method returns a [IList](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Collections.IList 'System.Collections.IList') of [LiteGameObject](#T-gdio-common-objects-LiteGameObject 'gdio.common.objects.LiteGameObject').  LiteGameObject is a slimmer representation of UnityEngine.GameObject

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-GetObjectPosition-System-String,gdio-common-objects-CoordinateConversion,System-String,System-Int32-'></a>
### GetObjectPosition(objectHierarchyPath,cordSpace,cameraHierarchyPath,timeout) `method`

##### Summary



##### Returns



##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| objectHierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath to the object to return the poisition of. |
| cordSpace | [gdio.common.objects.CoordinateConversion](#T-gdio-common-objects-CoordinateConversion 'gdio.common.objects.CoordinateConversion') | The coorindate space conversion to perform on the position before returning it. |
| cameraHierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchPath to the Camera GameObject to use.  The default is string.Empty, which uses Camera.main/> |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-GetSceneName-System-Int32-'></a>
### GetSceneName(timeout) `method`

##### Summary

Return the name of the current active scene.

##### Returns

The name of the scene as a string.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

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



##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| keys | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of keys([KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode')) to press. |
| numberOfFrames | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to press and hold the keys for. |
| modifiers | [gdio.unity_api.KeyCode[]](#T-gdio-unity_api-KeyCode[] 'gdio.unity_api.KeyCode[]') | An array of modifiers()[KeyCode](#T-gdio-unity_api-KeyCode 'gdio.unity_api.KeyCode') to press. |
| modifierNumberOfFrames | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to hold the modifiers down for, before pressing the keys. |
| delayAfterModifiersMsec | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The delay to wait between holding the modifies and pressing the keys. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-LoadScene-System-String,System-Int32-'></a>
### LoadScene(sceneName,timeout) `method`

##### Summary

This method loads the scene, defined by the scene name passed as an argument.

##### Returns

Returns TRUE if the request was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| sceneName | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The name of the scene to load |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-MouseDrag-gdio-common-objects-MouseButtons,gdio-common-objects-Vector2,System-UInt64,gdio-common-objects-Vector2,System-Boolean,System-Int32-'></a>
### MouseDrag(button,destination,frameCount,origin,waitForEmptyInput,timeout) `method`

##### Summary

Perform a mouse drag operation.

##### Returns

Returns TRUE if the requests was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| button | [gdio.common.objects.MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons') | The mouse button, [MouseButtons](#T-gdio-common-objects-MouseButtons 'gdio.common.objects.MouseButtons'), to perform the drag operation with. |
| destination | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The desintation vector to drag the mouse to. |
| frameCount | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames taken to complete the drag operation. |
| origin | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The origin to start the drag operation.  If null, the mouse drag operation will begin at the current position of Input.mousePosition. |
| waitForEmptyInput | [System.Boolean](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Boolean 'System.Boolean') | Wait for the empty input event to be returned from the agent before returning from the method call. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. If waitForEmptyInput is set to TRUE, then the method call will wait the timeout alotment to recieve the event. |

<a name='M-gdio-unity_api-v2-ApiClient-MouseMoveToObject-System-String,System-UInt64,System-Boolean,System-Boolean,System-Int32-'></a>
### MouseMoveToObject(objectHierarchyPath,frameCount,waitForObject,waitForEmptyInput,timeout) `method`

##### Summary

Move the mouse to the center of a specific object, identified by the HierarchyPath.

##### Returns

Returns TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| objectHierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath to move the mouse pointer to. |
| frameCount | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to compelte the mouse move over. |
| waitForObject | [System.Boolean](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Boolean 'System.Boolean') | If TRUE, wait for the object to exist so that mouse move can complete successfully. |
| waitForEmptyInput | [System.Boolean](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Boolean 'System.Boolean') | Wait for the empty input event to be returned from the GameDriver agent, before returning from the method. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent.  If waitForEmptyInput is TRUE, then the method call will wait the timeout alotment to recieve the event. |

<a name='M-gdio-unity_api-v2-ApiClient-MoveMouseToPoint-gdio-common-objects-Vector2,System-UInt64,gdio-common-objects-Vector2,System-Boolean,System-Int32-'></a>
### MoveMouseToPoint(desintation,frameCount,origin,waitForEmptyInput,timeout) `method`

##### Summary

Move the mouse to the destination vector.

##### Returns

Returns TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| desintation | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | Destination vector to move the mouse to. |
| frameCount | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to complete the operaiton over. |
| origin | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The origin to start the mouse move operation.  If null, the mouse move operation will begin at the current position of Input.mousePosition. |
| waitForEmptyInput | [System.Boolean](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Boolean 'System.Boolean') | Wait for the empty input event to be returned from the GameDriver agent, before returning from the method. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent.  If waitForEmptyInput is TRUE, then the method call will wait the timeout alotment to recieve the event. |

<a name='M-gdio-unity_api-v2-ApiClient-NavAgentMoveToPoint-System-String,gdio-common-objects-Vector3,System-Boolean,System-Int32-'></a>
### NavAgentMoveToPoint(navAgentHierarchyPath,desintation,waitForMoveToComplete,timeout) `method`

##### Summary

Move a NavAgent to a a destination point.

##### Returns

Returns TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| navAgentHierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath to the NavAgent. |
| desintation | [gdio.common.objects.Vector3](#T-gdio-common-objects-Vector3 'gdio.common.objects.Vector3') | The desintation vector to move to. |
| waitForMoveToComplete | [System.Boolean](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Boolean 'System.Boolean') | Wait for the NavAgent move-to operation to complete before the method returns. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-Raycast-gdio-common-objects-Vector3,System-String,System-Int32-'></a>
### Raycast(raycastPoint,cameraHierarchyPath,timeout) `method`

##### Summary

Perform a Raycast to a point.

##### Returns

Returns an array of [RaycastResult](#T-gdio-common-objects-RaycastResult 'gdio.common.objects.RaycastResult').

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| raycastPoint | [gdio.common.objects.Vector3](#T-gdio-common-objects-Vector3 'gdio.common.objects.Vector3') | The vector to perform a raycast to. |
| cameraHierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath for the  UnityEngine.Camera to use as a Raycast reference.  If the Camera is string.Empty, the Camera.main is used |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-RotateObject-System-String,gdio-common-objects-Quaternion,System-Boolean,System-Int32-'></a>
### RotateObject(hierarchyPath,quaternion,waitForObject,timeout) `method`

##### Summary

Rotate an object defined by the HierarchyPath and rotated by a Quaternion.

##### Returns

Returns TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath for the object to rotate. |
| quaternion | [gdio.common.objects.Quaternion](#T-gdio-common-objects-Quaternion 'gdio.common.objects.Quaternion') | The quaternion value to manipulate the object. |
| waitForObject | [System.Boolean](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Boolean 'System.Boolean') | Wait for th object to exist if it doesn't. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-RotateObject-System-String,gdio-common-objects-Vector3,gdio-common-objects-Space,System-Boolean,System-Int32-'></a>
### RotateObject(hierarchyPath,eulers,relativeTo,waitForObject,timeout) `method`

##### Summary

Rotate an object defined by the HierarchyPath and rotated by Eulers.

##### Returns

Returns TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath for the object to rotate. |
| eulers | [gdio.common.objects.Vector3](#T-gdio-common-objects-Vector3 'gdio.common.objects.Vector3') | The Eulers vector to manipulate the object. |
| relativeTo | [gdio.common.objects.Space](#T-gdio-common-objects-Space 'gdio.common.objects.Space') | The [Space](#T-gdio-common-objects-Space 'gdio.common.objects.Space') to perform the rotation relative to. |
| waitForObject | [System.Boolean](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Boolean 'System.Boolean') | Wait for th object to exist if it doesn't. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-RotateObject-System-String,System-Single,System-Single,System-Single,gdio-common-objects-Space,System-Boolean,System-Int32-'></a>
### RotateObject(hierarchyPath,xAngle,yAngle,zAngle,relativeTo,waitForObject,timeout) `method`

##### Summary

Rottate an objected defined by the HierarchyPath and rotated by the x, y, and z angles relative to the Space

##### Returns

Returns TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath for the object to rotate. |
| xAngle | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The X angle value to rotate. |
| yAngle | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The Y angle value to rotate. |
| zAngle | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The Z angle value to rotate. |
| relativeTo | [gdio.common.objects.Space](#T-gdio-common-objects-Space 'gdio.common.objects.Space') | The [Space](#T-gdio-common-objects-Space 'gdio.common.objects.Space') to perform the rotation relative to. |
| waitForObject | [System.Boolean](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Boolean 'System.Boolean') | Wait for th object to exist if it doesn't. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-RotateObject-System-String,gdio-common-objects-Vector3,System-Single,gdio-common-objects-Space,System-Boolean,System-Int32-'></a>
### RotateObject(hierarchyPath,axis,angle,relativeTo,waitForObject,timeout) `method`

##### Summary

Rottate an objected defined by the HierarchyPath and rotated by the axis and angle, relative to the Space

##### Returns

Returns TRUE if the method call was successfully processed by the GameDriver agent.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath for the object to rotate. |
| axis | [gdio.common.objects.Vector3](#T-gdio-common-objects-Vector3 'gdio.common.objects.Vector3') |  |
| angle | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') |  |
| relativeTo | [gdio.common.objects.Space](#T-gdio-common-objects-Space 'gdio.common.objects.Space') | The [Space](#T-gdio-common-objects-Space 'gdio.common.objects.Space') to perform the rotation relative to. |
| waitForObject | [System.Boolean](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Boolean 'System.Boolean') | Wait for th object to exist if it doesn't. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-SetInputFieldText-System-String,System-String,System-Boolean,System-Int32-'></a>
### SetInputFieldText(hierarchyPath,value,waitForObject,timeout) `method`

##### Summary

Set the text of a InputField or TMP_InputField

##### Returns

Returns TRUE if the GameDriver agent was able to successfully set the InputField text.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath to the InputField or TMP_InputField. |
| value | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The text value to set in the field. |
| waitForObject | [System.Boolean](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Boolean 'System.Boolean') | If TRUE, wait for the object to exist if it doesn't. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The time to wait for the object to exist. |

<a name='M-gdio-unity_api-v2-ApiClient-SetObjectFieldValue-System-String,System-String,System-Object,System-Boolean,System-Int32,gdio-plugin-serializer-ICustomSerializer-'></a>
### SetObjectFieldValue(hierarchyPath,fieldOrPropertyName,value,waitForObject,timeout,valueSerializer) `method`

##### Summary

Set the field or property of an object.

##### Returns

Returns TRUE if the field/property was successfully set to the value.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath to the object to set the field/property value. |
| fieldOrPropertyName | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The field or property name to set the value of. |
| value | [System.Object](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Object 'System.Object') | The value to set for the field/property. |
| waitForObject | [System.Boolean](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Boolean 'System.Boolean') | If TRUE, wait for the object to exist if it doesn't. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The time to wait for the object to exist. |
| valueSerializer | [gdio.plugin.serializer.ICustomSerializer](#T-gdio-plugin-serializer-ICustomSerializer 'gdio.plugin.serializer.ICustomSerializer') | The [ICustomSerializer](#T-gdio-plugin-serializer-ICustomSerializer 'gdio.plugin.serializer.ICustomSerializer') used to serialize the value.  This is only required if a a custom class of object is being used. |

<a name='M-gdio-unity_api-v2-ApiClient-Tap-gdio-common-objects-Vector2,System-Int32,System-UInt64,System-Int32-'></a>
### Tap(position,tapCount,frameCount,timeout) `method`

##### Summary

Tap the handheld device at the defined position.

##### Returns

Returns TRUE if the GameDriver agent was able to process the request successfully.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| position | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | The vector position to tap the device screen. |
| tapCount | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of taps that should be registered. |
| frameCount | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to complete the tap input over. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-Tap-System-Single,System-Single,System-Int32,System-UInt64,System-Int32-'></a>
### Tap(x,y,tapCount,frameCount,timeout) `method`

##### Summary

Tap the handheld device at the defined position.

##### Returns

Returns TRUE if the GameDriver agent was able to process the request successfully.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| x | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The coordinate of the position to tap the device screen. |
| y | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The coordinate position to tap the device screen. |
| tapCount | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of taps that should be registered. |
| frameCount | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to complete the tap input over. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-TapObject-System-String,System-Int32,System-UInt64,System-Int32-'></a>
### TapObject(hierarchyPath,tapCount,frameCount,timeout) `method`

##### Summary

Tap an object.

##### Returns

Returns TRUE if the GameDriver agent was able to process the request successfully.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath of the object to tap. |
| tapCount | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of taps that should be registered. |
| frameCount | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to complete the tap input over. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-TouchInput-gdio-common-objects-Vector2,gdio-common-objects-Vector2,System-Int32,System-Int32,System-UInt64,System-Boolean,System-Single,System-Single,System-Single,System-Single,System-Single,System-Int32-'></a>
### TouchInput(startPosition,destinationPosition,fingerId,tapCount,frameCount,waitForEmptyInput,radius,pressure,altitudeAngle,azmulthAngle,maximumPossiblePressure,timeout) `method`

##### Summary

Send a raw TouchInput event to the game.

##### Returns

Returns TRUE if the GameDriver agent was able to process the request successfully.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| startPosition | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | Vector position of the start of the touch input. |
| destinationPosition | [gdio.common.objects.Vector2](#T-gdio-common-objects-Vector2 'gdio.common.objects.Vector2') | Vector destination position of where the touch input ends. |
| fingerId | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The finder id of the touch input. |
| tapCount | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of taps that should be registered. |
| frameCount | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to complete the tap input over. |
| waitForEmptyInput | [System.Boolean](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Boolean 'System.Boolean') | If TRUE, wait for the Empty Input event to be broadcast before returning from the method. |
| radius | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The radius of the touch input. |
| pressure | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The pressure of the touch input. |
| altitudeAngle | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The altitude angle of the touch input. |
| azmulthAngle | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The azmulth ange of the touch input. |
| maximumPossiblePressure | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The maximum possible pressure for the touch input. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-TouchInput-System-Single,System-Single,System-Single,System-Single,System-Int32,System-Int32,System-UInt64,System-Boolean,System-Single,System-Single,System-Single,System-Single,System-Single,System-Int32-'></a>
### TouchInput(x1,y1,x2,y2,fingerId,tapCount,frameCount,waitForEmptyInput,radius,pressure,altitudeAngle,azmulthAngle,maximumPossiblePressure,timeout) `method`

##### Summary

Send a raw TouchInput event to the game.

##### Returns

Returns TRUE if the GameDriver agent was able to process the request successfully.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| x1 | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The X coordinate of the start position. |
| y1 | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The Y coordinate of the start position. |
| x2 | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The X coordinate of the end position. |
| y2 | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The Y coordinate of the end position. |
| fingerId | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The finder id of the touch input. |
| tapCount | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of taps that should be registered. |
| frameCount | [System.UInt64](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.UInt64 'System.UInt64') | The number of frames to complete the tap input over. |
| waitForEmptyInput | [System.Boolean](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Boolean 'System.Boolean') | If TRUE, wait for the Empty Input event to be broadcast before returning from the method. |
| radius | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The radius of the touch input. |
| pressure | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The pressure of the touch input. |
| altitudeAngle | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The altitude angle of the touch input. |
| azmulthAngle | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The azmulth ange of the touch input. |
| maximumPossiblePressure | [System.Single](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Single 'System.Single') | The maximum possible pressure for the touch input. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The timeout in seconds to wait for a response that the request was processed by the GameDriver agent. |

<a name='M-gdio-unity_api-v2-ApiClient-Wait-System-Int32-'></a>
### Wait(milliSeconds) `method`

##### Summary

Client side Wait or Pause.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| milliSeconds | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The number of milliseconds to wait. |

<a name='M-gdio-unity_api-v2-ApiClient-WaitForObject-System-String,System-Int32-'></a>
### WaitForObject(hierarchyPath,timeout) `method`

##### Summary

Wait for an object to exist.

##### Returns

Returns TRUE if the object exists within the alloted timeout.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath of the object. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The amount of time to wait for the object to exist. |

<a name='M-gdio-unity_api-v2-ApiClient-WaitForObjectValue-System-String,System-String,System-Object,System-Boolean,System-Int32,gdio-plugin-serializer-ICustomSerializer-'></a>
### WaitForObjectValue(hierarchyPath,fieldOrPropertyName,value,waitForObject,timeout,valueSerializer) `method`

##### Summary

Wait for an object to exist and have a specific value for a specified field/property.

##### Returns

Returns TRUE if the object exists with the specified value in the alloted timeout.

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| hierarchyPath | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The HierarchyPath to the object. |
| fieldOrPropertyName | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') | The field/property name for inspection. |
| value | [System.Object](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Object 'System.Object') | The value to wait for. |
| waitForObject | [System.Boolean](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Boolean 'System.Boolean') | If TRUE, wait for the object to exist if it doesn't. |
| timeout | [System.Int32](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Int32 'System.Int32') | The amount of time to wait for the object to exist with the specified value. |
| valueSerializer | [gdio.plugin.serializer.ICustomSerializer](#T-gdio-plugin-serializer-ICustomSerializer 'gdio.plugin.serializer.ICustomSerializer') | The [ICustomSerializer](#T-gdio-plugin-serializer-ICustomSerializer 'gdio.plugin.serializer.ICustomSerializer') used to serialize the value.  This is only required if a a custom class of object is being used. |

<a name='T-gdio-unity_api-utilities-ScreenCapture-GDI32'></a>
## GDI32 `type`

##### Namespace

gdio.unity_api.utilities.ScreenCapture

##### Summary

Helper class containing Gdi32 API functions

<a name='T-gdio-unity_api-v2-GameConnectionDetails'></a>
## GameConnectionDetails `type`

##### Namespace

gdio.unity_api.v2

##### Summary

This class provides information about the currently connected game.

<a name='F-gdio-unity_api-v2-GameConnectionDetails-Addr'></a>
### Addr `constants`

##### Summary

The [IPAddress](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Net.IPAddress 'System.Net.IPAddress') of the connected game./>

<a name='F-gdio-unity_api-v2-GameConnectionDetails-GamePath'></a>
### GamePath `constants`

##### Summary

The Application.DataPath of the connected game.

<a name='F-gdio-unity_api-v2-GameConnectionDetails-IsEditor'></a>
### IsEditor `constants`

##### Summary

Boolean value if the game is running in an UnityEditor instance.

<a name='F-gdio-unity_api-v2-GameConnectionDetails-IsStandalone'></a>
### IsStandalone `constants`

##### Summary

Boolean value if the game is running as a Standalone instance.

<a name='F-gdio-unity_api-v2-GameConnectionDetails-Platform'></a>
### Platform `constants`

##### Summary

The Application.Platform of the connected game.

<a name='F-gdio-unity_api-v2-GameConnectionDetails-Port'></a>
### Port `constants`

##### Summary

The port number of the connected game.

<a name='T-gdio-unity_api-v2-HookingObject'></a>
## HookingObject `type`

##### Namespace

gdio.unity_api.v2

##### Summary

Enumeration of input types that can be hooked.  Currently TOUCHINPUT is bundled with MOUSE and GAMEPAD is not supported.

<a name='F-gdio-unity_api-v2-HookingObject-ALL'></a>
### ALL `constants`

##### Summary

All inputs

<a name='F-gdio-unity_api-v2-HookingObject-GAMEPAD'></a>
### GAMEPAD `constants`

##### Summary

Gamepad input, CURRENTLY NOT SUPPORTED

<a name='F-gdio-unity_api-v2-HookingObject-KEYBOARD'></a>
### KEYBOARD `constants`

##### Summary

Keyboard input

<a name='F-gdio-unity_api-v2-HookingObject-MOUSE'></a>
### MOUSE `constants`

##### Summary

Mouse input

<a name='F-gdio-unity_api-v2-HookingObject-TOUCHINPUT'></a>
### TOUCHINPUT `constants`

##### Summary

Touch input, enum value is currently not used.  Enabled/Disabled via [MOUSE](#F-gdio-unity_api-v2-HookingObject-MOUSE 'gdio.unity_api.v2.HookingObject.MOUSE') enumeration.

<a name='T-gdio-unity_api-KeyCode'></a>
## KeyCode `type`

##### Namespace

gdio.unity_api

##### Summary

Key codes returned by Event keyCode. These map directly to a physical key on the keyboard.

<a name='F-gdio-unity_api-KeyCode-A'></a>
### A `constants`

##### Summary

a' key

<a name='F-gdio-unity_api-KeyCode-Alpha0'></a>
### Alpha0 `constants`

##### Summary

The '0' key on the top of the alphanumeric keyboard

<a name='F-gdio-unity_api-KeyCode-Alpha1'></a>
### Alpha1 `constants`

##### Summary

The '1' key on the top of the alphanumeric keyboard

<a name='F-gdio-unity_api-KeyCode-Alpha2'></a>
### Alpha2 `constants`

##### Summary

The '2' key on the top of the alphanumeric keyboard

<a name='F-gdio-unity_api-KeyCode-Alpha3'></a>
### Alpha3 `constants`

##### Summary

The '3' key on the top of the alphanumeric keyboard

<a name='F-gdio-unity_api-KeyCode-Alpha4'></a>
### Alpha4 `constants`

##### Summary

The '4' key on the top of the alphanumeric keyboard

<a name='F-gdio-unity_api-KeyCode-Alpha5'></a>
### Alpha5 `constants`

##### Summary

The '5' key on the top of the alphanumeric keyboard

<a name='F-gdio-unity_api-KeyCode-Alpha6'></a>
### Alpha6 `constants`

##### Summary

The '6' key on the top of the alphanumeric keyboard

<a name='F-gdio-unity_api-KeyCode-Alpha7'></a>
### Alpha7 `constants`

##### Summary

The '7' key on the top of the alphanumeric keyboard

<a name='F-gdio-unity_api-KeyCode-Alpha8'></a>
### Alpha8 `constants`

##### Summary

The '8' key on the top of the alphanumeric keyboard

<a name='F-gdio-unity_api-KeyCode-Alpha9'></a>
### Alpha9 `constants`

##### Summary

The '9' key on the top of the alphanumeric keyboard

<a name='F-gdio-unity_api-KeyCode-AltGr'></a>
### AltGr `constants`

##### Summary

Alt Gr key

<a name='F-gdio-unity_api-KeyCode-Ampersand'></a>
### Ampersand `constants`

##### Summary

Ampersand key &

<a name='F-gdio-unity_api-KeyCode-Asterisk'></a>
### Asterisk `constants`

##### Summary

Asterisk key '*'

<a name='F-gdio-unity_api-KeyCode-At'></a>
### At `constants`

##### Summary

At key '@'

<a name='F-gdio-unity_api-KeyCode-B'></a>
### B `constants`

##### Summary

b' key

<a name='F-gdio-unity_api-KeyCode-BackQuote'></a>
### BackQuote `constants`

##### Summary

Back quote key '\`'

<a name='F-gdio-unity_api-KeyCode-Backslash'></a>
### Backslash `constants`

##### Summary

Backslash key '\'

<a name='F-gdio-unity_api-KeyCode-Backspace'></a>
### Backspace `constants`

##### Summary

The backspace key

<a name='F-gdio-unity_api-KeyCode-Break'></a>
### Break `constants`

##### Summary

Break key

<a name='F-gdio-unity_api-KeyCode-C'></a>
### C `constants`

##### Summary

c' key

<a name='F-gdio-unity_api-KeyCode-CapsLock'></a>
### CapsLock `constants`

##### Summary

Capslock key

<a name='F-gdio-unity_api-KeyCode-Caret'></a>
### Caret `constants`

##### Summary

Caret key '^'

<a name='F-gdio-unity_api-KeyCode-Clear'></a>
### Clear `constants`

##### Summary

The Clear key

<a name='F-gdio-unity_api-KeyCode-Colon'></a>
### Colon `constants`

##### Summary

Colon ':' key

<a name='F-gdio-unity_api-KeyCode-Comma'></a>
### Comma `constants`

##### Summary

Comma ',' key

<a name='F-gdio-unity_api-KeyCode-D'></a>
### D `constants`

##### Summary

d' key

<a name='F-gdio-unity_api-KeyCode-Delete'></a>
### Delete `constants`

##### Summary

The forward delete key

<a name='F-gdio-unity_api-KeyCode-Dollar'></a>
### Dollar `constants`

##### Summary

Dollar sign key $

<a name='F-gdio-unity_api-KeyCode-DoubleQuote'></a>
### DoubleQuote `constants`

##### Summary

Double quote key "

<a name='F-gdio-unity_api-KeyCode-DownArrow'></a>
### DownArrow `constants`

##### Summary

Down arrow key

<a name='F-gdio-unity_api-KeyCode-E'></a>
### E `constants`

##### Summary

e' key

<a name='F-gdio-unity_api-KeyCode-End'></a>
### End `constants`

##### Summary

End key

<a name='F-gdio-unity_api-KeyCode-Equals'></a>
### Equals `constants`

##### Summary

Equals '=' key

<a name='F-gdio-unity_api-KeyCode-Escape'></a>
### Escape `constants`

##### Summary

Escape key

<a name='F-gdio-unity_api-KeyCode-Exclaim'></a>
### Exclaim `constants`

##### Summary

Exclamation mark key !

<a name='F-gdio-unity_api-KeyCode-F'></a>
### F `constants`

##### Summary

f' key

<a name='F-gdio-unity_api-KeyCode-F1'></a>
### F1 `constants`

##### Summary

F1 function key

<a name='F-gdio-unity_api-KeyCode-F10'></a>
### F10 `constants`

##### Summary

F10 function key

<a name='F-gdio-unity_api-KeyCode-F11'></a>
### F11 `constants`

##### Summary

F11 function key

<a name='F-gdio-unity_api-KeyCode-F12'></a>
### F12 `constants`

##### Summary

F12 function key

<a name='F-gdio-unity_api-KeyCode-F13'></a>
### F13 `constants`

##### Summary

F13 function key

<a name='F-gdio-unity_api-KeyCode-F14'></a>
### F14 `constants`

##### Summary

F14 function key

<a name='F-gdio-unity_api-KeyCode-F15'></a>
### F15 `constants`

##### Summary

F15 function key

<a name='F-gdio-unity_api-KeyCode-F2'></a>
### F2 `constants`

##### Summary

F2 function key

<a name='F-gdio-unity_api-KeyCode-F3'></a>
### F3 `constants`

##### Summary

F3 function key

<a name='F-gdio-unity_api-KeyCode-F4'></a>
### F4 `constants`

##### Summary

F4 function key

<a name='F-gdio-unity_api-KeyCode-F5'></a>
### F5 `constants`

##### Summary

F5 function key

<a name='F-gdio-unity_api-KeyCode-F6'></a>
### F6 `constants`

##### Summary

F6 function key

<a name='F-gdio-unity_api-KeyCode-F7'></a>
### F7 `constants`

##### Summary

F7 function key

<a name='F-gdio-unity_api-KeyCode-F8'></a>
### F8 `constants`

##### Summary

F8 function key

<a name='F-gdio-unity_api-KeyCode-F9'></a>
### F9 `constants`

##### Summary

F9 function key

<a name='F-gdio-unity_api-KeyCode-G'></a>
### G `constants`

##### Summary

g' key

<a name='F-gdio-unity_api-KeyCode-Greater'></a>
### Greater `constants`

##### Summary

Greater than '>' key

<a name='F-gdio-unity_api-KeyCode-H'></a>
### H `constants`

##### Summary

h' key

<a name='F-gdio-unity_api-KeyCode-Hash'></a>
### Hash `constants`

##### Summary

Hash key #

<a name='F-gdio-unity_api-KeyCode-Help'></a>
### Help `constants`

##### Summary

Help key

<a name='F-gdio-unity_api-KeyCode-Home'></a>
### Home `constants`

##### Summary

Home key

<a name='F-gdio-unity_api-KeyCode-I'></a>
### I `constants`

##### Summary

i' key

<a name='F-gdio-unity_api-KeyCode-Insert'></a>
### Insert `constants`

##### Summary

Insert key key

<a name='F-gdio-unity_api-KeyCode-J'></a>
### J `constants`

##### Summary

j' key

<a name='F-gdio-unity_api-KeyCode-Joystick1Button0'></a>
### Joystick1Button0 `constants`

##### Summary

Button 0 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button1'></a>
### Joystick1Button1 `constants`

##### Summary

Button 1 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button10'></a>
### Joystick1Button10 `constants`

##### Summary

Button 10 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button11'></a>
### Joystick1Button11 `constants`

##### Summary

Button 11 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button12'></a>
### Joystick1Button12 `constants`

##### Summary

Button 12 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button13'></a>
### Joystick1Button13 `constants`

##### Summary

Button 13 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button14'></a>
### Joystick1Button14 `constants`

##### Summary

Button 14 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button15'></a>
### Joystick1Button15 `constants`

##### Summary

Button 15 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button16'></a>
### Joystick1Button16 `constants`

##### Summary

Button 16 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button17'></a>
### Joystick1Button17 `constants`

##### Summary

Button 17 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button18'></a>
### Joystick1Button18 `constants`

##### Summary

Button 18 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button19'></a>
### Joystick1Button19 `constants`

##### Summary

Button 19 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button2'></a>
### Joystick1Button2 `constants`

##### Summary

Button 2 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button3'></a>
### Joystick1Button3 `constants`

##### Summary

Button 3 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button4'></a>
### Joystick1Button4 `constants`

##### Summary

Button 4 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button5'></a>
### Joystick1Button5 `constants`

##### Summary

Button 5 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button6'></a>
### Joystick1Button6 `constants`

##### Summary

Button 6 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button7'></a>
### Joystick1Button7 `constants`

##### Summary

Button 7 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button8'></a>
### Joystick1Button8 `constants`

##### Summary

Button 8 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick1Button9'></a>
### Joystick1Button9 `constants`

##### Summary

Button 9 on first joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button0'></a>
### Joystick2Button0 `constants`

##### Summary

Button 0 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button1'></a>
### Joystick2Button1 `constants`

##### Summary

Button 1 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button10'></a>
### Joystick2Button10 `constants`

##### Summary

Button 10 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button11'></a>
### Joystick2Button11 `constants`

##### Summary

Button 11 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button12'></a>
### Joystick2Button12 `constants`

##### Summary

Button 12 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button13'></a>
### Joystick2Button13 `constants`

##### Summary

Button 13 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button14'></a>
### Joystick2Button14 `constants`

##### Summary

Button 14 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button15'></a>
### Joystick2Button15 `constants`

##### Summary

Button 15 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button16'></a>
### Joystick2Button16 `constants`

##### Summary

Button 16 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button17'></a>
### Joystick2Button17 `constants`

##### Summary

Button 17 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button18'></a>
### Joystick2Button18 `constants`

##### Summary

Button 18 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button19'></a>
### Joystick2Button19 `constants`

##### Summary

Button 19 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button2'></a>
### Joystick2Button2 `constants`

##### Summary

Button 2 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button3'></a>
### Joystick2Button3 `constants`

##### Summary

Button 3 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button4'></a>
### Joystick2Button4 `constants`

##### Summary

Button 4 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button5'></a>
### Joystick2Button5 `constants`

##### Summary

Button 5 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button6'></a>
### Joystick2Button6 `constants`

##### Summary

Button 6 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button7'></a>
### Joystick2Button7 `constants`

##### Summary

Button 7 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button8'></a>
### Joystick2Button8 `constants`

##### Summary

Button 8 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick2Button9'></a>
### Joystick2Button9 `constants`

##### Summary

Button 9 on second joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button0'></a>
### Joystick3Button0 `constants`

##### Summary

Button 0 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button1'></a>
### Joystick3Button1 `constants`

##### Summary

Button 1 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button10'></a>
### Joystick3Button10 `constants`

##### Summary

Button 10 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button11'></a>
### Joystick3Button11 `constants`

##### Summary

Button 11 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button12'></a>
### Joystick3Button12 `constants`

##### Summary

Button 12 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button13'></a>
### Joystick3Button13 `constants`

##### Summary

Button 13 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button14'></a>
### Joystick3Button14 `constants`

##### Summary

Button 14 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button15'></a>
### Joystick3Button15 `constants`

##### Summary

Button 15 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button16'></a>
### Joystick3Button16 `constants`

##### Summary

Button 16 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button17'></a>
### Joystick3Button17 `constants`

##### Summary

Button 17 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button18'></a>
### Joystick3Button18 `constants`

##### Summary

Button 18 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button19'></a>
### Joystick3Button19 `constants`

##### Summary

Button 19 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button2'></a>
### Joystick3Button2 `constants`

##### Summary

Button 2 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button3'></a>
### Joystick3Button3 `constants`

##### Summary

Button 3 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button4'></a>
### Joystick3Button4 `constants`

##### Summary

Button 4 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button5'></a>
### Joystick3Button5 `constants`

##### Summary

Button 5 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button6'></a>
### Joystick3Button6 `constants`

##### Summary

Button 6 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button7'></a>
### Joystick3Button7 `constants`

##### Summary

Button 7 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button8'></a>
### Joystick3Button8 `constants`

##### Summary

Button 8 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick3Button9'></a>
### Joystick3Button9 `constants`

##### Summary

Button 9 on third joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button0'></a>
### Joystick4Button0 `constants`

##### Summary

Button 0 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button1'></a>
### Joystick4Button1 `constants`

##### Summary

Button 1 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button10'></a>
### Joystick4Button10 `constants`

##### Summary

Button 10 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button11'></a>
### Joystick4Button11 `constants`

##### Summary

Button 11 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button12'></a>
### Joystick4Button12 `constants`

##### Summary

Button 12 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button13'></a>
### Joystick4Button13 `constants`

##### Summary

Button 13 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button14'></a>
### Joystick4Button14 `constants`

##### Summary

Button 14 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button15'></a>
### Joystick4Button15 `constants`

##### Summary

Button 15 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button16'></a>
### Joystick4Button16 `constants`

##### Summary

Button 16 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button17'></a>
### Joystick4Button17 `constants`

##### Summary

Button 17 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button18'></a>
### Joystick4Button18 `constants`

##### Summary

Button 18 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button19'></a>
### Joystick4Button19 `constants`

##### Summary

Button 19 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button2'></a>
### Joystick4Button2 `constants`

##### Summary

Button 2 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button3'></a>
### Joystick4Button3 `constants`

##### Summary

Button 3 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button4'></a>
### Joystick4Button4 `constants`

##### Summary

Button 4 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button5'></a>
### Joystick4Button5 `constants`

##### Summary

Button 5 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button6'></a>
### Joystick4Button6 `constants`

##### Summary

Button 6 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button7'></a>
### Joystick4Button7 `constants`

##### Summary

Button 7 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button8'></a>
### Joystick4Button8 `constants`

##### Summary

Button 8 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick4Button9'></a>
### Joystick4Button9 `constants`

##### Summary

Button 9 on forth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button0'></a>
### Joystick5Button0 `constants`

##### Summary

Button 0 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button1'></a>
### Joystick5Button1 `constants`

##### Summary

Button 1 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button10'></a>
### Joystick5Button10 `constants`

##### Summary

Button 10 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button11'></a>
### Joystick5Button11 `constants`

##### Summary

Button 11 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button12'></a>
### Joystick5Button12 `constants`

##### Summary

Button 12 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button13'></a>
### Joystick5Button13 `constants`

##### Summary

Button 13 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button14'></a>
### Joystick5Button14 `constants`

##### Summary

Button 14 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button15'></a>
### Joystick5Button15 `constants`

##### Summary

Button 15 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button16'></a>
### Joystick5Button16 `constants`

##### Summary

Button 16 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button17'></a>
### Joystick5Button17 `constants`

##### Summary

Button 17 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button18'></a>
### Joystick5Button18 `constants`

##### Summary

Button 18 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button19'></a>
### Joystick5Button19 `constants`

##### Summary

Button 19 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button2'></a>
### Joystick5Button2 `constants`

##### Summary

Button 2 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button3'></a>
### Joystick5Button3 `constants`

##### Summary

Button 3 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button4'></a>
### Joystick5Button4 `constants`

##### Summary

Button 4 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button5'></a>
### Joystick5Button5 `constants`

##### Summary

Button 5 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button6'></a>
### Joystick5Button6 `constants`

##### Summary

Button 6 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button7'></a>
### Joystick5Button7 `constants`

##### Summary

Button 7 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button8'></a>
### Joystick5Button8 `constants`

##### Summary

Button 8 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick5Button9'></a>
### Joystick5Button9 `constants`

##### Summary

Button 9 on fifth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button0'></a>
### Joystick6Button0 `constants`

##### Summary

Button 0 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button1'></a>
### Joystick6Button1 `constants`

##### Summary

Button 1 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button10'></a>
### Joystick6Button10 `constants`

##### Summary

Button 10 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button11'></a>
### Joystick6Button11 `constants`

##### Summary

Button 11 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button12'></a>
### Joystick6Button12 `constants`

##### Summary

Button 12 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button13'></a>
### Joystick6Button13 `constants`

##### Summary

Button 13 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button14'></a>
### Joystick6Button14 `constants`

##### Summary

Button 14 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button15'></a>
### Joystick6Button15 `constants`

##### Summary

Button 15 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button16'></a>
### Joystick6Button16 `constants`

##### Summary

Button 16 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button17'></a>
### Joystick6Button17 `constants`

##### Summary

Button 17 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button18'></a>
### Joystick6Button18 `constants`

##### Summary

Button 18 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button19'></a>
### Joystick6Button19 `constants`

##### Summary

Button 19 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button2'></a>
### Joystick6Button2 `constants`

##### Summary

Button 2 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button3'></a>
### Joystick6Button3 `constants`

##### Summary

Button 3 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button4'></a>
### Joystick6Button4 `constants`

##### Summary

Button 4 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button5'></a>
### Joystick6Button5 `constants`

##### Summary

Button 5 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button6'></a>
### Joystick6Button6 `constants`

##### Summary

Button 6 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button7'></a>
### Joystick6Button7 `constants`

##### Summary

Button 7 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button8'></a>
### Joystick6Button8 `constants`

##### Summary

Button 8 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick6Button9'></a>
### Joystick6Button9 `constants`

##### Summary

Button 9 on sixth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button0'></a>
### Joystick7Button0 `constants`

##### Summary

Button 0 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button1'></a>
### Joystick7Button1 `constants`

##### Summary

Button 1 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button10'></a>
### Joystick7Button10 `constants`

##### Summary

Button 10 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button11'></a>
### Joystick7Button11 `constants`

##### Summary

Button 11 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button12'></a>
### Joystick7Button12 `constants`

##### Summary

Button 12 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button13'></a>
### Joystick7Button13 `constants`

##### Summary

Button 13 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button14'></a>
### Joystick7Button14 `constants`

##### Summary

Button 14 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button15'></a>
### Joystick7Button15 `constants`

##### Summary

Button 15 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button16'></a>
### Joystick7Button16 `constants`

##### Summary

Button 16 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button17'></a>
### Joystick7Button17 `constants`

##### Summary

Button 17 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button18'></a>
### Joystick7Button18 `constants`

##### Summary

Button 18 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button19'></a>
### Joystick7Button19 `constants`

##### Summary

Button 19 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button2'></a>
### Joystick7Button2 `constants`

##### Summary

Button 2 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button3'></a>
### Joystick7Button3 `constants`

##### Summary

Button 3 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button4'></a>
### Joystick7Button4 `constants`

##### Summary

Button 4 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button5'></a>
### Joystick7Button5 `constants`

##### Summary

Button 5 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button6'></a>
### Joystick7Button6 `constants`

##### Summary

Button 6 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button7'></a>
### Joystick7Button7 `constants`

##### Summary

Button 7 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button8'></a>
### Joystick7Button8 `constants`

##### Summary

Button 8 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick7Button9'></a>
### Joystick7Button9 `constants`

##### Summary

Button 9 on seventh joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button0'></a>
### Joystick8Button0 `constants`

##### Summary

Button 0 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button1'></a>
### Joystick8Button1 `constants`

##### Summary

Button 1 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button10'></a>
### Joystick8Button10 `constants`

##### Summary

Button 10 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button11'></a>
### Joystick8Button11 `constants`

##### Summary

Button 11 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button12'></a>
### Joystick8Button12 `constants`

##### Summary

Button 12 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button13'></a>
### Joystick8Button13 `constants`

##### Summary

Button 13 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button14'></a>
### Joystick8Button14 `constants`

##### Summary

Button 14 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button15'></a>
### Joystick8Button15 `constants`

##### Summary

Button 15 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button16'></a>
### Joystick8Button16 `constants`

##### Summary

Button 16 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button17'></a>
### Joystick8Button17 `constants`

##### Summary

Button 17 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button18'></a>
### Joystick8Button18 `constants`

##### Summary

Button 18 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button19'></a>
### Joystick8Button19 `constants`

##### Summary

Button 19 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button2'></a>
### Joystick8Button2 `constants`

##### Summary

Button 2 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button3'></a>
### Joystick8Button3 `constants`

##### Summary

Button 3 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button4'></a>
### Joystick8Button4 `constants`

##### Summary

Button 4 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button5'></a>
### Joystick8Button5 `constants`

##### Summary

Button 5 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button6'></a>
### Joystick8Button6 `constants`

##### Summary

Button 6 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button7'></a>
### Joystick8Button7 `constants`

##### Summary

Button 7 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button8'></a>
### Joystick8Button8 `constants`

##### Summary

Button 8 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-Joystick8Button9'></a>
### Joystick8Button9 `constants`

##### Summary

Button 9 on eighth joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton0'></a>
### JoystickButton0 `constants`

##### Summary

Button 0 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton1'></a>
### JoystickButton1 `constants`

##### Summary

Button 1 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton10'></a>
### JoystickButton10 `constants`

##### Summary

Button 10 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton11'></a>
### JoystickButton11 `constants`

##### Summary

Button 11 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton12'></a>
### JoystickButton12 `constants`

##### Summary

Button 12 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton13'></a>
### JoystickButton13 `constants`

##### Summary

Button 13 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton14'></a>
### JoystickButton14 `constants`

##### Summary

Button 14 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton15'></a>
### JoystickButton15 `constants`

##### Summary

Button 15 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton16'></a>
### JoystickButton16 `constants`

##### Summary

Button 16 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton17'></a>
### JoystickButton17 `constants`

##### Summary

Button 17 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton18'></a>
### JoystickButton18 `constants`

##### Summary

Button 18 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton19'></a>
### JoystickButton19 `constants`

##### Summary

Button 19 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton2'></a>
### JoystickButton2 `constants`

##### Summary

Button 2 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton3'></a>
### JoystickButton3 `constants`

##### Summary

Button 3 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton4'></a>
### JoystickButton4 `constants`

##### Summary

Button 4 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton5'></a>
### JoystickButton5 `constants`

##### Summary

Button 5 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton6'></a>
### JoystickButton6 `constants`

##### Summary

Button 6 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton7'></a>
### JoystickButton7 `constants`

##### Summary

Button 7 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton8'></a>
### JoystickButton8 `constants`

##### Summary

Button 8 on any joystick

<a name='F-gdio-unity_api-KeyCode-JoystickButton9'></a>
### JoystickButton9 `constants`

##### Summary

Button 9 on any joystick

<a name='F-gdio-unity_api-KeyCode-K'></a>
### K `constants`

##### Summary

k' key

<a name='F-gdio-unity_api-KeyCode-Keypad0'></a>
### Keypad0 `constants`

##### Summary

Numeric keypad 0

<a name='F-gdio-unity_api-KeyCode-Keypad1'></a>
### Keypad1 `constants`

##### Summary

Numeric keypad 1

<a name='F-gdio-unity_api-KeyCode-Keypad2'></a>
### Keypad2 `constants`

##### Summary

Numeric keypad 2

<a name='F-gdio-unity_api-KeyCode-Keypad3'></a>
### Keypad3 `constants`

##### Summary

Numeric keypad 3

<a name='F-gdio-unity_api-KeyCode-Keypad4'></a>
### Keypad4 `constants`

##### Summary

Numeric keypad 4

<a name='F-gdio-unity_api-KeyCode-Keypad5'></a>
### Keypad5 `constants`

##### Summary

Numeric keypad 5

<a name='F-gdio-unity_api-KeyCode-Keypad6'></a>
### Keypad6 `constants`

##### Summary

Numeric keypad 6

<a name='F-gdio-unity_api-KeyCode-Keypad7'></a>
### Keypad7 `constants`

##### Summary

Numeric keypad 7

<a name='F-gdio-unity_api-KeyCode-Keypad8'></a>
### Keypad8 `constants`

##### Summary

Numeric keypad 8

<a name='F-gdio-unity_api-KeyCode-Keypad9'></a>
### Keypad9 `constants`

##### Summary

Numeric keypad 9

<a name='F-gdio-unity_api-KeyCode-KeypadDivide'></a>
### KeypadDivide `constants`

##### Summary

Numeric keypad '/'

<a name='F-gdio-unity_api-KeyCode-KeypadEnter'></a>
### KeypadEnter `constants`

##### Summary

Numeric keypad enter

<a name='F-gdio-unity_api-KeyCode-KeypadEquals'></a>
### KeypadEquals `constants`

##### Summary

Numeric keypad '='

<a name='F-gdio-unity_api-KeyCode-KeypadMinus'></a>
### KeypadMinus `constants`

##### Summary

Numeric keypad '-'

<a name='F-gdio-unity_api-KeyCode-KeypadMultiply'></a>
### KeypadMultiply `constants`

##### Summary

Numeric keypad '*'

<a name='F-gdio-unity_api-KeyCode-KeypadPeriod'></a>
### KeypadPeriod `constants`

##### Summary

Numeric keypad '

<a name='F-gdio-unity_api-KeyCode-KeypadPlus'></a>
### KeypadPlus `constants`

##### Summary

Numeric keypad '+'

<a name='F-gdio-unity_api-KeyCode-L'></a>
### L `constants`

##### Summary

l' key

<a name='F-gdio-unity_api-KeyCode-LeftAlt'></a>
### LeftAlt `constants`

##### Summary

Left Alt key

<a name='F-gdio-unity_api-KeyCode-LeftApple'></a>
### LeftApple `constants`

##### Summary

Left Command key

<a name='F-gdio-unity_api-KeyCode-LeftArrow'></a>
### LeftArrow `constants`

##### Summary

Left arrow key

<a name='F-gdio-unity_api-KeyCode-LeftBracket'></a>
### LeftBracket `constants`

##### Summary

Left square bracket key '['

<a name='F-gdio-unity_api-KeyCode-LeftCommand'></a>
### LeftCommand `constants`

##### Summary

Left Command key

<a name='F-gdio-unity_api-KeyCode-LeftControl'></a>
### LeftControl `constants`

##### Summary

Left Control key

<a name='F-gdio-unity_api-KeyCode-LeftParen'></a>
### LeftParen `constants`

##### Summary

Left Parenthesis key '('

<a name='F-gdio-unity_api-KeyCode-LeftShift'></a>
### LeftShift `constants`

##### Summary

Left shift key

<a name='F-gdio-unity_api-KeyCode-LeftWindows'></a>
### LeftWindows `constants`

##### Summary

Left Windows key

<a name='F-gdio-unity_api-KeyCode-Less'></a>
### Less `constants`

##### Summary

Less than '<' key

<a name='F-gdio-unity_api-KeyCode-M'></a>
### M `constants`

##### Summary

m' key

<a name='F-gdio-unity_api-KeyCode-Menu'></a>
### Menu `constants`

##### Summary

Menu key

<a name='F-gdio-unity_api-KeyCode-Minus'></a>
### Minus `constants`

##### Summary

Minus '-' key

<a name='F-gdio-unity_api-KeyCode-Mouse0'></a>
### Mouse0 `constants`

##### Summary

The Left (or primary) mouse button

<a name='F-gdio-unity_api-KeyCode-Mouse1'></a>
### Mouse1 `constants`

##### Summary

Right mouse button (or secondary mouse button)

<a name='F-gdio-unity_api-KeyCode-Mouse2'></a>
### Mouse2 `constants`

##### Summary

Middle mouse button (or third button)

<a name='F-gdio-unity_api-KeyCode-Mouse3'></a>
### Mouse3 `constants`

##### Summary

Additional (fourth) mouse button

<a name='F-gdio-unity_api-KeyCode-Mouse4'></a>
### Mouse4 `constants`

##### Summary

Additional (fifth) mouse button

<a name='F-gdio-unity_api-KeyCode-Mouse5'></a>
### Mouse5 `constants`

##### Summary

Additional (or sixth) mouse button

<a name='F-gdio-unity_api-KeyCode-Mouse6'></a>
### Mouse6 `constants`

##### Summary

Additional (or seventh) mouse button

<a name='F-gdio-unity_api-KeyCode-N'></a>
### N `constants`

##### Summary

n' key

<a name='F-gdio-unity_api-KeyCode-None'></a>
### None `constants`

##### Summary

Not assigned (never returned as the result of a keystroke)

<a name='F-gdio-unity_api-KeyCode-Numlock'></a>
### Numlock `constants`

##### Summary

Numlock key

<a name='F-gdio-unity_api-KeyCode-O'></a>
### O `constants`

##### Summary

o' key

<a name='F-gdio-unity_api-KeyCode-P'></a>
### P `constants`

##### Summary

p' key

<a name='F-gdio-unity_api-KeyCode-PageDown'></a>
### PageDown `constants`

##### Summary

Page down

<a name='F-gdio-unity_api-KeyCode-PageUp'></a>
### PageUp `constants`

##### Summary

Page up

<a name='F-gdio-unity_api-KeyCode-Pause'></a>
### Pause `constants`

##### Summary

Pause on PC machines

<a name='F-gdio-unity_api-KeyCode-Period'></a>
### Period `constants`

##### Summary

Period '

<a name='F-gdio-unity_api-KeyCode-Plus'></a>
### Plus `constants`

##### Summary

Plus key '+'

<a name='F-gdio-unity_api-KeyCode-Print'></a>
### Print `constants`

##### Summary

Print key

<a name='F-gdio-unity_api-KeyCode-Q'></a>
### Q `constants`

##### Summary

q' key

<a name='F-gdio-unity_api-KeyCode-Question'></a>
### Question `constants`

##### Summary

Question mark '?' key

<a name='F-gdio-unity_api-KeyCode-Quote'></a>
### Quote `constants`

##### Summary

Quote key '

<a name='F-gdio-unity_api-KeyCode-R'></a>
### R `constants`

##### Summary

r' key

<a name='F-gdio-unity_api-KeyCode-Return'></a>
### Return `constants`

##### Summary

Return key

<a name='F-gdio-unity_api-KeyCode-RightAlt'></a>
### RightAlt `constants`

##### Summary

Right Alt key

<a name='F-gdio-unity_api-KeyCode-RightApple'></a>
### RightApple `constants`

##### Summary

Right Command key

<a name='F-gdio-unity_api-KeyCode-RightArrow'></a>
### RightArrow `constants`

##### Summary

Right arrow key

<a name='F-gdio-unity_api-KeyCode-RightBracket'></a>
### RightBracket `constants`

##### Summary

Right square bracket key ']'

<a name='F-gdio-unity_api-KeyCode-RightCommand'></a>
### RightCommand `constants`

##### Summary

Right Command key

<a name='F-gdio-unity_api-KeyCode-RightControl'></a>
### RightControl `constants`

##### Summary

Right Control key

<a name='F-gdio-unity_api-KeyCode-RightParen'></a>
### RightParen `constants`

##### Summary

Right Parenthesis key ')'

<a name='F-gdio-unity_api-KeyCode-RightShift'></a>
### RightShift `constants`

##### Summary

Right shift key

<a name='F-gdio-unity_api-KeyCode-RightWindows'></a>
### RightWindows `constants`

##### Summary

Right Windows key

<a name='F-gdio-unity_api-KeyCode-S'></a>
### S `constants`

##### Summary

s' key

<a name='F-gdio-unity_api-KeyCode-ScrollLock'></a>
### ScrollLock `constants`

##### Summary

Scroll lock key

<a name='F-gdio-unity_api-KeyCode-Semicolon'></a>
### Semicolon `constants`

##### Summary

Semicolon ';' key

<a name='F-gdio-unity_api-KeyCode-Slash'></a>
### Slash `constants`

##### Summary

Slash '/' key

<a name='F-gdio-unity_api-KeyCode-Space'></a>
### Space `constants`

##### Summary

Space key

<a name='F-gdio-unity_api-KeyCode-SysReq'></a>
### SysReq `constants`

##### Summary

Sys Req key

<a name='F-gdio-unity_api-KeyCode-T'></a>
### T `constants`

##### Summary

t' key

<a name='F-gdio-unity_api-KeyCode-Tab'></a>
### Tab `constants`

##### Summary

The tab key

<a name='F-gdio-unity_api-KeyCode-U'></a>
### U `constants`

##### Summary

u' key

<a name='F-gdio-unity_api-KeyCode-Underscore'></a>
### Underscore `constants`

##### Summary

Underscore '_' key

<a name='F-gdio-unity_api-KeyCode-UpArrow'></a>
### UpArrow `constants`

##### Summary

Up arrow key

<a name='F-gdio-unity_api-KeyCode-V'></a>
### V `constants`

##### Summary

v' key

<a name='F-gdio-unity_api-KeyCode-W'></a>
### W `constants`

##### Summary

w' key

<a name='F-gdio-unity_api-KeyCode-X'></a>
### X `constants`

##### Summary

x' key

<a name='F-gdio-unity_api-KeyCode-Y'></a>
### Y `constants`

##### Summary

y' key

<a name='F-gdio-unity_api-KeyCode-Z'></a>
### Z `constants`

##### Summary

z' key

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
| filename | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') |  |
| format | [System.Drawing.Imaging.ImageFormat](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Drawing.Imaging.ImageFormat 'System.Drawing.Imaging.ImageFormat') |  |

<a name='M-gdio-unity_api-utilities-ScreenCapture-CaptureWindow-System-IntPtr-'></a>
### CaptureWindow(handle) `method`

##### Summary

Creates an Image object containing a screen shot of a specific window

##### Returns



##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| handle | [System.IntPtr](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.IntPtr 'System.IntPtr') | The handle to the window. (In windows forms, this is obtained by the Handle property) |

<a name='M-gdio-unity_api-utilities-ScreenCapture-CaptureWindowToFile-System-IntPtr,System-String,System-Drawing-Imaging-ImageFormat-'></a>
### CaptureWindowToFile(handle,filename,format) `method`

##### Summary

Captures a screen shot of a specific window, and saves it to a file

##### Parameters

| Name | Type | Description |
| ---- | ---- | ----------- |
| handle | [System.IntPtr](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.IntPtr 'System.IntPtr') |  |
| filename | [System.String](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.String 'System.String') |  |
| format | [System.Drawing.Imaging.ImageFormat](http://msdn.microsoft.com/query/dev14.query?appId=Dev14IDEF1&l=EN-US&k=k:System.Drawing.Imaging.ImageFormat 'System.Drawing.Imaging.ImageFormat') |  |

<a name='T-gdio-unity_api-utilities-ScreenCapture-User32'></a>
## User32 `type`

##### Namespace

gdio.unity_api.utilities.ScreenCapture

##### Summary

Helper class containing User32 API functions
