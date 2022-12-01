---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new AdminReportSettings
{
	DisplayConcealedNames = true,
};
var result = await graphClient.Admin.ReportSettings.PatchAsync(requestBody);


```