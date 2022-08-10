---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new PrintTaskTrigger
{
	Event = PrintEvent.Jobstarted,
	AdditionalData = new Dictionary<string, object>
	{
		{
			"definition@odata.bind" , "https://graph.microsoft.com/v1.0/print/taskDefinitions/{taskDefinitionId}"
		},
	},
};
var result = await graphClient.Print.Printers["printer-id"].TaskTriggers.PostAsync(requestBody);


```