---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Groups

Get-MgGroup -Filter "graphlearn_courses/courseId eq ‘123’" -Property "displayName,id,description,graphlearn_courses" 

```