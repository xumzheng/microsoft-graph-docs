---
description: "Automatically generated file. DO NOT MODIFY"
---

```python

// THE PYTHON SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
client =  GraphServiceClient(request_adapter)

request_body = PlannerTaskConfiguration()
request_body.@odatatype = '#microsoft.graph.plannerTaskConfiguration'

edit_policy = PlannerTaskPolicy()
rules_planner_task_role_based_rule1 = PlannerTaskRoleBasedRule()
rulesPlannerTaskRoleBasedRule1.defaultRule = 'block'

rules_planner_task_role_based_rule1_role = PlannerTaskConfigurationRoleBase()
rulesPlannerTaskRoleBasedRule1Role.@odatatype = '#microsoft.graph.plannerRelationshipBasedUserType'

rulesPlannerTaskRoleBasedRule1Role.RoleKind(PlannerUserRoleKind('relationship'))

additionalData = [
'role' => 'defaultRules', 
];
rulesPlannerTaskRoleBasedRule1Role.additionaldata(additionalData)



rulesPlannerTaskRoleBasedRule1.role = rulesPlannerTaskRoleBasedRule1Role
rules_planner_task_role_based_rule1_property_rule = PlannerTaskPropertyRule()
rulesPlannerTaskRoleBasedRule1PropertyRule.PercentComplete(['allow', ])

rulesPlannerTaskRoleBasedRule1PropertyRule.RuleKind(PlannerRuleKind('taskrule'))

rules_planner_task_role_based_rule1_property_rule_assignments = PlannerFieldRules()
rulesPlannerTaskRoleBasedRule1PropertyRuleAssignments.DefaultRules(['addSelf', ])

rulesPlannerTaskRoleBasedRule1PropertyRuleAssignments.Overrides([])


rulesPlannerTaskRoleBasedRule1PropertyRule.assignments = rulesPlannerTaskRoleBasedRule1PropertyRuleAssignments

rulesPlannerTaskRoleBasedRule1.property_rule = rulesPlannerTaskRoleBasedRule1PropertyRule

rulesArray []= rulesPlannerTaskRoleBasedRule1;
rules_planner_task_role_based_rule2 = PlannerTaskRoleBasedRule()
rulesPlannerTaskRoleBasedRule2.defaultRule = 'block'

rules_planner_task_role_based_rule2_role = PlannerTaskConfigurationRoleBase()
rulesPlannerTaskRoleBasedRule2Role.@odatatype = '#microsoft.graph.plannerRelationshipBasedUserType'

rulesPlannerTaskRoleBasedRule2Role.RoleKind(PlannerUserRoleKind('relationship'))

additionalData = [
'role' => 'taskAssignees', 
];
rulesPlannerTaskRoleBasedRule2Role.additionaldata(additionalData)



rulesPlannerTaskRoleBasedRule2.role = rulesPlannerTaskRoleBasedRule2Role
rules_planner_task_role_based_rule2_property_rule = PlannerTaskPropertyRule()
rulesPlannerTaskRoleBasedRule2PropertyRule.StartDate(['allow', ])

rulesPlannerTaskRoleBasedRule2PropertyRule.DueDate(['allow', ])

rulesPlannerTaskRoleBasedRule2PropertyRule.PercentComplete(['allow', ])

rulesPlannerTaskRoleBasedRule2PropertyRule.Order(['allow', ])

rulesPlannerTaskRoleBasedRule2PropertyRule.RuleKind(PlannerRuleKind('taskrule'))

rules_planner_task_role_based_rule2_property_rule_references = PlannerFieldRules()
rulesPlannerTaskRoleBasedRule2PropertyRuleReferences.DefaultRules(['allow', ])

overrides_planner_rule_override1 = PlannerRuleOverride()
overridesPlannerRuleOverride1.name = 'userCreated'

overridesPlannerRuleOverride1.Rules(['allow', ])


overridesArray []= overridesPlannerRuleOverride1;
overrides_planner_rule_override2 = PlannerRuleOverride()
overridesPlannerRuleOverride2.name = 'applicationCreated'

overridesPlannerRuleOverride2.Rules(['block', ])


overridesArray []= overridesPlannerRuleOverride2;
rulesPlannerTaskRoleBasedRule2PropertyRuleReferences.overrides(overridesArray)



rulesPlannerTaskRoleBasedRule2PropertyRule.references = rulesPlannerTaskRoleBasedRule2PropertyRuleReferences
rules_planner_task_role_based_rule2_property_rule_check_lists = PlannerFieldRules()
rulesPlannerTaskRoleBasedRule2PropertyRuleCheckLists.DefaultRules(['allow', ])

overrides_planner_rule_override1 = PlannerRuleOverride()
overridesPlannerRuleOverride1.name = 'userCreated'

overridesPlannerRuleOverride1.Rules(['allow', ])


overridesArray []= overridesPlannerRuleOverride1;
overrides_planner_rule_override2 = PlannerRuleOverride()
overridesPlannerRuleOverride2.name = 'applicationCreated'

overridesPlannerRuleOverride2.Rules(['check', ])


overridesArray []= overridesPlannerRuleOverride2;
rulesPlannerTaskRoleBasedRule2PropertyRuleCheckLists.overrides(overridesArray)



rulesPlannerTaskRoleBasedRule2PropertyRule.check_lists = rulesPlannerTaskRoleBasedRule2PropertyRuleCheckLists
rules_planner_task_role_based_rule2_property_rule_assignments = PlannerFieldRules()
rulesPlannerTaskRoleBasedRule2PropertyRuleAssignments.DefaultRules(['block', ])

overrides_planner_rule_override1 = PlannerRuleOverride()
overridesPlannerRuleOverride1.name = 'userCreated'

overridesPlannerRuleOverride1.Rules(['removeSelf', ])


overridesArray []= overridesPlannerRuleOverride1;
overrides_planner_rule_override2 = PlannerRuleOverride()
overridesPlannerRuleOverride2.name = 'applicationCreated'

overridesPlannerRuleOverride2.Rules(['check', ])


overridesArray []= overridesPlannerRuleOverride2;
rulesPlannerTaskRoleBasedRule2PropertyRuleAssignments.overrides(overridesArray)



rulesPlannerTaskRoleBasedRule2PropertyRule.assignments = rulesPlannerTaskRoleBasedRule2PropertyRuleAssignments
rules_planner_task_role_based_rule2_property_rule_applied_categories = PlannerFieldRules()
rulesPlannerTaskRoleBasedRule2PropertyRuleAppliedCategories.DefaultRules(['allow', ])

rulesPlannerTaskRoleBasedRule2PropertyRuleAppliedCategories.Overrides([])


rulesPlannerTaskRoleBasedRule2PropertyRule.applied_categories = rulesPlannerTaskRoleBasedRule2PropertyRuleAppliedCategories

rulesPlannerTaskRoleBasedRule2.property_rule = rulesPlannerTaskRoleBasedRule2PropertyRule

rulesArray []= rulesPlannerTaskRoleBasedRule2;
editPolicy.rules(rulesArray)



request_body.edit_policy = editPolicy



result = await client.solutions.businessScenarios_by_id('businessScenario-id').planner.taskConfiguration.patch(request_body = request_body)


```