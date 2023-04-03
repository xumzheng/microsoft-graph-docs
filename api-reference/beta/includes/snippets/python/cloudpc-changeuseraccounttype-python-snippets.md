---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = ChangeUserAccountTypePostRequestBody();
requestBody.setUserAccountType(CloudPcUserAccountType('administrator'));



await client.deviceManagement().virtualEndpoint().cloudPCsById('cloudPC-id').changeUserAccountType().post(requestBody);


```