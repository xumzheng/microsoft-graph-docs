---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ContactFolder()
request_body.setParentFolderId('AQMkADIxYjJiYgEzLTFmNjYALTRjYTMtODA1NC0wZDkxZGNmOTcxNTQALgAAA8RJzXYaLKZPlmn0ge0edZkBADa3qi2IMXRNg6RwQSHe_F8AAAIBDgAAAA==')

request_body.setDisplayName('Important contacts')


request_config = ContactFoldersRequestBuilderPostRequestConfiguration(
request_config = ContactFoldersRequestBuilderPostRequestConfiguration(query_params=)


result = await client.me.contactFolders.post(request_body, headers=)


```