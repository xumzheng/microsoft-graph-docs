---
description: "Automatically generated file. DO NOT MODIFY"
---

```csharp

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
var graphClient = new GraphServiceClient(requestAdapter);

var requestBody = new Microsoft.Graph.Beta.DeviceManagement.VirtualEndpoint.Reports.GetTotalAggregatedRemoteConnectionReports.GetTotalAggregatedRemoteConnectionReportsPostRequestBody
{
	Top = 25,
	Skip = 0,
	Filter = "(TotalUsageInHour ge 40 and TotalUsageInHour le 80)",
	Select = new List<string>
	{
		"CloudPcId",
		"ManagedDeviceName",
		"UserPrincipalName",
		"TotalUsageInHour",
		"DaysSinceLastSignIn",
	},
};
await graphClient.DeviceManagement.VirtualEndpoint.Reports.GetTotalAggregatedRemoteConnectionReports.PostAsync(requestBody);


```