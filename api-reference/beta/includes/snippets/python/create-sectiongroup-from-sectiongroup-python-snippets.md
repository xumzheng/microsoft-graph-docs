---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new SectionGroupsPostRequestBody();
$additionalData = [
'displayName' => 'Section group name', 
];
$requestBody.setAdditionalData($additionalData);




$graphServiceClient.me().onenote().sectionGroupsById('sectionGroup-id').sectionGroups().post($requestBody);


```