---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = InsightsSettings()
request_body.isEnabledInOrganization = true

request_body.disabledForGroup = 'edbfe4fb-ec70-4300-928f-dbb2ae86c981'



request_configuration = ContactInsightsRequestBuilderPatchRequestConfiguration(
)


result = await client.organization_by_id('organization-id').settings.contactInsights.patch(request_body = request_body)


```