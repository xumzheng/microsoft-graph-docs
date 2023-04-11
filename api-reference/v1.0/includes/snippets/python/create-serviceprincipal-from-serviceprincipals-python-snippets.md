---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ServicePrincipal()
request_body.appId = '65415bb1-9267-4313-bbf5-ae259732ee12'



request_configuration = ServicePrincipalsRequestBuilderPostRequestConfiguration(
)


result = await client.servicePrincipals.post(request_body = request_body)


```