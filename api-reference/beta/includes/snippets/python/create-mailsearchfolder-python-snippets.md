---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MailFolder()
request_body.set@odatatype('microsoft.graph.mailSearchFolder')

request_body.setDisplayName('Weekly digests')

additionalData = [
'includeNestedFolders' => true,
'sourceFolderIds' => ['AQMkADYAAAIBDAAAAA==', ],
'filterQuery' => 'contains(subject, \'weekly digest\')', 
];
request_body.setAdditionalData(additionalData)




result = await client.me_mailFoldersby_id('mailFolder-id')_childFolders.post(request_body)


```