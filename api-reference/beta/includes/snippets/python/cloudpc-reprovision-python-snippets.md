---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ReprovisionPostRequestBody();
requestBody.setUserAccountType(CloudPcUserAccountType('administrator'));

requestBody.setOsVersion(CloudPcOperatingSystem('windows10'));



awaitclient.deviceManagement().virtualEndpoint().cloudPCsById('cloudPC-id').reprovision().post(requestBody);


```