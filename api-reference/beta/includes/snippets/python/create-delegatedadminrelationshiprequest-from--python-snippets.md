---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DelegatedAdminRelationshipRequest()
request_body.setAction(DelegatedAdminRelationshipRequestAction('lockforapproval'))


request_config = RequestsRequestBuilderPostRequestConfiguration(
request_config = RequestsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.tenantRelationships.delegatedAdminRelationships_by_id('delegatedAdminRelationship-id').requests.post(request_body, headers=)


```