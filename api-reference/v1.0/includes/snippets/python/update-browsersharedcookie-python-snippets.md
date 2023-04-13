---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = BrowserSharedCookie()
request_body.hostOrDomain = 'www.microsoft.com'

request_body.SourceEnvironment(BrowserSharedCookieSourceEnvironment('microsoftedge'))

request_body.displayName = 'Microsoft Cookie'

request_body.path = '/'

request_body.host_only = True

request_body.comment = 'Updating source environment.'




result = await client.admin.edge.internetExplorerMode.siteLists_by_id('browserSiteList-id').sharedCookies_by_id('browserSharedCookie-id').patch(request_body = request_body)


```