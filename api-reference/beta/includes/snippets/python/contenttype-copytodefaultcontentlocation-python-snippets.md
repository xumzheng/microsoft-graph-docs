---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = CopyToDefaultContentLocationPostRequestBody()
source_file = ItemReference()
source_file_sharepoint_ids = SharepointIds()
sourceFileSharepointIds.listId = 'e2ecf63b-b0fd-48f7-a54a-d8c15479e3b0'

sourceFileSharepointIds.listItemId = '2'


sourceFile.sharepoint_ids = sourceFileSharepointIds

request_body.source_file = sourceFile
request_body.destinationFileName = 'newname.txt'




await client.sites_by_id('site-id').contentTypes_by_id('contentType-id').copyToDefaultContentLocation.post(request_body = request_body)


```