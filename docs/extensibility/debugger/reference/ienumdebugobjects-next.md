---
description: "This method returns the next set of IDebugObject elements from the enumeration."
title: IEnumDebugObjects::Next
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- IEnumDebugObjects::Next
helpviewer_keywords:
- IEnumDebugObjects::Next method
author: maiak
ms.author: maiak
manager: jmartens
ms.technology: vs-ide-debug
dev_langs:
- CPP
- CSharp
---
# IEnumDebugObjects::Next

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
This method returns the next set of elements from the enumeration.

## Syntax

### [C#](#tab/csharp)
```csharp
int Next(
   uint           celt,
   IDebugObject[] rgelt,
   ref uint       pceltFetched
);
```
### [C++](#tab/cpp)
```cpp
HRESULT Next(
   ULONG          celt,
   IDebugObject** rgelt,
   ULONG*         pceltFetched
);
```
---

## Parameters
`celt`\
[in] The number of elements to retrieve. Also specifies the maximum size of the `rgelt` array.

`rgelt`\
[in, out] Array of [IDebugObject](../../../extensibility/debugger/reference/idebugobject.md) elements to be filled in.

`pceltFetched`\
[out] Returns the number of elements actually returned in `rgelt`.

## Return Value
 If successful, returns `S_OK`. Returns `S_FALSE` if fewer than the requested number of elements could be returned; otherwise, returns an error code.

## See also
- [IEnumDebugObjects](../../../extensibility/debugger/reference/ienumdebugobjects.md)
- [IDebugObject](../../../extensibility/debugger/reference/idebugobject.md)
