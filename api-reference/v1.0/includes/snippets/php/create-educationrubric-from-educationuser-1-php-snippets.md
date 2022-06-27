---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

//THIS SNIPPET IS A PREVIEW FOR THE KIOTA BASED SDK. NON-PRODUCTION USE ONLY
$graphClient = new GraphClient($requestAdapter);

$requestRequestBody = new EducationRubric();


$requestRequestBody->setDisplayName('Example Credit Rubric');

$description = new EducationItemBody();
$requestRequestBody->setDescription($description);


$description->setContent('This is an example of a credit rubric (no points)');
$description->setContentType(new BodyType('text'));

$levelsArray = [];

$levelslevels1 = new RubricLevel();

$levelslevels1->setDisplayName('Good');

$description = new EducationItemBody();
$levelslevels1->setDescription($description);


$description->setContent('');
$description->setContentType(new BodyType('text'));


$levelsArray []= $levelslevels1;

$levelslevels2 = new RubricLevel();

$levelslevels2->setDisplayName('Poor');

$description = new EducationItemBody();
$levelslevels2->setDescription($description);


$description->setContent('');
$description->setContentType(new BodyType('text'));


$levelsArray []= $levelslevels2;
$requestRequestBody->setLevels($levelsArray);
$qualitiesArray = [];

$qualitiesqualities1 = new RubricQuality();


$description = new EducationItemBody();
$qualitiesqualities1->setDescription($description);


$description->setContent('Argument');
$description->setContentType(new BodyType('text'));

$criteriaArray = [];

$criteriacriteria1 = new RubricCriterion();


$description = new EducationItemBody();
$criteriacriteria1->setDescription($description);


$description->setContent('The essay\'s argument is persuasive.');
$description->setContentType(new BodyType('text'));


$criteriaArray []= $criteriacriteria1;

$criteriacriteria2 = new RubricCriterion();


$description = new EducationItemBody();
$criteriacriteria2->setDescription($description);


$description->setContent('The essay\'s argument does not make sense.');
$description->setContentType(new BodyType('text'));


$criteriaArray []= $criteriacriteria2;
$qualitiesqualities1->setCriteria($criteriaArray);

$qualitiesArray []= $qualitiesqualities1;

$qualitiesqualities2 = new RubricQuality();


$description = new EducationItemBody();
$qualitiesqualities2->setDescription($description);


$description->setContent('Spelling and Grammar');
$description->setContentType(new BodyType('text'));

$criteriaArray = [];

$criteriacriteria1 = new RubricCriterion();


$description = new EducationItemBody();
$criteriacriteria1->setDescription($description);


$description->setContent('The essay uses proper spelling and grammar with few or no errors.');
$description->setContentType(new BodyType('text'));


$criteriaArray []= $criteriacriteria1;

$criteriacriteria2 = new RubricCriterion();


$description = new EducationItemBody();
$criteriacriteria2->setDescription($description);


$description->setContent('The essay has numerous errors in spelling and/or grammar.');
$description->setContentType(new BodyType('text'));


$criteriaArray []= $criteriacriteria2;
$qualitiesqualities2->setCriteria($criteriaArray);

$qualitiesArray []= $qualitiesqualities2;
$requestRequestBody->setQualities($qualitiesArray);
$result =  $graphClient->education()->me()->rubrics()->post($requestRequestBody);


```