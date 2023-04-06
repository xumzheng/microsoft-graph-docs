---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = LearningContent()
request_body.setTitle('Manage classes, resources, assessment, and planning in Microsoft Teams with Beedle')

request_body.setDescription('A module to guide users through the various teaching and learning enhancements that Beedle provides within Microsoft Teams, with many examples of everyday application.')

request_body.setContentWebUrl('https://learn.microsoft.com/learn/modules/manage-classes-resources-assessment-planning-beedle/')

request_body.setSourceName('MsLearn')

request_body.setThumbnailWebUrl('https://syndetics.com/index.aspx?isbn=9783319672175/LC.GIF')

request_body.setLanguageTag('en-us')

request_body.setNumberOfPages(9)

$request_body.setDuration( \DateInterval('PT20M'))

request_body.setFormat('Book')

request_body.setCreatedDateTime(DateTime('2018-01-01T00:00:00Z'))

request_body.setLastModifiedDateTime(DateTime('2021-04-01T04:26:06.1995367Z'))

request_body.setContributors(['Scott Simpson', ])

request_body.setAdditionalTags(['Create private or public teams', 'Add members to teams', ])

request_body.setSkillTags(['Create teams', 'Teams channels', 'Teams members', ])

request_body.setIsActive(true)

request_body.setIsPremium(false)

request_body.setIsSearchable(true)



result = await client.employeeExperience.learningProviders_by_id('learningProvider-id').learningContents_by_id('learningContent-id').patch(request_body, headers=)


```