---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerTaskConfiguration()
request_body.@odatatype = '#microsoft.graph.plannerTaskConfiguration'

editPolicy = PlannerTaskPolicy()
rulesPlannerTaskRoleBasedRule1 = PlannerTaskRoleBasedRule()
rulesPlannerTaskRoleBasedRule1.defaultRule = 'block'

rulesPlannerTaskRoleBasedRule1Role = PlannerTaskConfigurationRoleBase()
rulesPlannerTaskRoleBasedRule1Role.@odatatype = '#microsoft.graph.plannerRelationshipBasedUserType'

rulesPlannerTaskRoleBasedRule1Role.RoleKind(PlannerUserRoleKind('relationship'))

additionalData = [
'role' => 'defaultRules', 
];
rulesPlannerTaskRoleBasedRule1Role.additionaldata(additionalData)



rulesPlannerTaskRoleBasedRule1.role = rulesPlannerTaskRoleBasedRule1Role
rulesPlannerTaskRoleBasedRule1PropertyRule = PlannerTaskPropertyRule()
rulesPlannerTaskRoleBasedRule1PropertyRule.PercentComplete(['allow', ])

rulesPlannerTaskRoleBasedRule1PropertyRule.RuleKind(PlannerRuleKind('taskrule'))

rulesPlannerTaskRoleBasedRule1PropertyRuleAssignments = PlannerFieldRules()
rulesPlannerTaskRoleBasedRule1PropertyRuleAssignments.DefaultRules(['addSelf', ])

rulesPlannerTaskRoleBasedRule1PropertyRuleAssignments.Overrides([])


rulesPlannerTaskRoleBasedRule1PropertyRule.assignments = rulesPlannerTaskRoleBasedRule1PropertyRuleAssignments

rulesPlannerTaskRoleBasedRule1.propertyRule = rulesPlannerTaskRoleBasedRule1PropertyRule

rulesArray []= rulesPlannerTaskRoleBasedRule1;
rulesPlannerTaskRoleBasedRule2 = PlannerTaskRoleBasedRule()
rulesPlannerTaskRoleBasedRule2.defaultRule = 'block'

rulesPlannerTaskRoleBasedRule2Role = PlannerTaskConfigurationRoleBase()
rulesPlannerTaskRoleBasedRule2Role.@odatatype = '#microsoft.graph.plannerRelationshipBasedUserType'

rulesPlannerTaskRoleBasedRule2Role.RoleKind(PlannerUserRoleKind('relationship'))

additionalData = [
'role' => 'taskAssignees', 
];
rulesPlannerTaskRoleBasedRule2Role.additionaldata(additionalData)



rulesPlannerTaskRoleBasedRule2.role = rulesPlannerTaskRoleBasedRule2Role
rulesPlannerTaskRoleBasedRule2PropertyRule = PlannerTaskPropertyRule()
rulesPlannerTaskRoleBasedRule2PropertyRule.StartDate(['allow', ])

rulesPlannerTaskRoleBasedRule2PropertyRule.DueDate(['allow', ])

rulesPlannerTaskRoleBasedRule2PropertyRule.PercentComplete(['allow', ])

rulesPlannerTaskRoleBasedRule2PropertyRule.Order(['allow', ])

rulesPlannerTaskRoleBasedRule2PropertyRule.RuleKind(PlannerRuleKind('taskrule'))

rulesPlannerTaskRoleBasedRule2PropertyRuleReferences = PlannerFieldRules()
rulesPlannerTaskRoleBasedRule2PropertyRuleReferences.DefaultRules(['allow', ])

overridesPlannerRuleOverride1 = PlannerRuleOverride()
overridesPlannerRuleOverride1.name = 'userCreated'

overridesPlannerRuleOverride1.Rules(['allow', ])


overridesArray []= overridesPlannerRuleOverride1;
overridesPlannerRuleOverride2 = PlannerRuleOverride()
overridesPlannerRuleOverride2.name = 'applicationCreated'

overridesPlannerRuleOverride2.Rules(['block', ])


overridesArray []= overridesPlannerRuleOverride2;
rulesPlannerTaskRoleBasedRule2PropertyRuleReferences.overrides(overridesArray)



rulesPlannerTaskRoleBasedRule2PropertyRule.references = rulesPlannerTaskRoleBasedRule2PropertyRuleReferences
rulesPlannerTaskRoleBasedRule2PropertyRuleCheckLists = PlannerFieldRules()
rulesPlannerTaskRoleBasedRule2PropertyRuleCheckLists.DefaultRules(['allow', ])

overridesPlannerRuleOverride1 = PlannerRuleOverride()
overridesPlannerRuleOverride1.name = 'userCreated'

overridesPlannerRuleOverride1.Rules(['allow', ])


overridesArray []= overridesPlannerRuleOverride1;
overridesPlannerRuleOverride2 = PlannerRuleOverride()
overridesPlannerRuleOverride2.name = 'applicationCreated'

overridesPlannerRuleOverride2.Rules(['check', ])


overridesArray []= overridesPlannerRuleOverride2;
rulesPlannerTaskRoleBasedRule2PropertyRuleCheckLists.overrides(overridesArray)



rulesPlannerTaskRoleBasedRule2PropertyRule.checkLists = rulesPlannerTaskRoleBasedRule2PropertyRuleCheckLists
rulesPlannerTaskRoleBasedRule2PropertyRuleAssignments = PlannerFieldRules()
rulesPlannerTaskRoleBasedRule2PropertyRuleAssignments.DefaultRules(['block', ])

overridesPlannerRuleOverride1 = PlannerRuleOverride()
overridesPlannerRuleOverride1.name = 'userCreated'

overridesPlannerRuleOverride1.Rules(['removeSelf', ])


overridesArray []= overridesPlannerRuleOverride1;
overridesPlannerRuleOverride2 = PlannerRuleOverride()
overridesPlannerRuleOverride2.name = 'applicationCreated'

overridesPlannerRuleOverride2.Rules(['check', ])


overridesArray []= overridesPlannerRuleOverride2;
rulesPlannerTaskRoleBasedRule2PropertyRuleAssignments.overrides(overridesArray)



rulesPlannerTaskRoleBasedRule2PropertyRule.assignments = rulesPlannerTaskRoleBasedRule2PropertyRuleAssignments
rulesPlannerTaskRoleBasedRule2PropertyRuleAppliedCategories = PlannerFieldRules()
rulesPlannerTaskRoleBasedRule2PropertyRuleAppliedCategories.DefaultRules(['allow', ])

rulesPlannerTaskRoleBasedRule2PropertyRuleAppliedCategories.Overrides([])


rulesPlannerTaskRoleBasedRule2PropertyRule.appliedCategories = rulesPlannerTaskRoleBasedRule2PropertyRuleAppliedCategories

rulesPlannerTaskRoleBasedRule2.propertyRule = rulesPlannerTaskRoleBasedRule2PropertyRule

rulesArray []= rulesPlannerTaskRoleBasedRule2;
editPolicy.rules(rulesArray)



request_body.editPolicy = editPolicy


request_configuration = TaskConfigurationRequestBuilderPatchRequestConfiguration(
)


result = await client.solutions.businessScenarios_by_id('businessScenario-id').planner.taskConfiguration.patch(request_body = request_body)


```