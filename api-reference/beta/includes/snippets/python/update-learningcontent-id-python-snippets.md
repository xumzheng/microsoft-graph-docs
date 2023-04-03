---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(requestAdapter);

requestBody = LearningContent();
requestBody.setTitle('Manage classes, resources, assessment, and planning in Microsoft Teams with Beedle');

requestBody.setDescription('A module to guide users through the various teaching and learning enhancements that Beedle provides within Microsoft Teams, with many examples of everyday application.');

requestBody.setContentWebUrl('https://learn.microsoft.com/learn/modules/manage-classes-resources-assessment-planning-beedle/');

requestBody.setSourceName('MsLearn');

requestBody.setThumbnailWebUrl('https://syndetics.com/index.aspx?isbn=9783319672175/LC.GIF');

requestBody.setLanguageTag('en-us');

requestBody.setNumberOfPages(9);

$requestBody.setDuration( \DateInterval('PT20M'));

requestBody.setFormat('Book');

requestBody.setCreatedDateTime(DateTime('2018-01-01T00:00:00Z'));

requestBody.setLastModifiedDateTime(DateTime('2021-04-01T04:26:06.1995367Z'));

requestBody.setContributors(['Scott Simpson', ]);

requestBody.setAdditionalTags(['Create private or public teams', 'Add members to teams', ]);

requestBody.setSkillTags(['Create teams', 'Teams channels', 'Teams members', ]);

requestBody.setIsActive(true);

requestBody.setIsPremium(false);

requestBody.setIsSearchable(true);



result = awaitclient.employeeExperience().learningProvidersById('learningProvider-id').learningContentsById('learningContent-id').patch(requestBody);


```