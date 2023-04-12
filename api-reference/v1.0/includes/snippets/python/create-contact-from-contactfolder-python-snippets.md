---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Contact()
request_body.parentFolderId = 'parentFolderId-value'

request_body.birthday = DateTime('datetime-value')

request_body.fileAs = 'fileAs-value'

request_body.displayName = 'displayName-value'

request_body.givenName = 'givenName-value'

request_body.initials = 'initials-value'




result = await client.me.contactFolders_by_id('contactFolder-id').contacts.post(request_body = request_body)


```