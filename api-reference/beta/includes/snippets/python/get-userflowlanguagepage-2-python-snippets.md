---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)


request_configuration = OverridesPagesRequestBuilderGetRequestConfiguration(
)


result = await client.identity.b2cUserFlows_by_id('b2cIdentityUserFlow-id').languages_by_id('userFlowLanguageConfiguration-id').overridesPages.get()


```