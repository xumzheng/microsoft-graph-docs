---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = GetRemoteConnectionHistoricalReportsPostRequestBody()
request_body.filter = 'CloudPcId eq \'40f9315c-5b63-4126-9f89-b7dcb14fffff\' and SignInDateTime gt datetime\'2022-09-09T01:22:51.849Z\''

request_body.Select(['SignInDateTime', 'SignOutDateTime', 'UsageInHour', 'RoundTripTimeInMsP50', 'AvailableBandwidthInMBpsP50', 'RemoteSignInTimeInSec', ])

request_body.top = 25

request_body.skip = 0




await client.deviceManagement.virtualEndpoint.reports.getRemoteConnectionHistoricalReports.post(request_body = request_body)


```