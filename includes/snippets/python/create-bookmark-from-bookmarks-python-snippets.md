---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = Bookmark();
requestBody.setDisplayName('Contoso Install Site');

requestBody.setWebUrl('http://www.contoso.com/');

requestBody.setDescription('Try or buy Contoso for Home or Business and view product information');

keywords = AnswerKeyword();
keywords.setKeywords(['Contoso', 'install', ]);

keywords.setReservedKeywords(['Contoso', ]);

keywords.setMatchSimilarKeywords(true);


requestBody.setKeywords($keywords);
requestBody.setState(AnswerState('published'));



requestResult = graphServiceClient.search().bookmarks().post(requestBody);


```