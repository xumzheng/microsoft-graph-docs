---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = FollowedSite()
additionalData = [
'value' => value1 = ()
		value1.id = 'contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,712a596e-90a1-49e3-9b48-bfa80bee8740'


valueArray []= value1;
value2 = ()
		value2.id = 'contoso.sharepoint.com,da60e844-ba1d-49bc-b4d4-d5e36bae9019,0271110f-634f-4300-a841-3a8a2e851851'


valueArray []= value2;
request_body.value(valueArray)


];
request_body.additionaldata(additionalData)





await client.users_by_id('user-id').followedSites_by_id('site-id').post(request_body = request_body)


```