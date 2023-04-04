---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = MembersPostRequestBody();
additionalData = [
'@odata.type' => '#microsoft.graph.group', 
'description' => 'Self help community for golf', 
'displayName' => 'Golf Assist', 
'groupTypes' => ['Unified', ],
'mailEnabled' => true,
'mailNickname' => 'golfassist', 
'securityEnabled' => false,
];
request_body.setAdditionalData(additionalData);




await client.directory.administrativeUnitsById('administrativeUnit-id').members.post(request_body);


```