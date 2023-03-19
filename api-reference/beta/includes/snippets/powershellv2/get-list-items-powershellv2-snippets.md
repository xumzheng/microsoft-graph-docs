---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Beta.Sites

Get-MgBetaSiteListItem -SiteId $siteId -ListId $listId -ExpandProperty "fields(select=Name,Color,Quantity)" 

```