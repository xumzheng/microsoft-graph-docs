---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

requestBody = MailFolder();
requestBody.set@odatatype('microsoft.graph.mailSearchFolder');

additionalData = [
'filterQuery' => 'contains(subject, \'Analytics\')', 
];
requestBody.setAdditionalData(additionalData);




result = await client.me().mailFoldersById('mailFolder-id').patch(requestBody);


```