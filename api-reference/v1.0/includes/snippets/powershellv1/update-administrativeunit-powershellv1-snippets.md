---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv1

Import-Module Microsoft.Graph.Identity.DirectoryManagement

$params = @{
	DisplayName = "Greater Seattle District Technical Schools"
}

Update-MgDirectoryAdministrativeUnit -AdministrativeUnitId $administrativeUnitId -BodyParameter $params

```