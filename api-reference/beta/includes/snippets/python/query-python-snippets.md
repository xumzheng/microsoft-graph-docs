---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Query_post_request_body()
requests_search_request1 = Search_request()
requests_search_request1.EntityTypes([requests_search_request1.entitytype(EntityType.ExternalItem('entitytype.externalitem'))
])

requests_search_request1.ContentSources(['/external/connections/connectionfriendlyname', ])

requests_search_request1query = Search_query()
requests_search_request1query.query_string = 'contoso product'


requests_search_request1.query = requests_search_request1query
requests_search_request1.From = 0

requests_search_request1.Size = 25

requests_search_request1.Fields(['title', 'description', ])


requestsArray []= requestsSearchRequest1;
request_body.requests(requestsArray)





result = await client.search.query.post(request_body = request_body)


```