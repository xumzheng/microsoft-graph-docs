---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new AccessReviewHistoryDefinition();


$requestRequestBody->setDisplayName('Last quarter\'s group reviews April 2021');
$decisionsArray = [];
'approve',$decisionsArray []= $decisionsdecisions1;
'deny',$decisionsArray []= $decisionsdecisions2;
'dontKnow',$decisionsArray []= $decisionsdecisions3;
'notReviewed',$decisionsArray []= $decisionsdecisions4;
'notNotified',$decisionsArray []= $decisionsdecisions5;
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
$range->setStartDate(new Date("2018-08-03T21:02:30.667Z"));
$rangeAdditionalData = [
"count" => 0,
];
$range->setAdditionalData($rangeAdditionalData);



$scopesArray = [];

$scopesscopes1 = new AccessReviewScope();

$scopesscopes1AdditionalData = [
"@odata.type" => '#microsoft.graph.accessReviewQueryScope',
"queryType" => 'MicrosoftGraph',
"query" => '/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, \'accessPackageAssignments\')',
"queryRoot" => null,
];
$scopesscopes1->setAdditionalData($scopesscopes1AdditionalData);

$scopesArray []= $scopesscopes1;

$scopesscopes2 = new AccessReviewScope();

$scopesscopes2AdditionalData = [
"@odata.type" => '#microsoft.graph.accessReviewQueryScope',
"queryType" => 'MicrosoftGraph',
"query" => '/identityGovernance/accessReviews/definitions?$filter=contains(scope/query, \'/groups\')',
"queryRoot" => null,
];
$scopesscopes2->setAdditionalData($scopesscopes2AdditionalData);

$scopesArray []= $scopesscopes2;
$requestRequestBody->setScopes($scopesArray);
$result =  $graphClient->identityGovernance()->accessReviews()->historyDefinitions()->post($requestRequestBody);


```