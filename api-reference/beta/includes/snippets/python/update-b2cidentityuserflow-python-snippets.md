---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = B2cIdentityUserFlow()
request_body.isLanguageCustomizationEnabled = true

request_body.defaultLanguageTag = 'en'



request_configuration = B2cIdentityUserFlowRequestBuilderPatchRequestConfiguration(
)


result = await client.identity.b2cUserFlows_by_id('b2cIdentityUserFlow-id').patch(request_body = request_body)


```