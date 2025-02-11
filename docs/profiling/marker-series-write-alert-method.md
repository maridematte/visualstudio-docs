---
description: "Writes an alert to the Concurrency Visualizer trace file."
title: marker_series::write_alert Method
ms.date: 11/04/2016
ms.topic: reference
f1_keywords: 
- cvmarkersobj/Concurrency, diagnostic:marker_series::write_alert
helpviewer_keywords: 
- Concurrency, diagnostic:marker_series::write_alert method
author: mikejo5000
ms.author: mikejo
manager: jmartens
ms.technology: vs-ide-debug
---
# marker_series::write_alert method

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Writes an alert to the Concurrency Visualizer trace file.

## Syntax

```cpp
void write_alert(
   _In_ LPCTSTR _Format,
   ...
);
```

#### Parameters
 `_Format`
 A composite format string that contains text intermixed with zero or more format items, which correspond to objects in the argument list.

## Requirements
 **Header:** *cvmarkersobj.h*

 **Namespace:** Concurrency::diagnostic

## See also
- [marker_series class](../profiling/marker-series-class.md)
