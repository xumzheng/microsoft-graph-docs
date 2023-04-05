---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ChangeUserAccountTypePostRequestBody()
request_body.setUserAccountType(CloudPcUserAccountType('administrator'))



await client.deviceManagement_virtualEndpoint_cloudPCsby_id('cloudPC-id')_changeUserAccountType.post(request_body)


```