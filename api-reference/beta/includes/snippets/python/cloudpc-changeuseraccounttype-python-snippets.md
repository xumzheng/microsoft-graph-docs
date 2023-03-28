---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ChangeUserAccountTypePostRequestBody();
$requestBody.setUserAccountType(new CloudPcUserAccountType('administrator'));



$graphServiceClient.deviceManagement().virtualEndpoint().cloudPCsById('cloudPC-id').changeUserAccountType().post($requestBody);


```