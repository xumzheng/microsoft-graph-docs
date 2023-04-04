---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = GetTotalAggregatedRemoteConnectionReportsPostRequestBody();
request_body.setTop(25);

request_body.setSkip(0);

request_body.setFilter('(TotalUsageInHour ge 40 and TotalUsageInHour le 80)');

request_body.setSelect(['CloudPcId', 'ManagedDeviceName', 'UserPrincipalName', 'TotalUsageInHour', 'DaysSinceLastSignIn', ]);



await client.deviceManagement.virtualEndpoint.reports.getTotalAggregatedRemoteConnectionReports.post(request_body);


```