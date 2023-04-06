---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = Bookmark()
request_body.setDisplayName('Contoso Install Site')

request_body.setWebUrl('http://www.contoso.com/')

request_body.setDescription('Try or buy Contoso for Home or Business and view product information')

keywords = AnswerKeyword()
keywords.setKeywords(['Contoso', 'install', ])

keywords.setReservedKeywords(['Contoso', ])

keywords.setMatchSimilarKeywords(true)


request_body.setKeywords($keywords)
request_body.setAvailabilityStartDateTime(null)

request_body.setAvailabilityEndDateTime(null)

request_body.setPlatforms([request_body.setDevicePlatformType(DevicePlatformType('windows'))
])

targetedVariationsAnswerVariant1 = AnswerVariant()
targetedVariationsAnswerVariant1.setLanguageTag('es-es')

targetedVariationsAnswerVariant1.setDisplayName('Sitio de instalación Contoso')

targetedVariationsAnswerVariant1.setDescription('Pruebe o compre Contoso hogar o negocios y vea la información del producto')


targetedVariationsArray []= targetedVariationsAnswerVariant1;
request_body.setTargetedVariations(targetedVariationsArray)


request_body.setState(AnswerState('published'))



result = await client.search.bookmarks.post(request_body)


```