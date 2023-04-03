---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = ChangeUserAccountTypePostRequestBody();
requestBody.setUserAccountType(CloudPcUserAccountType('administrator'));



awaitclient.deviceManagement().virtualEndpoint().cloudPCsById('cloudPC-id').changeUserAccountType().post(requestBody);


```