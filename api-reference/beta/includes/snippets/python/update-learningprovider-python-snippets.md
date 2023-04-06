---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = LearningProvider()
request_body.setDisplayName('Microsoft')

request_body.setSquareLogoWebUrlForDarkTheme('https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png')

request_body.setLongLogoWebUrlForDarkTheme('https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png')

request_body.setSquareLogoWebUrlForLightTheme('https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png')

request_body.setLongLogoWebUrlForLightTheme('https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png')

request_body.setLoginWebUrl('https://www.linkedin.com/learning-login/teams')


request_config = LearningProviderRequestBuilderPatchRequestConfiguration(
request_config = LearningProviderRequestBuilderPatchRequestConfiguration(query_params=)


result = await client.employeeExperience.learningProviders_by_id('learningProvider-id').patch(request_body, headers=)


```