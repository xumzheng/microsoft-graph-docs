---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetDailyAggregatedRemoteConnectionReportsPostRequestBody()
request_body.setFilter('CloudPcId eq \'5db15afe-025d-4f1b-b43a-d0554b63ffff\' and RoundTripTimeInMsP50 lt 100 and EventDateTime gt 2022-06-01 ')

request_body.setSearch('abc0907')

request_body.setSelect(['EventDateTime', 'CloudPcId', 'ManagedDeviceName', 'UsageInHour', 'RoundTripTimeInMsP50', 'AvailableBandwidthInMBpsP50', 'RemoteSignInTimeInSecP50', 'UserPrincipalName', ])

request_body.setSkip(0)

request_body.setTop(25)



await client.deviceManagement.virtualEndpoint.reports.getDailyAggregatedRemoteConnectionReports.post(request_body, headers=)


```