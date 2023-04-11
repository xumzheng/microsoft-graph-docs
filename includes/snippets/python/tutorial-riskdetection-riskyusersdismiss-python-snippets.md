---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DismissPostRequestBody()
request_body.UserIds(['4628e7df-dff3-407c-a08f-75f08c0806dc', ])



request_configuration = DismissRequestBuilderPostRequestConfiguration(
)


await client.identityProtection.riskyUsers.dismiss.post(request_body = request_body)


```