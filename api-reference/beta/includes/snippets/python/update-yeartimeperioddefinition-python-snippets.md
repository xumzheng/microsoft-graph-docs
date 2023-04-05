---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = YearTimePeriodDefinition()
request_body.setDisplayName('Fiscal Year 2022')

request_body.setId('ebf18762-ab92-487e-21d1-08daddab28bb')



result = await client.external.industryData.yearsById('yearTimePeriodDefinition-id').patch(request_body)


```