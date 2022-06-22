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

$levels1 = new RubricLevel();

$levels1->setDisplayName('Good');

$description = new EducationItemBody();
$levels1->setDescription($description);


$description->setContent('');
$description->setContentType(new BodyType('text'));


$levelsArray []= $levels1;

$levels2 = new RubricLevel();

$levels2->setDisplayName('Poor');

$description = new EducationItemBody();
$levels2->setDescription($description);


$description->setContent('');
$description->setContentType(new BodyType('text'));


$levelsArray []= $levels2;
$requestRequestBody->setLevels($levelsArray);
$qualitiesArray = [];

$qualities1 = new RubricQuality();


$description = new EducationItemBody();
$qualities1->setDescription($description);


$description->setContent('Argument');
$description->setContentType(new BodyType('text'));

$criteriaArray = [];

$criteria1 = new RubricCriterion();


$description = new EducationItemBody();
$criteria1->setDescription($description);


$description->setContent('The essay\'s argument is persuasive.');
$description->setContentType(new BodyType('text'));


$criteriaArray []= $criteria1;

$criteria2 = new RubricCriterion();


$description = new EducationItemBody();
$criteria2->setDescription($description);


$description->setContent('The essay\'s argument does not make sense.');
$description->setContentType(new BodyType('text'));


$criteriaArray []= $criteria2;
$qualities1->setCriteria($criteriaArray);

$qualitiesArray []= $qualities1;

$qualities2 = new RubricQuality();


$description = new EducationItemBody();
$qualities2->setDescription($description);


$description->setContent('Spelling and Grammar');
$description->setContentType(new BodyType('text'));

$criteriaArray = [];

$criteria1 = new RubricCriterion();


$description = new EducationItemBody();
$criteria1->setDescription($description);


$description->setContent('The essay uses proper spelling and grammar with few or no errors.');
$description->setContentType(new BodyType('text'));


$criteriaArray []= $criteria1;

$criteria2 = new RubricCriterion();


$description = new EducationItemBody();
$criteria2->setDescription($description);


$description->setContent('The essay has numerous errors in spelling and/or grammar.');
$description->setContentType(new BodyType('text'));


$criteriaArray []= $criteria2;
$qualities2->setCriteria($criteriaArray);

$qualitiesArray []= $qualities2;
$requestRequestBody->setQualities($qualitiesArray);
$result =  $graphClient->education()->me()->rubrics()->post($requestRequestBody);


```