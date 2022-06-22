---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessReviewScheduleDefinition();


$requestRequestBody->setDisplayName('Test create');
$requestRequestBody->setDescriptionForAdmins('New scheduled access review');
$requestRequestBody->setDescriptionForReviewers('If you have any questions, contact jerry@contoso.com');

$scope = new AccessReviewScope();
$requestRequestBody->setScope($scope);


$scopeAdditionalData = [
	"@odata.type" => '#microsoft.graph.accessReviewQueryScope',
	"query" => '/groups/02f3bafb-448c-487c-88c2-5fd65ce49a41/transitiveMembers',
	"queryType" => 'MicrosoftGraph',
];
$scope->setAdditionalData($scopeAdditionalData);

$reviewersArray = [];

$reviewers1 = new AccessReviewReviewerScope();

$reviewers1->setQuery('/users/398164b1-5196-49dd-ada2-364b49f99b27');
$reviewers1->setQueryType('MicrosoftGraph');

$reviewersArray []= $reviewers1;
$requestRequestBody->setReviewers($reviewersArray);

$settings = new AccessReviewScheduleSettings();
$requestRequestBody->setSettings($settings);


$settings->setMailNotificationsEnabled(True);
$settings->setReminderNotificationsEnabled(True);
$settings->setJustificationRequiredOnApproval(True);
$settings->setDefaultDecisionEnabled(False);
$settings->setDefaultDecision('None');
$settings->setInstanceDurationInDays(1);
$settings->setRecommendationsEnabled(True);

$recurrence = new PatternedRecurrence();
$settings->setRecurrence($recurrence);



$pattern = new RecurrencePattern();
$recurrence->setPattern($pattern);


$pattern->setType(new RecurrencePatternType('weekly'));
$pattern->setInterval(1);


$range = new RecurrenceRange();
$recurrence->setRange($range);


$range->setType(new RecurrenceRangeType('noEnd'));
$range->setStartDate('2020-09-08T12:02:30.667Z');



$result =  $graphClient->identityGovernance()->accessReviews()->definitions()->post($requestRequestBody);


```