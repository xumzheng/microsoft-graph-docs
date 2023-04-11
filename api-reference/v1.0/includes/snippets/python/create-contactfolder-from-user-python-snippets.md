---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ContactFolder()
request_body.parentFolderId = 'AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA=='

request_body.displayName = 'Important contacts'



request_configuration = ContactFoldersRequestBuilderPostRequestConfiguration(
)


result = await client.me.contactFolders.post(request_body = request_body)


```