---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = GetDailyAggregatedRemoteConnectionReportsPostRequestBody();
requestBody.setFilter('CloudPcId eq \'5db15afe-025d-4f1b-b43a-d0554b63ffff\' and RoundTripTimeInMsP50 lt 100 and EventDateTime gt 2022-06-01 ');

requestBody.setSearch('abc0907');

requestBody.setSelect(['EventDateTime', 'CloudPcId', 'ManagedDeviceName', 'UsageInHour', 'RoundTripTimeInMsP50', 'AvailableBandwidthInMBpsP50', 'RemoteSignInTimeInSecP50', 'UserPrincipalName', ]);

requestBody.setSkip(0);

requestBody.setTop(25);



awaitclient.deviceManagement().virtualEndpoint().reports().getDailyAggregatedRemoteConnectionReports().post(requestBody);


```