---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ReprovisionPostRequestBody();
requestBody.setUserAccountType(CloudPcUserAccountType('administrator'));

requestBody.setOsVersion(CloudPcOperatingSystem('windows10'));



await client.deviceManagement().virtualEndpoint().cloudPCsById('cloudPC-id').reprovision().post(requestBody);


```