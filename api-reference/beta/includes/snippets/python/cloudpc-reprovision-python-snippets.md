---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ReprovisionPostRequestBody();
requestBody.setUserAccountType(CloudPcUserAccountType('administrator'));

requestBody.setOsVersion(CloudPcOperatingSystem('windows10'));



graphServiceClient.deviceManagement().virtualEndpoint().cloudPCsById('cloudPC-id').reprovision().post(requestBody);


```