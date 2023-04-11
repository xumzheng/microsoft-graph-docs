---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ContactFolder()
request_body.parentFolderId = 'parentFolderId-value'

request_body.displayName = 'displayName-value'



request_configuration = ContactFolderRequestBuilderPatchRequestConfiguration(
)


result = await client.me.contactFolders_by_id('contactFolder-id').patch(request_body = request_body)


```