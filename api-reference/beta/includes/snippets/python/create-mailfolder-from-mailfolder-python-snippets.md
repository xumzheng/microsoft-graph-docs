---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MailFolder()
request_body.setDisplayName('displayName-value')

request_body.setIsHidden(true)


request_config = ChildFoldersRequestBuilderPostRequestConfiguration(
request_config = ChildFoldersRequestBuilderPostRequestConfiguration(query_params=)


result = await client.me.mailFolders_by_id('mailFolder-id').childFolders.post(request_body, headers=)


```