---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CloudPcExportJob()
request_body.ReportName(CloudPcReportName('totalaggregatedremoteconnectionreports'))

request_body.Select(['CloudPcId', 'ManagedDeviceName', 'UserPrincipalName', 'DaysSinceLastSignIn', 'TotalUsageInHour', ])




result = await client.deviceManagement.virtualEndpoint.reports.exportJobs.post(request_body = request_body)


```