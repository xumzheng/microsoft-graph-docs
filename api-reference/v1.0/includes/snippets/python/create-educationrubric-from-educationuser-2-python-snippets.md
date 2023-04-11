---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = EducationRubric()
request_body.displayName = 'Example Points Rubric'

description = EducationItemBody()
description.content = 'This is an example of a rubric with points'

description.ContentType(BodyType('text'))


request_body.description = description
levelsRubricLevel1 = RubricLevel()
levelsRubricLevel1.displayName = 'Good'

levelsRubricLevel1Description = EducationItemBody()
levelsRubricLevel1Description.content = ''

levelsRubricLevel1Description.ContentType(BodyType('text'))


levelsRubricLevel1.description = levelsRubricLevel1Description
levelsRubricLevel1Grading = EducationAssignmentGradeType()
levelsRubricLevel1Grading.@odatatype = '#microsoft.graph.educationAssignmentPointsGradeType'

additionalData = [
'maxPoints' => 2,
];
levelsRubricLevel1Grading.additionaldata(additionalData)



levelsRubricLevel1.grading = levelsRubricLevel1Grading

levelsArray []= levelsRubricLevel1;
levelsRubricLevel2 = RubricLevel()
levelsRubricLevel2.displayName = 'Poor'

levelsRubricLevel2Description = EducationItemBody()
levelsRubricLevel2Description.content = ''

levelsRubricLevel2Description.ContentType(BodyType('text'))


levelsRubricLevel2.description = levelsRubricLevel2Description
levelsRubricLevel2Grading = EducationAssignmentGradeType()
levelsRubricLevel2Grading.@odatatype = '#microsoft.graph.educationAssignmentPointsGradeType'

additionalData = [
'maxPoints' => 1,
];
levelsRubricLevel2Grading.additionaldata(additionalData)



levelsRubricLevel2.grading = levelsRubricLevel2Grading

levelsArray []= levelsRubricLevel2;
request_body.levels(levelsArray)


qualitiesRubricQuality1 = RubricQuality()
qualitiesRubricQuality1Description = EducationItemBody()
qualitiesRubricQuality1Description.content = 'Argument'

qualitiesRubricQuality1Description.ContentType(BodyType('text'))


qualitiesRubricQuality1.description = qualitiesRubricQuality1Description
criteriaRubricCriterion1 = RubricCriterion()
criteriaRubricCriterion1Description = EducationItemBody()
criteriaRubricCriterion1Description.content = 'The essay\'s argument is persuasive.'

criteriaRubricCriterion1Description.ContentType(BodyType('text'))


criteriaRubricCriterion1.description = criteriaRubricCriterion1Description

criteriaArray []= criteriaRubricCriterion1;
criteriaRubricCriterion2 = RubricCriterion()
criteriaRubricCriterion2Description = EducationItemBody()
criteriaRubricCriterion2Description.content = 'The essay\'s argument does not make sense.'

criteriaRubricCriterion2Description.ContentType(BodyType('text'))


criteriaRubricCriterion2.description = criteriaRubricCriterion2Description

criteriaArray []= criteriaRubricCriterion2;
qualitiesRubricQuality1.criteria(criteriaArray)


qualitiesRubricQuality1.weight = 50.0


qualitiesArray []= qualitiesRubricQuality1;
qualitiesRubricQuality2 = RubricQuality()
qualitiesRubricQuality2Description = EducationItemBody()
qualitiesRubricQuality2Description.content = 'Spelling and Grammar'

qualitiesRubricQuality2Description.ContentType(BodyType('text'))


qualitiesRubricQuality2.description = qualitiesRubricQuality2Description
criteriaRubricCriterion1 = RubricCriterion()
criteriaRubricCriterion1Description = EducationItemBody()
criteriaRubricCriterion1Description.content = 'The essay uses proper spelling and grammar with few or no errors.'

criteriaRubricCriterion1Description.ContentType(BodyType('text'))


criteriaRubricCriterion1.description = criteriaRubricCriterion1Description

criteriaArray []= criteriaRubricCriterion1;
criteriaRubricCriterion2 = RubricCriterion()
criteriaRubricCriterion2Description = EducationItemBody()
criteriaRubricCriterion2Description.content = 'The essay has numerous errors in spelling and/or grammar.'

criteriaRubricCriterion2Description.ContentType(BodyType('text'))


criteriaRubricCriterion2.description = criteriaRubricCriterion2Description

criteriaArray []= criteriaRubricCriterion2;
qualitiesRubricQuality2.criteria(criteriaArray)


qualitiesRubricQuality2.weight = 50.0


qualitiesArray []= qualitiesRubricQuality2;
request_body.qualities(qualitiesArray)


grading = EducationAssignmentGradeType()
grading.@odatatype = '#microsoft.graph.educationAssignmentPointsGradeType'


request_body.grading = grading


request_configuration = RubricsRequestBuilderPostRequestConfiguration(
)


result = await client.education.me.rubrics.post(request_body = request_body)


```