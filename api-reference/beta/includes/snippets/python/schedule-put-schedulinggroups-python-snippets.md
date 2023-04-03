---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = SchedulingGroup();
additionalData = [
'displayName' => 'Cashiers', 
'isActive' => true,
'userIds' => ['c5d0c76b-80c4-481c-be50-923cd8d680a1', '2a4296b3-a28a-44ba-bc66-0274b9b95851', ],
];
requestBody.setAdditionalData(additionalData);



request_config = SchedulingGroupRequestBuilderPutRequestConfiguration();

headers = [
'Prefer' => 'return=representation',
];

request_config.headers = headers;


await client.teamsById('team-id').schedule().schedulingGroupsById('schedulingGroup-id').put(requestBody, request_config);


```