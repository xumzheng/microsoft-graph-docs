---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.Education.Classes.Item.Assignments.Item.SetUpResourcesFolder.SetUpResourcesFolderPostRequestBody
{
};
var result = await graphClient.Education.Classes["educationClass-id"].Assignments["educationAssignment-id"].SetUpResourcesFolder.PostAsync(requestBody);


```