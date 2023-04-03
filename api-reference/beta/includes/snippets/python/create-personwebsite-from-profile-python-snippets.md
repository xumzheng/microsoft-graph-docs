---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = PersonWebsite();
requestBody.setCategories(['football', ]);

requestBody.setDisplayName('Lyn Damer');

requestBody.setWebUrl('www.lyndamer.no');



result = awaitclient.me().profile().websites().post(requestBody);


```