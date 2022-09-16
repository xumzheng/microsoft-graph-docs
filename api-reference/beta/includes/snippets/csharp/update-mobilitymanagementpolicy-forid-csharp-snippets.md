---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new MobilityManagementPolicy
{
	OdataType = "#microsoft.graph.mobilityManagementPolicy",
	ComplianceUrl = "https://portal.uem.contoso.com/?portalAction=Compliance",
	DiscoveryUrl = "https://enrollment.uem.contoso.com/enrollmentserver/discovery.svc",
	TermsOfUseUrl = "https://portal.uem.contoso.com/TermsofUse.aspx",
};
await graphClient.Policies.MobileDeviceManagementPolicies["mobilityManagementPolicy-id"].PatchAsync(requestBody);


```