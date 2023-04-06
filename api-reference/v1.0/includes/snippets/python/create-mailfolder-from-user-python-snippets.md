---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = MailFolder()
request_body.setDisplayName('Clutter')

request_body.setIsHidden(true)


request_config = MailFoldersRequestBuilderPostRequestConfiguration(
request_config = MailFoldersRequestBuilderPostRequestConfiguration(query_params=)


result = await client.me.mailFolders.post(request_body, headers=)


```