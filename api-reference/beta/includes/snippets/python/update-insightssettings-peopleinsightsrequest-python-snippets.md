---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = InsightsSettings()
request_body.setIsEnabledInOrganization(true)

request_body.setDisabledForGroup('edbfe4fb-ec70-4300-928f-dbb2ae86c981')


request_config = PeopleInsightsRequestBuilderPatchRequestConfiguration(
request_config = PeopleInsightsRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.organization_by_id('organization-id').settings.peopleInsights.patch(request_body, headers=)


```