---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PronounsSettings()
request_body.setIsEnabledInOrganization(true)



result = await client.organizationby_id('organization-id')_settings_pronouns.patch(request_body)


```