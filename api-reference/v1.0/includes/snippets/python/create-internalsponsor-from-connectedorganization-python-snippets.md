---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceCreate()
request_body.set@odataid('https://graph.microsoft.com/v1.0/users/{id}')



await client.identityGovernance_entitlementManagement_connectedOrganizationsby_id('connectedOrganization-id')_internalSponsors_ref.post(request_body)


```