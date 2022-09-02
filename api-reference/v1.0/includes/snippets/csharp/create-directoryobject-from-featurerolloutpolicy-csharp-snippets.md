---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ReferenceCreate
{
	OdataId = "https://graph.microsoft.com/v1.0/directoryObjects/2441b489-4f12-4882-b039-8f6006bd66da",
};
await graphClient.Policies.FeatureRolloutPolicies["featureRolloutPolicy-id"].AppliesTo.Ref.PostAsync(requestBody);


```