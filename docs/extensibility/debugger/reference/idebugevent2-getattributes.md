---
description: "Gets the attributes for this debug event."
title: IDebugEvent2::GetAttributes
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- IDebugEvent2::GetAttributes
helpviewer_keywords:
- IDebugEvent2::GetAttributes
author: maiak
ms.author: maiak
manager: jmartens
ms.technology: vs-ide-debug
dev_langs:
- CPP
- CSharp
---
# IDebugEvent2::GetAttributes

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Gets the attributes for this debug event.

## Syntax

### [C#](#tab/csharp)
```csharp
int GetAttribute( 
   out uint pdwAttrib
);
```
### [C++](#tab/cpp)
```cpp
HRESULT GetAttribute( 
   DWORD* pdwAttrib
);
```
---

## Parameters
`pdwAttrib`\
[out] A combination of flags from the [EVENTATTRIBUTES](../../../extensibility/debugger/reference/eventattributes.md) enumeration.

## Return Value
 If successful, returns `S_OK`; otherwise, returns an error code.

## Remarks
 The [IDebugEvent2](../../../extensibility/debugger/reference/idebugevent2.md) interface is common to all events. This method describes the type of event; for example, is the event synchronous or asynchronous and is it a stopping event.

## See also
- [IDebugEvent2](../../../extensibility/debugger/reference/idebugevent2.md)
- [EVENTATTRIBUTES](../../../extensibility/debugger/reference/eventattributes.md)
