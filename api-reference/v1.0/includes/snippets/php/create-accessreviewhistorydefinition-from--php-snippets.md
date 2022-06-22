---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessReviewHistoryDefinition();


$requestRequestBody->setDisplayName('Last quarter\'s group reviews April 2021');
$decisionsArray = [];
'approve',$decisionsArray []= $decisions1;
'deny',$decisionsArray []= $decisions2;
'dontKnow',$decisionsArray []= $decisions3;
'notReviewed',$decisionsArray []= $decisions4;
'notNotified',$decisionsArray []= $decisions5;
$requestRequestBody->setDecisions($decisionsArray);

$scheduleSettings = new AccessReviewHistoryScheduleSettings();
$requestRequestBody->setScheduleSettings($scheduleSettings);


$scheduleSettings->setReportRange('P1M');

$recurrence = new PatternedRecurrence();
$scheduleSettings->setRecurrence($recurrence);



$pattern = new RecurrencePattern();
$recurrence->setPattern($pattern);


$pattern->setType(new RecurrencePatternType('monthly'));
$pattern->setInterval(1);


$range = new RecurrenceRange();
$recurrence->setRange($range);


$range->setType(new RecurrenceRangeType('noEnd'));
$range->setStartDate('2018-08-03T21:02:30.667Z');
$rangeAdditionalData = [
"count" => 0,
];
$range->setAdditionalData($rangeAdditionalData);



$scopesArray = [];

$scopes1 = new AccessReviewScope();

$scopes1AdditionalData = [
"@odata.type" => '#microsoft.graph.accessReviewQueryScope',
"queryType" => 'MicrosoftGraph',
"query" => '/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, \'accessPackageAssignments\')',
"queryRoot" => null,
];
$scopes1->setAdditionalData($scopes1AdditionalData);

$scopesArray []= $scopes1;

$scopes2 = new AccessReviewScope();

$scopes2AdditionalData = [
"@odata.type" => '#microsoft.graph.accessReviewQueryScope',
"queryType" => 'MicrosoftGraph',
"query" => '/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, \'/groups\')',
"queryRoot" => null,
];
$scopes2->setAdditionalData($scopes2AdditionalData);

$scopesArray []= $scopes2;
$requestRequestBody->setScopes($scopesArray);
$result =  $graphClient->identityGovernance()->accessReviews()->historyDefinitions()->post($requestRequestBody);


```