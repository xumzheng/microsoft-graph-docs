---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = SectionGroupsPostRequestBody();
additionalData = [
'displayName' => 'Section group name', 
];
requestBody.setAdditionalData(additionalData);




awaitclient.me().onenote().sectionGroupsById('sectionGroup-id').sectionGroups().post(requestBody);


```