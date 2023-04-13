---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = ApplyPostRequestBody()
criteria = WorkbookFilterCriteria()
criteria.criterion1 = 'criterion1-value'

criteria.criterion2 = 'criterion2-value'

criteria.color = 'color-value'

criteria_operator = Operator()

criteria.operator = criteriaOperator
criteria_icon = WorkbookIcon()
criteriaIcon.set = 'set-value'

criteriaIcon.index = 99


criteria.icon = criteriaIcon
criteria.dynamicCriteria = 'dynamicCriteria-value'

criteria_values = Json()

criteria.values = criteriaValues
criteria.filterOn = 'filterOn-value'


request_body.criteria = criteria



await client.drives_by_id('drive-id').items_by_id('driveItem-id').workbook.tables_by_id('workbookTable-id').columns_by_id('workbookTableColumn-id').filter.apply.post(request_body = request_body)


```