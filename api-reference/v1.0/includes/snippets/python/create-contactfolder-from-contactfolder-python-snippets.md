---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ContactFolder()
request_body.displayName = 'Family'



request_configuration = ChildFoldersRequestBuilderPostRequestConfiguration(
)


result = await client.me.contactFolders_by_id('contactFolder-id').childFolders.post(request_body = request_body)


```