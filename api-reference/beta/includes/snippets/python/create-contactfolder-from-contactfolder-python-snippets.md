---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ContactFolder()
request_body.setDisplayName('Family')



result = await client.me.contactFoldersById('contactFolder-id').childFolders.post(request_body)


```