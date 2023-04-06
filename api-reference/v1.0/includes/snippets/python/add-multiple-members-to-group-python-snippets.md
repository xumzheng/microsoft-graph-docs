---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Group()
additionalData = [
'members@odata.bind' => ['https://graph.microsoft.com/v1.0/directoryObjects/{id}', 'https://graph.microsoft.com/v1.0/directoryObjects/{id}', 'https://graph.microsoft.com/v1.0/directoryObjects/{id}', ],
];
request_body.setAdditionalData(additionalData)



request_config = GroupRequestBuilderPatchRequestConfiguration(
request_config = GroupRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.groups_by_id('group-id').patch(request_body, headers=)


```