---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = CopyToDefaultContentLocationPostRequestBody();
sourceFile = ItemReference();
sourceFileSharepointIds = SharepointIds();
sourceFileSharepointIds.setListId('e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0');

sourceFileSharepointIds.setListItemId('2');


sourceFile.setSharepointIds($sourceFileSharepointIds);

request_body.setSourceFile($sourceFile);
request_body.setDestinationFileName('newname.txt');



await client.sitesById('site-id').contentTypesById('contentType-id').copyToDefaultContentLocation.post(request_body);


```