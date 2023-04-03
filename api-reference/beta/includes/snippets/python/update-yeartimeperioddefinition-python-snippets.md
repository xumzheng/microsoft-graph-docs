---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = YearTimePeriodDefinition();
requestBody.setDisplayName('Fiscal Year 2022');

requestBody.setId('ebf18762-ab92-487e-21d1-08daddab28bb');



requestResult = graphServiceClient.external().industryData().yearsById('yearTimePeriodDefinition-id').patch(requestBody);


```