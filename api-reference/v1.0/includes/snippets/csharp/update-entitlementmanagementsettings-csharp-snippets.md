---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new EntitlementManagementSettings
{
	ExternalUserLifecycleAction = AccessPackageExternalUserLifecycleAction.None,
};
await graphClient.IdentityGovernance.EntitlementManagement.Settings.PatchAsync(requestBody);


```