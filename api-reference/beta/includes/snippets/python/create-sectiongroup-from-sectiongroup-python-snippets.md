---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = SectionGroupsPostRequestBody()
additionalData = [
'displayName' => 'Section group name', 
];
request_body.additionaldata(additionalData)




request_configuration = SectionGroupsRequestBuilderPostRequestConfiguration(
)


await client.me.onenote.sectionGroups_by_id('sectionGroup-id').sectionGroups.post(request_body = request_body)


```