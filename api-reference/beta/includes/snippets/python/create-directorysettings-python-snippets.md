---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = DirectorySetting()
request_body.templateId = '62375ab9-6b52-47ed-826b-58e47e0e304b'

valuesSettingValue1 = SettingValue()
valuesSettingValue1.name = 'GuestUsageGuidelinesUrl'

valuesSettingValue1.value = 'https://privacy.contoso.com/privacystatement'


valuesArray []= valuesSettingValue1;
valuesSettingValue2 = SettingValue()
valuesSettingValue2.name = 'EnableMSStandardBlockedWords'

valuesSettingValue2.value = 'true'


valuesArray []= valuesSettingValue2;
valuesSettingValue3 = SettingValue()
valuesSettingValue3.name = 'EnableMIPLabels'

valuesSettingValue3.value = 'true'


valuesArray []= valuesSettingValue3;
valuesSettingValue4 = SettingValue()
valuesSettingValue4.name = 'PrefixSuffixNamingRequirement'

valuesSettingValue4.value = '[Contoso-][GroupName]'


valuesArray []= valuesSettingValue4;
request_body.values(valuesArray)




request_configuration = SettingsRequestBuilderPostRequestConfiguration(
)


result = await client.settings.post(request_body = request_body)


```