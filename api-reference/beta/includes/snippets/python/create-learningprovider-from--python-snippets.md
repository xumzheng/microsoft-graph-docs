---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = LearningProvider()
request_body.displayName = 'Microsoft'

request_body.squareLogoWebUrlForDarkTheme = 'https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png'

request_body.longLogoWebUrlForDarkTheme = 'https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png'

request_body.squareLogoWebUrlForLightTheme = 'https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png'

request_body.longLogoWebUrlForLightTheme = 'https://support.content.office.net/en-us/media/4c531d12-4c13-4782-a6e4-4b8f991801a3.png'

request_body.loginWebUrl = 'https://www.linkedin.com/learning-login/teams'




result = await client.employeeExperience.learningProviders.post(request_body = request_body)


```