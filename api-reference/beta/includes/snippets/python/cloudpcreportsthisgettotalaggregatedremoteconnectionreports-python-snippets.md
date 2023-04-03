---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = GetTotalAggregatedRemoteConnectionReportsPostRequestBody();
requestBody.setTop(25);

requestBody.setSkip(0);

requestBody.setFilter('(TotalUsageInHour ge 40 and TotalUsageInHour le 80)');

requestBody.setSelect(['CloudPcId', 'ManagedDeviceName', 'UserPrincipalName', 'TotalUsageInHour', 'DaysSinceLastSignIn', ]);



await client.deviceManagement().virtualEndpoint().reports().getTotalAggregatedRemoteConnectionReports().post(requestBody);


```