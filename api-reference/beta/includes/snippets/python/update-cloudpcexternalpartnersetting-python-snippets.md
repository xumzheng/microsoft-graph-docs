---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = CloudPcExternalPartnerSetting();
requestBody.set@odatatype('#microsoft.graph.cloudPcExternalPartnerSetting');

requestBody.setEnableConnection(true);



result = await client.deviceManagement().virtualEndpoint().externalPartnerSettingsById('cloudPcExternalPartnerSetting-id').patch(requestBody);


```