---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

GraphServiceClient graphClient = new GraphServiceClient( authProvider );

var application = new Application
{
	AppRoles = new List<AppRole>()
	{
		new AppRole
		{
			AllowedMemberTypes = new List<String>()
			{
				"User",
				"Application"
			},
			Description = "Survey.Read",
			DisplayName = "Survey.Read",
			Id = Guid.Parse("7a9ddfc4-cc8a-48ea-8275-8ecbffffd5a0"),
			IsEnabled = false,
			Origin = "Application",
			Value = "Survey.Read"
		}
	}
};

await graphClient.Applications["{application-id}"]
	.Request()
	.UpdateAsync(application);

```