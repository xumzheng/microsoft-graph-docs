---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new SitePage();
$requestBody->set@odatatype('#microsoft.graph.sitePage');

$requestBody->setTitle('sample');

$requestBody->setShowComments(true);

$requestBody->setShowRecommendedPages(false);



$requestResult = $graphServiceClient->sitesById('site-id')->pagesById('sitePage-id')->patch($requestBody);


```