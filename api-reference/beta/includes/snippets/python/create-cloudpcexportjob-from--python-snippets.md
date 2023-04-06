---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CloudPcExportJob()
request_body.setReportName(CloudPcReportName('totalaggregatedremoteconnectionreports'))

request_body.setSelect(['CloudPcId', 'ManagedDeviceName', 'UserPrincipalName', 'DaysSinceLastSignIn', 'TotalUsageInHour', ])


request_config = ExportJobsRequestBuilderPostRequestConfiguration(
request_config = ExportJobsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.deviceManagement.virtualEndpoint.reports.exportJobs.post(request_body, headers=)


```