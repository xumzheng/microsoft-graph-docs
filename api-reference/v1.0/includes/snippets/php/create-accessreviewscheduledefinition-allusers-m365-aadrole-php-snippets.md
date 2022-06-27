---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessReviewScheduleDefinition();


$requestRequestBody->setDisplayName('Review employee access to LinkedIn');
$requestRequestBody->setDescriptionForAdmins('Review employee access to LinkedIn');

$scope = new AccessReviewScope();
$requestRequestBody->setScope($scope);


$scopeAdditionalData = [
	"@odata.type" => '#microsoft.graph.principalResourceMembershipsScope',
	"principalScopes" => [],
"resourceScopes" => [],
];
$scope->setAdditionalData($scopeAdditionalData);

$reviewersArray = [];

$reviewersreviewers1 = new AccessReviewReviewerScope();

$reviewersreviewers1->setQuery('./manager');
$reviewersreviewers1->setQueryType('MicrosoftGraph');
$reviewersreviewers1->setQueryRoot('decisions');

$reviewersArray []= $reviewersreviewers1;
$requestRequestBody->setReviewers($reviewersArray);
$fallbackReviewersArray = [];

$fallbackReviewersfallbackReviewers1 = new AccessReviewReviewerScope();

$fallbackReviewersfallbackReviewers1->setQuery('/groups/072ac5f4-3f13-4088-ab30-0a276f3e6322/transitiveMembers');
$fallbackReviewersfallbackReviewers1->setQueryType('MicrosoftGraph');

$fallbackReviewersArray []= $fallbackReviewersfallbackReviewers1;
$requestRequestBody->setFallbackReviewers($fallbackReviewersArray);

$settings = new AccessReviewScheduleSettings();
$requestRequestBody->setSettings($settings);


$settings->setMailNotificationsEnabled(True);
$settings->setReminderNotificationsEnabled(True);
$settings->setJustificationRequiredOnApproval(True);
$settings->setDefaultDecisionEnabled(True);
$settings->setDefaultDecision('Recommendation');
$settings->setInstanceDurationInDays(180);
$settings->setAutoApplyDecisionsEnabled(True);
$settings->setRecommendationsEnabled(True);

$recurrence = new PatternedRecurrence();
$settings->setRecurrence($recurrence);



$pattern = new RecurrencePattern();
$recurrence->setPattern($pattern);


$pattern->setType(new RecurrencePatternType('absoluteMonthly'));
$pattern->setInterval(6);
$pattern->setDayOfMonth(0);


$range = new RecurrenceRange();
$recurrence->setRange($range);


$range->setType(new RecurrenceRangeType('numbered'));
$range->setStartDate(new Date("2021-05-05"));
$range->setEndDate(new Date("2022-05-05"));



$requestRequestBodyAdditionalData = [
"backupReviewers" => [],
];
$requestRequestBody->setAdditionalData($requestRequestBodyAdditionalData);
$result =  $graphClient->identityGovernance()->accessReviews()->definitions()->post($requestRequestBody);


```