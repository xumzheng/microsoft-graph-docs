---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessReviewScheduleDefinition();


$requestRequestBody->setDisplayName('Review inactive guests on teams');
$requestRequestBody->setDescriptionForAdmins('Control guest user access to our teams.');
$requestRequestBody->setDescriptionForReviewers('Information security is everyone\'s responsibility. Review our access policy for more.');

$instanceEnumerationScope = new AccessReviewScope();
$requestRequestBody->setInstanceEnumerationScope($instanceEnumerationScope);


$instanceEnumerationScopeAdditionalData = [
	"@odata.type" => '#microsoft.graph.accessReviewQueryScope',
	"query" => '/groups?$filter=(groupTypes/any(c:c+eq+\'Unified\') and resourceProvisioningOptions/Any(x:x eq \'Team\')\')',
	"queryType" => 'MicrosoftGraph',
];
$instanceEnumerationScope->setAdditionalData($instanceEnumerationScopeAdditionalData);


$scope = new AccessReviewScope();
$requestRequestBody->setScope($scope);


$scopeAdditionalData = [
"@odata.type" => '#microsoft.graph.accessReviewInactiveUsersQueryScope',
"query" => './members/microsoft.graph.user/?$filter=(userType eq \'Guest\')',
"queryType" => 'MicrosoftGraph',
"inactiveDuration" => 'P30D',
];
$scope->setAdditionalData($scopeAdditionalData);

$reviewersArray = [];

$reviewersreviewers1 = new AccessReviewReviewerScope();

$reviewersreviewers1AdditionalData = [
"query" => './owners',
"queryType" => 'MicrosoftGraph',
];
$reviewersreviewers1->setAdditionalData($reviewersreviewers1AdditionalData);

$reviewersArray []= $reviewersreviewers1;
$requestRequestBody->setReviewers($reviewersArray);
$fallbackReviewersArray = [];

$fallbackReviewersfallbackReviewers1 = new AccessReviewReviewerScope();

$fallbackReviewersfallbackReviewers1AdditionalData = [
"query" => '/users/fc9a2c2b-1ddc-486d-a211-5fe8ca77fa1f',
"queryType" => 'MicrosoftGraph',
];
$fallbackReviewersfallbackReviewers1->setAdditionalData($fallbackReviewersfallbackReviewers1AdditionalData);

$fallbackReviewersArray []= $fallbackReviewersfallbackReviewers1;
$requestRequestBody->setFallbackReviewers($fallbackReviewersArray);

$settings = new AccessReviewScheduleSettings();
$requestRequestBody->setSettings($settings);


$settings->setMailNotificationsEnabled(True);
$settings->setReminderNotificationsEnabled(True);
$settings->setJustificationRequiredOnApproval(True);
$settings->setRecommendationsEnabled(True);
$settings->setInstanceDurationInDays(3);

$recurrence = new PatternedRecurrence();
$settings->setRecurrence($recurrence);



$pattern = new RecurrencePattern();
$recurrence->setPattern($pattern);


$pattern->setType(new RecurrencePatternType('absoluteMonthly'));
$pattern->setDayOfMonth(5);
$pattern->setInterval(3);


$range = new RecurrenceRange();
$recurrence->setRange($range);


$range->setType(new RecurrenceRangeType('noEnd'));
$range->setStartDate(new Date("2020-05-04T00:00:00.000Z"));


$settings->setDefaultDecisionEnabled(True);
$settings->setDefaultDecision('Deny');
$settings->setAutoApplyDecisionsEnabled(True);

$result =  $graphClient->identityGovernance()->accessReviews()->definitions()->post($requestRequestBody);


```