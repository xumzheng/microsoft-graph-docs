---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = AccessReview()
request_body.displayName = 'TestReview'

request_body.startDateTime = DateTime('2017-02-10T00:35:53.214Z')

request_body.endDateTime = DateTime('2017-03-12T00:35:53.214Z')

reviewedEntity = Identity()
reviewedEntity.id = '99025615-a0b1-47ec-9117-35377b10998b'


request_body.reviewedEntity = reviewedEntity
request_body.reviewerType = 'delegated'

request_body.businessFlowTemplateId = '6e4f3d20-c5c3-407f-9695-8460952bcc68'

request_body.description = 'Sample description'

reviewersAccessReviewReviewer1 = AccessReviewReviewer()
reviewersAccessReviewReviewer1.id = 'f260246a-09b1-4fd5-8d18-daed736071ec'


reviewersArray []= reviewersAccessReviewReviewer1;
reviewersAccessReviewReviewer2 = AccessReviewReviewer()
reviewersAccessReviewReviewer2.id = '5a4e184c-4ee5-4883-96e9-b371f8da88e3'


reviewersArray []= reviewersAccessReviewReviewer2;
request_body.reviewers(reviewersArray)


settings = AccessReviewSettings()
settings.mailNotificationsEnabled = true

settings.remindersEnabled = true

settings.justificationRequiredOnApproval = true

settings.autoReviewEnabled = false

settings.activityDurationInDays = 30

settings.autoApplyReviewResultsEnabled = false

settings.accessRecommendationsEnabled = false

settingsRecurrenceSettings = AccessReviewRecurrenceSettings()
settingsRecurrenceSettings.recurrenceType = 'onetime'

settingsRecurrenceSettings.recurrenceEndType = 'endBy'

settingsRecurrenceSettings.durationInDays = 0

settingsRecurrenceSettings.recurrenceCount = 0


settings.recurrenceSettings = settingsRecurrenceSettings
settingsAutoReviewSettings = AutoReviewSettings()
settingsAutoReviewSettings.notReviewedResult = 'Deny'


settings.autoReviewSettings = settingsAutoReviewSettings

request_body.settings = settings



result = await client.accessReviews.post(request_body = request_body)


```