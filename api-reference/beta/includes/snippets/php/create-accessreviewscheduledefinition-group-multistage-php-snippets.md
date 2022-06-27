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

$stageSettingsstageSettings1 = new AccessReviewStageSettings();

$stageSettingsstageSettings1->setStageId('1');
$stageSettingsstageSettings1->setDurationInDays(2);
$stageSettingsstageSettings1->setRecommendationsEnabled(False);
$stageSettingsstageSettings1->setDecisionsThatWillMoveToNextStage(['NotReviewed','Approve',]);
$reviewersArray = [];

$reviewersreviewers1 = new AccessReviewReviewerScope();

$reviewersreviewers1AdditionalData = [
"query" => '/users/398164b1-5196-49dd-ada2-364b49f99b27',
"queryType" => 'MicrosoftGraph',
];
$reviewersreviewers1->setAdditionalData($reviewersreviewers1AdditionalData);

$reviewersArray []= $reviewersreviewers1;
$stageSettingsstageSettings1->setReviewers($reviewersArray);

$stageSettingsArray []= $stageSettingsstageSettings1;

$stageSettingsstageSettings2 = new AccessReviewStageSettings();

$stageSettingsstageSettings2->setStageId('2');
$stageSettingsstageSettings2->setDependsOn(['1',]);
$stageSettingsstageSettings2->setDurationInDays(2);
$stageSettingsstageSettings2->setRecommendationsEnabled(True);
$reviewersArray = [];

$reviewersreviewers1 = new AccessReviewReviewerScope();

$reviewersreviewers1AdditionalData = [
"query" => './manager',
"queryType" => 'MicrosoftGraph',
"queryRoot" => 'decisions',
];
$reviewersreviewers1->setAdditionalData($reviewersreviewers1AdditionalData);

$reviewersArray []= $reviewersreviewers1;
$stageSettingsstageSettings2->setReviewers($reviewersArray);
$fallbackReviewersArray = [];

$fallbackReviewersfallbackReviewers1 = new AccessReviewReviewerScope();

$fallbackReviewersfallbackReviewers1AdditionalData = [
"query" => '/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers',
"queryType" => 'MicrosoftGraph',
];
$fallbackReviewersfallbackReviewers1->setAdditionalData($fallbackReviewersfallbackReviewers1AdditionalData);

$fallbackReviewersArray []= $fallbackReviewersfallbackReviewers1;
$stageSettingsstageSettings2->setFallbackReviewers($fallbackReviewersArray);

$stageSettingsArray []= $stageSettingsstageSettings2;
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
$range->setStartDate(new Date("2020-09-08T12:02:30.667Z"));


$settings->setDecisionHistoriesForReviewersEnabled(True);

$result =  $graphClient->identityGovernance()->accessReviews()->definitions()->post($requestRequestBody);


```