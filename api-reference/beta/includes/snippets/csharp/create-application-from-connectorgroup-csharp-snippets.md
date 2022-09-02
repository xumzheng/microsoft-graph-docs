---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ReferenceUpdate
{
	OdataId = "https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}",
};
await graphClient.Applications["application-id"].ConnectorGroup.Ref.PutAsync(requestBody);


```