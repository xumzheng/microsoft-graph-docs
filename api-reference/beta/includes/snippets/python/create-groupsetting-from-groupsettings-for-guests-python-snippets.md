---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DirectorySetting()
request_body.setTemplateId('08d542b9-071f-4e16-94b0-74abb372e3d9')

valuesSettingValue1 = SettingValue()
valuesSettingValue1.setName('AllowToAddGuests')

valuesSettingValue1.setValue('false')


valuesArray []= valuesSettingValue1;
request_body.setValues(valuesArray)




result = await client.groups_by_id('group-id').settings.post(request_body, headers=)


```