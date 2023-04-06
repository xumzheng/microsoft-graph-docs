---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ContactFolder()
request_body.setParentFolderId('parentFolderId-value')

request_body.setDisplayName('displayName-value')


request_config = ContactFolderRequestBuilderPatchRequestConfiguration(
request_config = ContactFolderRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.me.contactFolders_by_id('contactFolder-id').patch(request_body, headers=)


```