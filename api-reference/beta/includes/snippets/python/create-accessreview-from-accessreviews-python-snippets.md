---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphServiceClient =  GraphServiceClient(requestAdapter);

requestBody = AccessReview();
requestBody.setDisplayName('TestReview');

requestBody.setStartDateTime(DateTime('2017-02-10T00:35:53.214Z'));

requestBody.setEndDateTime(DateTime('2017-03-12T00:35:53.214Z'));

reviewedEntity = Identity();
reviewedEntity.setId('99025615-a0b1-47ec-9117-35377b10998b');


requestBody.setReviewedEntity($reviewedEntity);
requestBody.setReviewerType('delegated');

requestBody.setBusinessFlowTemplateId('6e4f3d20-c5c3-407f-9695-8460952bcc68');

requestBody.setDescription('Sample description');

reviewersAccessReviewReviewer1 = AccessReviewReviewer();
reviewersAccessReviewReviewer1.setId('f260246a-09b1-4fd5-8d18-daed736071ec');


reviewersArray []= reviewersAccessReviewReviewer1;
reviewersAccessReviewReviewer2 = AccessReviewReviewer();
reviewersAccessReviewReviewer2.setId('5a4e184c-4ee5-4883-96e9-b371f8da88e3');


reviewersArray []= reviewersAccessReviewReviewer2;
requestBody.setReviewers(reviewersArray);


settings = AccessReviewSettings();
settings.setMailNotificationsEnabled(true);

settings.setRemindersEnabled(true);

settings.setJustificationRequiredOnApproval(true);

settings.setAutoReviewEnabled(false);

settings.setActivityDurationInDays(30);

settings.setAutoApplyReviewResultsEnabled(false);

settings.setAccessRecommendationsEnabled(false);

settingsRecurrenceSettings = AccessReviewRecurrenceSettings();
settingsRecurrenceSettings.setRecurrenceType('onetime');

settingsRecurrenceSettings.setRecurrenceEndType('endBy');

settingsRecurrenceSettings.setDurationInDays(0);

settingsRecurrenceSettings.setRecurrenceCount(0);


settings.setRecurrenceSettings($settingsRecurrenceSettings);
settingsAutoReviewSettings = AutoReviewSettings();
settingsAutoReviewSettings.setNotReviewedResult('Deny');


settings.setAutoReviewSettings($settingsAutoReviewSettings);

requestBody.setSettings($settings);


requestResult = graphServiceClient.accessReviews().post(requestBody);


```