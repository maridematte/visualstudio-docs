---
description: "Retrieves the file name for the last load error."
title: "IDiaDataSource::get_lastError"
ms.date: "11/04/2016"
ms.topic: "reference"
dev_langs:
  - "C++"
helpviewer_keywords:
  - "IDiaDataSource::get_lastError method"
author: "mikejo5000"
ms.author: "mikejo"
manager: jmartens
ms.technology: vs-ide-debug
---
# IDiaDataSource::get_lastError

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Retrieves the file name for the last load error.

## Syntax

```C++
HRESULT get_lastError (
   BSTR* pRetVal
);
```

#### Parameters
 pRetVal

[out] Returns a string that contains the .pdb file name associated with the last load error.

## Return Value
 Returns the last error code caused by a load operation. Returns `E_INVALIDARG` if the `pRetVal` parameter is `NULL`.

## Example

```C++
BSTR    fileName;
HRESULT errorCode = pSource->get_lastError( &fileName );
```

## See also
- [IDiaDataSource](../../debugger/debug-interface-access/idiadatasource.md)
