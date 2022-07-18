---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new CustomAccessPackageWorkflowExtension
{
	DisplayName = "test_action_0124",
	Description = "this is for graph testing only",
	EndpointConfiguration = new CustomExtensionEndpointConfiguration
	{
		@odata.type = "#microsoft.graph.logicAppTriggerEndpointConfiguration",
		AdditionalData = new()
		{
			{"subscriptionId", "38ab2ccc-3747-4567-b36b-9478f5602f0d"},
			{"resourceGroupName", "EMLogicApp"},
			{"logicAppWorkflowName", "customextension_test"},
		}
	},
	AuthenticationConfiguration = new CustomExtensionAuthenticationConfiguration
	{
		@odata.type = "#microsoft.graph.azureAdTokenAuthentication",
		AdditionalData = new()
		{
			{"resourceId", "f604bd15-f785-4309-ad7c-6fad18ddb6cb"},
		}
	},
};
var result = await graphClient.IdentityGovernance.EntitlementManagement.AccessPackageCatalogs["accessPackageCatalog-id"].CustomAccessPackageWorkflowExtensions.PostAsync(requestBody);


```