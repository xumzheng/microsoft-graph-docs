---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = WorkbookCommentReply()
request_body.content = 'This is my reply to the comment.'

request_body.contentType = 'plain'




result = await client.drives_by_id('drive-id').items_by_id('driveItem-id').workbook.comments_by_id('workbookComment-id').replies.post(request_body = request_body)


```