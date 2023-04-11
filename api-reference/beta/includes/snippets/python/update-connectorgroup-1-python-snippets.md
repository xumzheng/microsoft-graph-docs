---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ConnectorGroup()
request_body.name = 'Connector Group Demo'



request_configuration = ConnectorGroupsRequestBuilderPostRequestConfiguration(
)


result = await client.onPremisesPublishingProfiles_by_id('onPremisesPublishingProfile-id').connectorGroups.post(request_body = request_body)


```