---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Bookmark()
request_body.displayName = 'Contoso Install Site'

request_body.webUrl = 'http://www.contoso.com/'

request_body.description = 'Try or buy Contoso for Home or Business and view product information'

keywords = AnswerKeyword()
keywords.Keywords(['Contoso', 'install', ])

keywords.ReservedKeywords(['Contoso', ])

keywords.match_similar_keywords = True


request_body.keywords = keywords
request_body.State(AnswerState('published'))




result = await client.search.bookmarks.post(request_body = request_body)


```