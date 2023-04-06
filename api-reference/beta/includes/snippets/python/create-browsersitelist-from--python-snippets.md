---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BrowserSiteList()
request_body.setDisplayName('Production Site List A')

request_body.setDescription('Production site list for team A')


request_config = SiteListsRequestBuilderPostRequestConfiguration(
request_config = SiteListsRequestBuilderPostRequestConfiguration(query_params=)


result = await client.admin.edge.internetExplorerMode.siteLists.post(request_body, headers=)


```