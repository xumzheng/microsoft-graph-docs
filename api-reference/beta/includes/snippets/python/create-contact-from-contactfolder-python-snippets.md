---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = Contact();
requestBody.setParentFolderId('parentFolderId-value');

requestBody.setBirthday(DateTime('2016-10-19T10:37:00Z'));

requestBody.setFileAs('fileAs-value');

requestBody.setDisplayName('displayName-value');

requestBody.setGivenName('givenName-value');

requestBody.setInitials('initials-value');



result = await client.me().contactFoldersById('contactFolder-id').contacts().post(requestBody);


```