---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CloudPcExportJob();
requestBody.setReportName(CloudPcReportName('totalaggregatedremoteconnectionreports'));

requestBody.setSelect(['CloudPcId', 'ManagedDeviceName', 'UserPrincipalName', 'DaysSinceLastSignIn', 'TotalUsageInHour', ]);



result = await client.deviceManagement().virtualEndpoint().reports().exportJobs().post(requestBody);


```