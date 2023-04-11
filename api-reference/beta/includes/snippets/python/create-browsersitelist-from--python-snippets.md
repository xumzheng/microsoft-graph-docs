---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BrowserSiteList()
request_body.displayName = 'Production Site List A'

request_body.description = 'Production site list for team A'



request_configuration = SiteListsRequestBuilderPostRequestConfiguration(
)


result = await client.admin.edge.internetExplorerMode.siteLists.post(request_body = request_body)


```