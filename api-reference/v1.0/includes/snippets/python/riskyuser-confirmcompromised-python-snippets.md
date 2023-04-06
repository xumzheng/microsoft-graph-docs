---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConfirmCompromisedPostRequestBody()
request_body.setUserIds(['29f270bb-4d23-4f68-8a57-dc73dc0d4caf', '20f91ec9-d140-4d90-9cd9-f618587a1471', ])


request_config = ConfirmCompromisedRequestBuilderPostRequestConfiguration(
request_config = ConfirmCompromisedRequestBuilderPostRequestConfiguration(query_params=)


await client.identityProtection.riskyUsers.confirmCompromised.post(request_body, headers=)


```