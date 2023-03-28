---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new MembersPostRequestBody();
$additionalData = [
'@odata.type' => '#microsoft.graph.group', 
'description' => 'Self help community for golf', 
'displayName' => 'Golf Assist', 
'groupTypes' => ['Unified', ],
'mailEnabled' => true,
'mailNickname' => 'golfassist', 
'securityEnabled' => false,
];
$requestBody.setAdditionalData($additionalData);




$graphServiceClient.administrativeUnitsById('administrativeUnit-id').members().post($requestBody);


```