---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessReview();


$requestRequestBody->setDisplayName('TestReview');
$requestRequestBody->setStartDateTime(new DateTime("2017-02-10T00:35:53.214Z"));
$requestRequestBody->setEndDateTime(new DateTime("2017-03-12T00:35:53.214Z"));

$reviewedEntity = new Identity();
$requestRequestBody->setReviewedEntity($reviewedEntity);


$reviewedEntity->setId('99025615-a0b1-47ec-9117-35377b10998b');

$requestRequestBody->setReviewerType('delegated');
$requestRequestBody->setBusinessFlowTemplateId('6e4f3d20-c5c3-407f-9695-8460952bcc68');
$requestRequestBody->setDescription('Sample description');
$reviewersArray = [];

$reviewers1 = new AccessReviewReviewer();

$reviewers1->setId('f260246a-09b1-4fd5-8d18-daed736071ec');

$reviewersArray []= $reviewers1;

$reviewers2 = new AccessReviewReviewer();

$reviewers2->setId('5a4e184c-4ee5-4883-96e9-b371f8da88e3');

$reviewersArray []= $reviewers2;
$requestRequestBody->setReviewers($reviewersArray);

$settings = new AccessReviewSettings();
$requestRequestBody->setSettings($settings);


$settings->setMailNotificationsEnabled(True);
$settings->setRemindersEnabled(True);
$settings->setJustificationRequiredOnApproval(True);
$settings->setAutoReviewEnabled(False);
$settings->setActivityDurationInDays(30);
$settings->setAutoApplyReviewResultsEnabled(False);
$settings->setAccessRecommendationsEnabled(False);

$recurrenceSettings = new AccessReviewRecurrenceSettings();
$settings->setRecurrenceSettings($recurrenceSettings);


$recurrenceSettings->setRecurrenceType('onetime');
$recurrenceSettings->setRecurrenceEndType('endBy');
$recurrenceSettings->setDurationInDays(0);
$recurrenceSettings->setRecurrenceCount(0);


$autoReviewSettings = new AutoReviewSettings();
$settings->setAutoReviewSettings($autoReviewSettings);


$autoReviewSettings->setNotReviewedResult('Deny');


$result =  $graphClient->accessReviews()->post($requestRequestBody);


```