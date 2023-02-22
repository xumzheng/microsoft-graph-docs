---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var teamsAppSettings = new TeamsAppSettings
{
	AllowUserRequestsForAppAccess = true
};

await graphClient.Teamwork.TeamsAppSettings
	.Request()
	.UpdateAsync(teamsAppSettings);

```