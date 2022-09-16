---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new InternalDomainFederation
{
	DisplayName = "Contoso name change",
	FederatedIdpMfaBehavior = FederatedIdpMfaBehavior.AcceptIfMfaDoneByFederatedIdp,
};
await graphClient.Domains["domain-id"].FederationConfiguration["internalDomainFederation-id"].PatchAsync(requestBody);


```