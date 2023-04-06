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
request_body.setAdditionalData(additionalData)



request_config = SectionGroupsRequestBuilderPostRequestConfiguration(
request_config = SectionGroupsRequestBuilderPostRequestConfiguration(query_params=)


await client.me.onenote.sectionGroups_by_id('sectionGroup-id').sectionGroups.post(request_body, headers=)


```