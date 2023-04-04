---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = Contact();
request_body.setParentFolderId('parentFolderId-value');

request_body.setBirthday(DateTime('datetime-value'));

request_body.setFileAs('fileAs-value');

request_body.setDisplayName('displayName-value');

request_body.setGivenName('givenName-value');

request_body.setInitials('initials-value');



result = await client.me.contactFoldersById('contactFolder-id').contacts.post(request_body);


```