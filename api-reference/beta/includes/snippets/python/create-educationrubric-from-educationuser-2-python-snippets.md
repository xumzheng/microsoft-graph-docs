---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter);

request_body = EducationRubric();
request_body.setDisplayName('Example Points Rubric');

description = EducationItemBody();
description.setContent('This is an example of a rubric with points');

description.setContentType(BodyType('text'));


request_body.setDescription($description);
levelsRubricLevel1 = RubricLevel();
levelsRubricLevel1.setDisplayName('Good');

levelsRubricLevel1Description = EducationItemBody();
levelsRubricLevel1Description.setContent('');

levelsRubricLevel1Description.setContentType(BodyType('text'));


levelsRubricLevel1.setDescription($levelsRubricLevel1Description);
levelsRubricLevel1Grading = EducationAssignmentGradeType();
levelsRubricLevel1Grading.set@odatatype('#microsoft.graph.educationAssignmentPointsGradeType');

additionalData = [
'maxPoints' => 2,
];
levelsRubricLevel1Grading.setAdditionalData(additionalData);



levelsRubricLevel1.setGrading($levelsRubricLevel1Grading);

levelsArray []= levelsRubricLevel1;
levelsRubricLevel2 = RubricLevel();
levelsRubricLevel2.setDisplayName('Poor');

levelsRubricLevel2Description = EducationItemBody();
levelsRubricLevel2Description.setContent('');

levelsRubricLevel2Description.setContentType(BodyType('text'));


levelsRubricLevel2.setDescription($levelsRubricLevel2Description);
levelsRubricLevel2Grading = EducationAssignmentGradeType();
levelsRubricLevel2Grading.set@odatatype('#microsoft.graph.educationAssignmentPointsGradeType');

additionalData = [
'maxPoints' => 1,
];
levelsRubricLevel2Grading.setAdditionalData(additionalData);



levelsRubricLevel2.setGrading($levelsRubricLevel2Grading);

levelsArray []= levelsRubricLevel2;
request_body.setLevels(levelsArray);


qualitiesRubricQuality1 = RubricQuality();
qualitiesRubricQuality1Description = EducationItemBody();
qualitiesRubricQuality1Description.setContent('Argument');

qualitiesRubricQuality1Description.setContentType(BodyType('text'));


qualitiesRubricQuality1.setDescription($qualitiesRubricQuality1Description);
criteriaRubricCriterion1 = RubricCriterion();
criteriaRubricCriterion1Description = EducationItemBody();
criteriaRubricCriterion1Description.setContent('The essay\'s argument is persuasive.');

criteriaRubricCriterion1Description.setContentType(BodyType('text'));


criteriaRubricCriterion1.setDescription($criteriaRubricCriterion1Description);

criteriaArray []= criteriaRubricCriterion1;
criteriaRubricCriterion2 = RubricCriterion();
criteriaRubricCriterion2Description = EducationItemBody();
criteriaRubricCriterion2Description.setContent('The essay\'s argument does not make sense.');

criteriaRubricCriterion2Description.setContentType(BodyType('text'));


criteriaRubricCriterion2.setDescription($criteriaRubricCriterion2Description);

criteriaArray []= criteriaRubricCriterion2;
qualitiesRubricQuality1.setCriteria(criteriaArray);


qualitiesRubricQuality1.setWeight(50.0);


qualitiesArray []= qualitiesRubricQuality1;
qualitiesRubricQuality2 = RubricQuality();
qualitiesRubricQuality2Description = EducationItemBody();
qualitiesRubricQuality2Description.setContent('Spelling and Grammar');

qualitiesRubricQuality2Description.setContentType(BodyType('text'));


qualitiesRubricQuality2.setDescription($qualitiesRubricQuality2Description);
criteriaRubricCriterion1 = RubricCriterion();
criteriaRubricCriterion1Description = EducationItemBody();
criteriaRubricCriterion1Description.setContent('The essay uses proper spelling and grammar with few or no errors.');

criteriaRubricCriterion1Description.setContentType(BodyType('text'));


criteriaRubricCriterion1.setDescription($criteriaRubricCriterion1Description);

criteriaArray []= criteriaRubricCriterion1;
criteriaRubricCriterion2 = RubricCriterion();
criteriaRubricCriterion2Description = EducationItemBody();
criteriaRubricCriterion2Description.setContent('The essay has numerous errors in spelling and/or grammar.');

criteriaRubricCriterion2Description.setContentType(BodyType('text'));


criteriaRubricCriterion2.setDescription($criteriaRubricCriterion2Description);

criteriaArray []= criteriaRubricCriterion2;
qualitiesRubricQuality2.setCriteria(criteriaArray);


qualitiesRubricQuality2.setWeight(50.0);


qualitiesArray []= qualitiesRubricQuality2;
request_body.setQualities(qualitiesArray);


grading = EducationAssignmentGradeType();
grading.set@odatatype('#microsoft.graph.educationAssignmentPointsGradeType');


request_body.setGrading($grading);


result = await client.education().me().rubrics().post(request_body);


```