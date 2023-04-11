---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceCreate()
request_body.@odataid = 'https://graph.microsoft.com/v1.0/users/{id}'



request_configuration = RefRequestBuilderPostRequestConfiguration(
)


await client.identityGovernance.entitlementManagement.connectedOrganizations_by_id('connectedOrganization-id').externalSponsors.ref.post(request_body = request_body)


```