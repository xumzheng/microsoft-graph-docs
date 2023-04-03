---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = ChangeUserAccountTypePostRequestBody();
requestBody.setUserAccountType(CloudPcUserAccountType('administrator'));



graphServiceClient.deviceManagement().virtualEndpoint().cloudPCsById('cloudPC-id').changeUserAccountType().post(requestBody);


```