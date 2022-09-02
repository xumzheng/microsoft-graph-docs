---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new ReferenceCreate
{
	OdataId = "https://graph.microsoft.com/v1.0/education/users/13015",
};
await graphClient.Education.Classes["educationClass-id"].Members.Ref.PostAsync(requestBody);


```