---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY$requestBody = new ItemPatent();
$requestBody.setDescription('Calculating the intent of a user to purchase an item based on the amount of time they hover their mouse over a given pixel.');

$requestBody.setDisplayName('Inferring User Intent through browsing behaviors');

$requestBody.setIsPending(true);

$requestBody.setNumber('USPTO-3954432633');

$requestBody.setWebUrl('https://patents.gov/3954432633');



$requestResult = $graphServiceClient.me().profile().patents().post($requestBody);


```