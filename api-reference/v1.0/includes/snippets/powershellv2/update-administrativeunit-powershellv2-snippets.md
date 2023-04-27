---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
	displayName = "Greater Seattle District Technical Schools"
}

Update-MgDirectoryAdministrativeUnit -AdministrativeUnitId $administrativeUnitId -BodyParameter $params

```