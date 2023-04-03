---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = MailFolder();
requestBody.set@odatatype('microsoft.graph.mailSearchFolder');

requestBody.setDisplayName('Weekly digests');

additionalData = [
'includeNestedFolders' => true,
'sourceFolderIds' => ['AQMkADYAAAIBDAAAAA==', ],
'filterQuery' => 'contains(subject, \'weekly digest\')', 
];
requestBody.setAdditionalData(additionalData);




result = awaitclient.me().mailFoldersById('mailFolder-id').childFolders().post(requestBody);


```