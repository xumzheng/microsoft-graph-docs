---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SchedulingGroup()
additionalData = [
'displayName' => 'Cashiers', 
'isActive' => true,
'userIds' => ['c5d0c76b-80c4-481c-be50-923cd8d680a1', '2a4296b3-a28a-44ba-bc66-0274b9b95851', ],
];
request_body.setAdditionalData(additionalData)



request_configuration = SchedulingGroupRequestBuilderPutRequestConfiguration(
request_configuration = SchedulingGroupRequestBuilderPutRequestConfiguration(query_params=)
System.Collections.Generic.List`1[System.Tuple`2[System.String,System.String]])


await client.teams_by_id('team-id').schedule.schedulingGroups_by_id('schedulingGroup-id').put(request_body, request_configuration)


```