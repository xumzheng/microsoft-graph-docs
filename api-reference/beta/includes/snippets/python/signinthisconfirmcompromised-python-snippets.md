---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConfirmCompromisedPostRequestBody()
request_body.RequestIds(['f01c6af6-6683-4a37-a945-0a925501eede', '42bf60ac-d0cb-4206-aa5c-101884298f55', 'f09c8f14-8d8e-42cf-8a7e-732b0594e79b', ])



request_configuration = ConfirmCompromisedRequestBuilderPostRequestConfiguration(
)


await client.auditLogs.signIns.confirmCompromised.post(request_body = request_body)


```