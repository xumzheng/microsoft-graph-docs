---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = SectionGroupsPostRequestBody();
additionalData = [
'displayName' => 'Section group name', 
];
requestBody.setAdditionalData(additionalData);




await client.me().onenote().sectionGroupsById('sectionGroup-id').sectionGroups().post(requestBody);


```