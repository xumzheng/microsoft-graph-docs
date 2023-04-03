---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = CloudPcExternalPartnerSetting();
requestBody.set@odatatype('#microsoft.graph.cloudPcExternalPartnerSetting');

requestBody.setEnableConnection(true);



requestResult = graphServiceClient.deviceManagement().virtualEndpoint().externalPartnerSettingsById('cloudPcExternalPartnerSetting-id').patch(requestBody);


```