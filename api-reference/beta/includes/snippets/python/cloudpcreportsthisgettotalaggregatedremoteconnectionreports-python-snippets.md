---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetTotalAggregatedRemoteConnectionReportsPostRequestBody()
request_body.top = 25

request_body.skip = 0

request_body.filter = '(TotalUsageInHour ge 40 and TotalUsageInHour le 80)'

request_body.Select(['CloudPcId', 'ManagedDeviceName', 'UserPrincipalName', 'TotalUsageInHour', 'DaysSinceLastSignIn', ])



request_configuration = GetTotalAggregatedRemoteConnectionReportsRequestBuilderPostRequestConfiguration(
)


await client.deviceManagement.virtualEndpoint.reports.getTotalAggregatedRemoteConnectionReports.post(request_body = request_body)


```