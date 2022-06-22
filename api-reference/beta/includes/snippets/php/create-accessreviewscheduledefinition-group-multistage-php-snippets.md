---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessReviewScheduleDefinition();


$requestRequestBody->setDisplayName('Group Multi-stage Access Review');
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

$stageSettingsArray = [];

$stageSettings1 = new AccessReviewStageSettings();

$stageSettings1->setStageId('1');
$stageSettings1->setDurationInDays(2);
$stageSettings1->setRecommendationsEnabled(False);
$stageSettings1->setDecisionsThatWillMoveToNextStage( [
'NotReviewed','Approve',],
$reviewersArray = [];

$reviewers1 = new AccessReviewReviewerScope();

$reviewers1AdditionalData = [
		"query" => '/users/398164b1-5196-49dd-ada2-364b49f99b27',
		"queryType" => 'MicrosoftGraph',
	];
$reviewers1->setAdditionalData($reviewers1AdditionalData);

$reviewersArray []= $reviewers1;
$stageSettings1->setReviewers($reviewersArray);

$stageSettingsArray []= $stageSettings1;

$stageSettings2 = new AccessReviewStageSettings();

$stageSettings2->setStageId('2');
$stageSettings2->setDependsOn( [
'1',],
$stageSettings2->setDurationInDays(2);
$stageSettings2->setRecommendationsEnabled(True);
$reviewersArray = [];

$reviewers1 = new AccessReviewReviewerScope();

$reviewers1AdditionalData = [
"query" => './manager',
"queryType" => 'MicrosoftGraph',
"queryRoot" => 'decisions',
];
$reviewers1->setAdditionalData($reviewers1AdditionalData);

$reviewersArray []= $reviewers1;
$stageSettings2->setReviewers($reviewersArray);
$fallbackReviewersArray = [];

$fallbackReviewers1 = new AccessReviewReviewerScope();

$fallbackReviewers1AdditionalData = [
"query" => '/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers',
"queryType" => 'MicrosoftGraph',
];
$fallbackReviewers1->setAdditionalData($fallbackReviewers1AdditionalData);

$fallbackReviewersArray []= $fallbackReviewers1;
$stageSettings2->setFallbackReviewers($fallbackReviewersArray);

$stageSettingsArray []= $stageSettings2;
$requestRequestBody->setStageSettings($stageSettingsArray);

$settings = new AccessReviewScheduleSettings();
$requestRequestBody->setSettings($settings);


$settings->setMailNotificationsEnabled(True);
$settings->setReminderNotificationsEnabled(True);
$settings->setJustificationRequiredOnApproval(True);
$settings->setDefaultDecisionEnabled(False);
$settings->setDefaultDecision('None');
$settings->setInstanceDurationInDays(4);

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


$settings->setDecisionHistoriesForReviewersEnabled(True);

$result =  $graphClient->identityGovernance()->accessReviews()->definitions()->post($requestRequestBody);


```