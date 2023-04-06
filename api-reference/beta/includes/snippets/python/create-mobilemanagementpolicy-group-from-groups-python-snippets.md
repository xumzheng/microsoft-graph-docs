---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ReferenceCreate()
request_body.set@odataid('https://graph.microsoft.com/odata/groups(\'1a9db3ab-0acf-4808-99ae-e8ed581cb2e0\')')


request_config = RefRequestBuilderPostRequestConfiguration(
request_config = RefRequestBuilderPostRequestConfiguration(query_params=)


await client.policies.mobileAppManagementPolicies_by_id('mobilityManagementPolicy-id').includedGroups.ref.post(request_body, headers=)


```