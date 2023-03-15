---
description: "Automatically generated file. DO NOT MODIFY"
---

```powershellv2

Import-Module Microsoft.Graph.Teams

Get-MgChatInstalledApp -ChatId $chatId -ExpandProperty "teamsAppDefinition(`$expand=bot)" 

```