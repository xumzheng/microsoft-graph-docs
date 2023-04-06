---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CopyToSectionPostRequestBody()
request_body.setId('id-value')

request_body.setGroupId('groupId-value')


request_config = CopyToSectionRequestBuilderPostRequestConfiguration(
request_config = CopyToSectionRequestBuilderPostRequestConfiguration(query_params=)


result = await client.me.onenote.pages_by_id('onenotePage-id').copyToSection.post(request_body, headers=)


```