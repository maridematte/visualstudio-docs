---
title: CPPClean Task
description: This article describes the CPPClean task, which is used to delete the temporary files that MSBuild creates when a C++ project is built.
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- vc.task.cppclean
dev_langs:
- VB
- CSharp
- C++
- C++
helpviewer_keywords:
- MSBuild (C++), CPPClean task
- CPPClean task (MSBuild (C++))
author: ghogen
ms.author: ghogen
manager: jmartens
ms.technology: msbuild
---
# CPPClean Task

Deletes the temporary files that MSBuild creates when a C++ project is built. The process of deleting build files is known as *cleaning*.

## Parameters

 The following table describes the parameters of the **CPPClean** task.

|Parameter|Description|
|---------------|-----------------|
|**DeletedFiles**|Optional `ITaskItem[]` output parameter.<br /><br /> Defines an array of MSBuild output file items that can be consumed and emitted by tasks.|
|**DoDelete**|Optional **Boolean** parameter.<br /><br /> If `true`, clean temporary build files.|
|**FilePatternsToDeleteOnClean**|Required `String` parameter.<br /><br /> Specifies a semicolon-delimited list of file extensions of files to clean.|
|**FilesExcludedFromClean**|Optional `String` parameter.<br /><br /> Specifies a semicolon-delimited list of files not to clean.|
|**FoldersToClean**|Required `String` parameter.<br /><br /> Specifies a semicolon-delimited list of directories to clean. You can specify a full or a relative path, and the path can contain the wildcard symbol (*).|

## See also

- [Task reference](../msbuild/msbuild-task-reference.md)
