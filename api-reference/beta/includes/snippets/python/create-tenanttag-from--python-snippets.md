---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = TenantTag()
request_body.setDisplayName('Support')

request_body.setDescription('Tenants that have purchased extended support')


request_config = TenantTagsRequestBuilderPostRequestConfiguration(
request_config = TenantTagsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.tenantRelationships.managedTenants.tenantTags.post(request_body, headers=)


```