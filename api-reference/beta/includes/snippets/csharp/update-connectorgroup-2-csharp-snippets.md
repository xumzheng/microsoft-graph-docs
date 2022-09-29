---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ConnectorGroup
{
	Name = "name-value",
	Region = ConnectorGroupRegion.Nam,
};
var result = await graphClient.OnPremisesPublishingProfiles["onPremisesPublishingProfile-id"].ConnectorGroups["connectorGroup-id"].PatchAsync(requestBody);


```