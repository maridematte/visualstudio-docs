---
description: "Determines if the field represents a closed type."
title: IDebugExtendedField::IsClosedType
ms.date: 11/04/2016
ms.topic: reference
helpviewer_keywords:
- IsClosedType
- IDebugExtendedField::IsClosedType
author: maiak
ms.author: maiak
manager: jmartens
ms.technology: vs-ide-debug
dev_langs:
- CPP
- CSharp
---
# IDebugExtendedField::IsClosedType

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Determines if the field represents a closed type.

## Syntax

### [C#](#tab/csharp)
```csharp
int IsClosedType();
```
### [C++](#tab/cpp)
```cpp
HRESULT IsClosedType(
   void
);
```
---

## Return Value
 If the field is a closed type, returns `S_OK`; otherwise, returns `S_FALSE`.

## See also
- [IDebugExtendedField](../../../extensibility/debugger/reference/idebugextendedfield.md)
