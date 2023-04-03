---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Contact();
requestBody.setParentFolderId('parentFolderId-value');

requestBody.setBirthday(DateTime('datetime-value'));

requestBody.setFileAs('fileAs-value');

requestBody.setDisplayName('displayName-value');

requestBody.setGivenName('givenName-value');

requestBody.setInitials('initials-value');



requestResult = graphServiceClient.me().contactFoldersById('contactFolder-id').contacts().post(requestBody);


```