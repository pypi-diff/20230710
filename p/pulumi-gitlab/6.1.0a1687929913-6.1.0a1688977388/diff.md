# Comparing `tmp/pulumi_gitlab-6.1.0a1687929913.tar.gz` & `tmp/pulumi_gitlab-6.1.0a1688977388.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_gitlab-6.1.0a1687929913.tar", last modified: Wed Jun 28 05:29:55 2023, max compression
+gzip compressed data, was "pulumi_gitlab-6.1.0a1688977388.tar", last modified: Mon Jul 10 08:27:57 2023, max compression
```

## Comparing `pulumi_gitlab-6.1.0a1687929913.tar` & `pulumi_gitlab-6.1.0a1688977388.tar`

### file list

```diff
@@ -1,140 +1,140 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:29:55.206578 pulumi_gitlab-6.1.0a1687929913/
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-28 05:29:55.206578 pulumi_gitlab-6.1.0a1687929913/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:29:55.206578 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/
--rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42471 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/application.py
--rw-r--r--   0 runner    (1001) docker     (123)   690759 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/application_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    19640 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/branch.py
--rw-r--r--   0 runner    (1001) docker     (123)    30927 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/branch_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/cluster_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)    19017 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/cluster_agent_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:29:55.206578 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    14100 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/deploy_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    15436 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/deploy_key_enable.py
--rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/deploy_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     7828 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_cluster_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_cluster_agents.py
--rw-r--r--   0 runner    (1001) docker     (123)     5938 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_current_user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12479 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    13528 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_group_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_group_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_group_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)    11541 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_group_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_group_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_group_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_instance_deploy_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     5812 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_instance_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_instance_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)    43520 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project.py
--rw-r--r--   0 runner    (1001) docker     (123)     4021 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_branches.py
--rw-r--r--   0 runner    (1001) docker     (123)    13666 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    24330 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)    30589 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_issues.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)     9546 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)     8568 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_milestones.py
--rw-r--r--   0 runner    (1001) docker     (123)     7308 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_protected_branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_protected_branches.py
--rw-r--r--   0 runner    (1001) docker     (123)     6221 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    24645 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_release_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4588 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_release_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     9411 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_repository_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6384 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_repository_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    16997 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     4219 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_user_sshkeys.py
--rw-r--r--   0 runner    (1001) docker     (123)    11124 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    68245 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_badge.py
--rw-r--r--   0 runner    (1001) docker     (123)    33679 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    46605 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    23721 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_ldap_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    20008 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_project_file_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_saml_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    14114 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_share_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    34419 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/instance_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    18253 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/instance_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    17060 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/integration_custom_issue_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    26646 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/integration_emails_on_push.py
--rw-r--r--   0 runner    (1001) docker     (123)    15426 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/integration_external_wiki.py
--rw-r--r--   0 runner    (1001) docker     (123)    19113 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/integration_github.py
--rw-r--r--   0 runner    (1001) docker     (123)    45241 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/integration_jira.py
--rw-r--r--   0 runner    (1001) docker     (123)    38076 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/integration_microsoft_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)    15604 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/integration_pipelines_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    59785 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/integration_slack.py
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/label.py
--rw-r--r--   0 runner    (1001) docker     (123)   165040 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22870 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/pages_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    20010 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/personal_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    13422 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/pipeline_schedule_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/pipeline_trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)   260430 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_access_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    24082 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_approval_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_badge.py
--rw-r--r--   0 runner    (1001) docker     (123)    36176 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_cluster.py
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    13423 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_freeze_period.py
--rw-r--r--   0 runner    (1001) docker     (123)    43374 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    73619 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_issue.py
--rw-r--r--   0 runner    (1001) docker     (123)    19661 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_issue_board.py
--rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_label.py
--rw-r--r--   0 runner    (1001) docker     (123)    24086 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_level_mr_approvals.py
--rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_membership.py
--rw-r--r--   0 runner    (1001) docker     (123)    25238 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_milestone.py
--rw-r--r--   0 runner    (1001) docker     (123)    17018 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_mirror.py
--rw-r--r--   0 runner    (1001) docker     (123)    19909 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_protected_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_runner_enablement.py
--rw-r--r--   0 runner    (1001) docker     (123)    15163 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_share_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    17670 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    23752 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    16592 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21523 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/release_link.py
--rw-r--r--   0 runner    (1001) docker     (123)    35168 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/repository_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24337 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/service_custom_issue_tracker.py
--rw-r--r--   0 runner    (1001) docker     (123)    26698 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/service_emails_on_push.py
--rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/service_external_wiki.py
--rw-r--r--   0 runner    (1001) docker     (123)    19121 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/service_github.py
--rw-r--r--   0 runner    (1001) docker     (123)    45261 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/service_jira.py
--rw-r--r--   0 runner    (1001) docker     (123)    38116 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/service_microsoft_teams.py
--rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/service_pipelines_email.py
--rw-r--r--   0 runner    (1001) docker     (123)    59807 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/service_slack.py
--rw-r--r--   0 runner    (1001) docker     (123)    21890 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/system_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10971 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/tag_protection.py
--rw-r--r--   0 runner    (1001) docker     (123)    20056 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/topic.py
--rw-r--r--   0 runner    (1001) docker     (123)    32444 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/user_custom_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/user_gpg_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/user_ssh_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 05:29:55.206578 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-06-28 05:29:55.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-06-28 05:29:55.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 05:29:55.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 05:29:55.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-28 05:29:55.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-28 05:29:55.000000 pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-28 05:29:55.206578 pulumi_gitlab-6.1.0a1687929913/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-06-28 05:29:54.000000 pulumi_gitlab-6.1.0a1687929913/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:27:57.665746 pulumi_gitlab-6.1.0a1688977388/
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-10 08:27:57.665746 pulumi_gitlab-6.1.0a1688977388/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:27:57.661746 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/
+-rw-r--r--   0 runner    (1001) docker     (123)    18023 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45582 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19364 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)   690759 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/application_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19640 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30857 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/branch_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13955 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/cluster_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21349 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/cluster_agent_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:27:57.665746 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14100 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/deploy_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15458 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/deploy_key_enable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19814 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/deploy_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4228 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7993 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_cluster_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4095 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_cluster_agents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_current_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_group_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_group_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6777 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11721 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_group_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_group_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5118 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_group_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5852 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_instance_deploy_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_instance_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_instance_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44465 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13966 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24930 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31009 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_issues.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_milestones.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_protected_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4539 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_protected_branches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6341 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6743 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24990 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_release_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_release_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9606 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6474 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_repository_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17432 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_user_sshkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11289 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68245 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23283 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13282 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_badge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33679 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10032 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46605 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24408 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_ldap_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20008 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12260 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_project_file_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_saml_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14114 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_share_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23002 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34419 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/instance_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18253 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/instance_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17060 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/integration_custom_issue_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26646 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/integration_emails_on_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15426 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/integration_external_wiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19113 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/integration_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45241 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/integration_jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38076 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/integration_microsoft_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15604 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/integration_pipelines_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60436 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/integration_slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)   168744 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22870 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/pages_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20010 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/personal_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17527 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12158 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/pipeline_schedule_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11100 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/pipeline_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)   262332 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_access_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24082 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_approval_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14991 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_badge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36176 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18418 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13423 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_freeze_period.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43374 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73619 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19661 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_issue_board.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14572 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_label.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24086 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_level_mr_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13988 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_membership.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25238 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_milestone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17018 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_mirror.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19909 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_protected_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9163 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_runner_enablement.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15850 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_share_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17670 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23752 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16592 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21523 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/release_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35168 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/repository_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28833 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17108 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/service_custom_issue_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26698 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/service_emails_on_push.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15462 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/service_external_wiki.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19121 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/service_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45261 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/service_jira.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38116 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/service_microsoft_teams.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15644 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/service_pipelines_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60458 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/service_slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21890 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/system_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14208 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/tag_protection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20899 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/topic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32444 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/user_custom_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/user_gpg_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15296 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/user_ssh_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 08:27:57.665746 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4558 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 08:27:57.665746 pulumi_gitlab-6.1.0a1688977388/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-10 08:27:57.000000 pulumi_gitlab-6.1.0a1688977388/setup.py
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/PKG-INFO` & `pulumi_gitlab-6.1.0a1688977388/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_gitlab
-Version: 6.1.0a1687929913
+Version: 6.1.0a1688977388
 Summary: A Pulumi package for creating and managing GitLab resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-gitlab
 Keywords: pulumi gitlab
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/README.md` & `pulumi_gitlab-6.1.0a1688977388/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/__init__.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/_inputs.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/_inputs.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     'ProjectContainerExpirationPolicyArgs',
     'ProjectIssueBoardListArgs',
     'ProjectIssueTaskCompletionStatusArgs',
     'ProjectProtectedEnvironmentDeployAccessLevelArgs',
     'ProjectPushRulesArgs',
     'ProjectTagCommitArgs',
     'ProjectTagReleaseArgs',
+    'TagProtectionAllowedToCreateArgs',
 ]
 
 @pulumi.input_type
 class BranchCommitArgs:
     def __init__(__self__, *,
                  author_email: Optional[pulumi.Input[str]] = None,
                  author_name: Optional[pulumi.Input[str]] = None,
@@ -403,19 +404,19 @@
         if cadence is not None:
             pulumi.set(__self__, "cadence", cadence)
         if enabled is not None:
             pulumi.set(__self__, "enabled", enabled)
         if keep_n is not None:
             pulumi.set(__self__, "keep_n", keep_n)
         if name_regex is not None:
+            warnings.warn("""`name_regex` has been deprecated. Use `name_regex_delete` instead.""", DeprecationWarning)
+            pulumi.log.warn("""name_regex is deprecated: `name_regex` has been deprecated. Use `name_regex_delete` instead.""")
+        if name_regex is not None:
             pulumi.set(__self__, "name_regex", name_regex)
         if name_regex_delete is not None:
-            warnings.warn("""`name_regex_delete` has been deprecated. Use `name_regex` instead.""", DeprecationWarning)
-            pulumi.log.warn("""name_regex_delete is deprecated: `name_regex_delete` has been deprecated. Use `name_regex` instead.""")
-        if name_regex_delete is not None:
             pulumi.set(__self__, "name_regex_delete", name_regex_delete)
         if name_regex_keep is not None:
             pulumi.set(__self__, "name_regex_keep", name_regex_keep)
         if next_run_at is not None:
             pulumi.set(__self__, "next_run_at", next_run_at)
         if older_than is not None:
             pulumi.set(__self__, "older_than", older_than)
@@ -458,14 +459,17 @@
 
     @property
     @pulumi.getter(name="nameRegex")
     def name_regex(self) -> Optional[pulumi.Input[str]]:
         """
         The regular expression to match image names to delete.
         """
+        warnings.warn("""`name_regex` has been deprecated. Use `name_regex_delete` instead.""", DeprecationWarning)
+        pulumi.log.warn("""name_regex is deprecated: `name_regex` has been deprecated. Use `name_regex_delete` instead.""")
+
         return pulumi.get(self, "name_regex")
 
     @name_regex.setter
     def name_regex(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name_regex", value)
 
     @property
@@ -1075,7 +1079,78 @@
         return pulumi.get(self, "tag_name")
 
     @tag_name.setter
     def tag_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "tag_name", value)
 
 
+@pulumi.input_type
+class TagProtectionAllowedToCreateArgs:
+    def __init__(__self__, *,
+                 access_level: Optional[pulumi.Input[str]] = None,
+                 access_level_description: Optional[pulumi.Input[str]] = None,
+                 group_id: Optional[pulumi.Input[int]] = None,
+                 user_id: Optional[pulumi.Input[int]] = None):
+        """
+        :param pulumi.Input[str] access_level: Level of access.
+        :param pulumi.Input[str] access_level_description: Readable description of level of access.
+        :param pulumi.Input[int] group_id: The ID of a GitLab group allowed to perform the relevant action. Mutually exclusive with `user_id`.
+        :param pulumi.Input[int] user_id: The ID of a GitLab user allowed to perform the relevant action. Mutually exclusive with `group_id`.
+        """
+        if access_level is not None:
+            pulumi.set(__self__, "access_level", access_level)
+        if access_level_description is not None:
+            pulumi.set(__self__, "access_level_description", access_level_description)
+        if group_id is not None:
+            pulumi.set(__self__, "group_id", group_id)
+        if user_id is not None:
+            pulumi.set(__self__, "user_id", user_id)
+
+    @property
+    @pulumi.getter(name="accessLevel")
+    def access_level(self) -> Optional[pulumi.Input[str]]:
+        """
+        Level of access.
+        """
+        return pulumi.get(self, "access_level")
+
+    @access_level.setter
+    def access_level(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "access_level", value)
+
+    @property
+    @pulumi.getter(name="accessLevelDescription")
+    def access_level_description(self) -> Optional[pulumi.Input[str]]:
+        """
+        Readable description of level of access.
+        """
+        return pulumi.get(self, "access_level_description")
+
+    @access_level_description.setter
+    def access_level_description(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "access_level_description", value)
+
+    @property
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> Optional[pulumi.Input[int]]:
+        """
+        The ID of a GitLab group allowed to perform the relevant action. Mutually exclusive with `user_id`.
+        """
+        return pulumi.get(self, "group_id")
+
+    @group_id.setter
+    def group_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "group_id", value)
+
+    @property
+    @pulumi.getter(name="userId")
+    def user_id(self) -> Optional[pulumi.Input[int]]:
+        """
+        The ID of a GitLab user allowed to perform the relevant action. Mutually exclusive with `group_id`.
+        """
+        return pulumi.get(self, "user_id")
+
+    @user_id.setter
+    def user_id(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "user_id", value)
+
+
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/_utilities.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/application.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/application.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/application_settings.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/application_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/branch.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/branch.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/branch_protection.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/branch_protection.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         :param pulumi.Input[bool] allow_force_push: Can be set to true to allow users with push access to force push.
         :param pulumi.Input[Sequence[pulumi.Input['BranchProtectionAllowedToMergeArgs']]] allowed_to_merges: Defines permissions for action.
         :param pulumi.Input[Sequence[pulumi.Input['BranchProtectionAllowedToPushArgs']]] allowed_to_pushes: Defines permissions for action.
         :param pulumi.Input[Sequence[pulumi.Input['BranchProtectionAllowedToUnprotectArgs']]] allowed_to_unprotects: Defines permissions for action.
         :param pulumi.Input[bool] code_owner_approval_required: Can be set to true to require code owner approval before merging. Only available own Premium and Ultimate instances.
         :param pulumi.Input[str] merge_access_level: Access levels allowed to merge. Valid values are: `no one`, `developer`, `maintainer`.
         :param pulumi.Input[str] push_access_level: Access levels allowed to push. Valid values are: `no one`, `developer`, `maintainer`.
-        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `no one`, `developer`, `maintainer`.
+        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
         """
         pulumi.set(__self__, "branch", branch)
         pulumi.set(__self__, "project", project)
         if allow_force_push is not None:
             pulumi.set(__self__, "allow_force_push", allow_force_push)
         if allowed_to_merges is not None:
             pulumi.set(__self__, "allowed_to_merges", allowed_to_merges)
@@ -166,15 +166,15 @@
     def push_access_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "push_access_level", value)
 
     @property
     @pulumi.getter(name="unprotectAccessLevel")
     def unprotect_access_level(self) -> Optional[pulumi.Input[str]]:
         """
-        Access levels allowed to unprotect. Valid values are: `no one`, `developer`, `maintainer`.
+        Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
         """
         return pulumi.get(self, "unprotect_access_level")
 
     @unprotect_access_level.setter
     def unprotect_access_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "unprotect_access_level", value)
 
@@ -201,15 +201,15 @@
         :param pulumi.Input[Sequence[pulumi.Input['BranchProtectionAllowedToUnprotectArgs']]] allowed_to_unprotects: Defines permissions for action.
         :param pulumi.Input[str] branch: Name of the branch.
         :param pulumi.Input[int] branch_protection_id: The ID of the branch protection (not the branch name).
         :param pulumi.Input[bool] code_owner_approval_required: Can be set to true to require code owner approval before merging. Only available own Premium and Ultimate instances.
         :param pulumi.Input[str] merge_access_level: Access levels allowed to merge. Valid values are: `no one`, `developer`, `maintainer`.
         :param pulumi.Input[str] project: The id of the project.
         :param pulumi.Input[str] push_access_level: Access levels allowed to push. Valid values are: `no one`, `developer`, `maintainer`.
-        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `no one`, `developer`, `maintainer`.
+        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
         """
         if allow_force_push is not None:
             pulumi.set(__self__, "allow_force_push", allow_force_push)
         if allowed_to_merges is not None:
             pulumi.set(__self__, "allowed_to_merges", allowed_to_merges)
         if allowed_to_pushes is not None:
             pulumi.set(__self__, "allowed_to_pushes", allowed_to_pushes)
@@ -350,15 +350,15 @@
     def push_access_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "push_access_level", value)
 
     @property
     @pulumi.getter(name="unprotectAccessLevel")
     def unprotect_access_level(self) -> Optional[pulumi.Input[str]]:
         """
-        Access levels allowed to unprotect. Valid values are: `no one`, `developer`, `maintainer`.
+        Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
         """
         return pulumi.get(self, "unprotect_access_level")
 
     @unprotect_access_level.setter
     def unprotect_access_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "unprotect_access_level", value)
 
@@ -395,15 +395,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BranchProtectionAllowedToPushArgs']]]] allowed_to_pushes: Defines permissions for action.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BranchProtectionAllowedToUnprotectArgs']]]] allowed_to_unprotects: Defines permissions for action.
         :param pulumi.Input[str] branch: Name of the branch.
         :param pulumi.Input[bool] code_owner_approval_required: Can be set to true to require code owner approval before merging. Only available own Premium and Ultimate instances.
         :param pulumi.Input[str] merge_access_level: Access levels allowed to merge. Valid values are: `no one`, `developer`, `maintainer`.
         :param pulumi.Input[str] project: The id of the project.
         :param pulumi.Input[str] push_access_level: Access levels allowed to push. Valid values are: `no one`, `developer`, `maintainer`.
-        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `no one`, `developer`, `maintainer`.
+        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: BranchProtectionArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -499,15 +499,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['BranchProtectionAllowedToUnprotectArgs']]]] allowed_to_unprotects: Defines permissions for action.
         :param pulumi.Input[str] branch: Name of the branch.
         :param pulumi.Input[int] branch_protection_id: The ID of the branch protection (not the branch name).
         :param pulumi.Input[bool] code_owner_approval_required: Can be set to true to require code owner approval before merging. Only available own Premium and Ultimate instances.
         :param pulumi.Input[str] merge_access_level: Access levels allowed to merge. Valid values are: `no one`, `developer`, `maintainer`.
         :param pulumi.Input[str] project: The id of the project.
         :param pulumi.Input[str] push_access_level: Access levels allowed to push. Valid values are: `no one`, `developer`, `maintainer`.
-        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `no one`, `developer`, `maintainer`.
+        :param pulumi.Input[str] unprotect_access_level: Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _BranchProtectionState.__new__(_BranchProtectionState)
 
         __props__.__dict__["allow_force_push"] = allow_force_push
         __props__.__dict__["allowed_to_merges"] = allowed_to_merges
@@ -602,11 +602,11 @@
         """
         return pulumi.get(self, "push_access_level")
 
     @property
     @pulumi.getter(name="unprotectAccessLevel")
     def unprotect_access_level(self) -> pulumi.Output[Optional[str]]:
         """
-        Access levels allowed to unprotect. Valid values are: `no one`, `developer`, `maintainer`.
+        Access levels allowed to unprotect. Valid values are: `developer`, `maintainer`.
         """
         return pulumi.get(self, "unprotect_access_level")
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/cluster_agent.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/cluster_agent.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/cluster_agent_token.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_tag.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,485 +4,453 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
+from ._inputs import *
 
-__all__ = ['ClusterAgentTokenArgs', 'ClusterAgentToken']
+__all__ = ['ProjectTagArgs', 'ProjectTag']
 
 @pulumi.input_type
-class ClusterAgentTokenArgs:
+class ProjectTagArgs:
     def __init__(__self__, *,
-                 agent_id: pulumi.Input[int],
                  project: pulumi.Input[str],
-                 description: Optional[pulumi.Input[str]] = None,
+                 ref: pulumi.Input[str],
+                 message: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None):
         """
-        The set of arguments for constructing a ClusterAgentToken resource.
-        :param pulumi.Input[int] agent_id: The ID of the agent.
-        :param pulumi.Input[str] project: ID or full path of the project maintained by the authenticated user.
-        :param pulumi.Input[str] description: The Description for the agent.
-        :param pulumi.Input[str] name: The Name of the agent.
+        The set of arguments for constructing a ProjectTag resource.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of the project owned by the authenticated user.
+        :param pulumi.Input[str] ref: Create tag using commit SHA, another tag name, or branch name. This attribute is not available for imported resources.
+        :param pulumi.Input[str] message: The message of the annotated tag.
+        :param pulumi.Input[str] name: The name of a tag.
         """
-        pulumi.set(__self__, "agent_id", agent_id)
         pulumi.set(__self__, "project", project)
-        if description is not None:
-            pulumi.set(__self__, "description", description)
+        pulumi.set(__self__, "ref", ref)
+        if message is not None:
+            pulumi.set(__self__, "message", message)
         if name is not None:
             pulumi.set(__self__, "name", name)
 
     @property
-    @pulumi.getter(name="agentId")
-    def agent_id(self) -> pulumi.Input[int]:
-        """
-        The ID of the agent.
-        """
-        return pulumi.get(self, "agent_id")
-
-    @agent_id.setter
-    def agent_id(self, value: pulumi.Input[int]):
-        pulumi.set(self, "agent_id", value)
-
-    @property
     @pulumi.getter
     def project(self) -> pulumi.Input[str]:
         """
-        ID or full path of the project maintained by the authenticated user.
+        The ID or URL-encoded path of the project owned by the authenticated user.
         """
         return pulumi.get(self, "project")
 
     @project.setter
     def project(self, value: pulumi.Input[str]):
         pulumi.set(self, "project", value)
 
     @property
     @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
+    def ref(self) -> pulumi.Input[str]:
+        """
+        Create tag using commit SHA, another tag name, or branch name. This attribute is not available for imported resources.
+        """
+        return pulumi.get(self, "ref")
+
+    @ref.setter
+    def ref(self, value: pulumi.Input[str]):
+        pulumi.set(self, "ref", value)
+
+    @property
+    @pulumi.getter
+    def message(self) -> Optional[pulumi.Input[str]]:
         """
-        The Description for the agent.
+        The message of the annotated tag.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "message")
 
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
+    @message.setter
+    def message(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "message", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The Name of the agent.
+        The name of a tag.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
 
 @pulumi.input_type
-class _ClusterAgentTokenState:
+class _ProjectTagState:
     def __init__(__self__, *,
-                 agent_id: Optional[pulumi.Input[int]] = None,
-                 created_at: Optional[pulumi.Input[str]] = None,
-                 created_by_user_id: Optional[pulumi.Input[int]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
-                 last_used_at: Optional[pulumi.Input[str]] = None,
+                 commits: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTagCommitArgs']]]] = None,
+                 message: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
-                 status: Optional[pulumi.Input[str]] = None,
-                 token: Optional[pulumi.Input[str]] = None,
-                 token_id: Optional[pulumi.Input[int]] = None):
-        """
-        Input properties used for looking up and filtering ClusterAgentToken resources.
-        :param pulumi.Input[int] agent_id: The ID of the agent.
-        :param pulumi.Input[str] created_at: The ISO8601 datetime when the agent was created.
-        :param pulumi.Input[int] created_by_user_id: The ID of the user who created the agent.
-        :param pulumi.Input[str] description: The Description for the agent.
-        :param pulumi.Input[str] last_used_at: The ISO8601 datetime when the token was last used.
-        :param pulumi.Input[str] name: The Name of the agent.
-        :param pulumi.Input[str] project: ID or full path of the project maintained by the authenticated user.
-        :param pulumi.Input[str] status: The status of the token. Valid values are `active`, `revoked`.
-        :param pulumi.Input[str] token: The secret token for the agent. The `token` is not available in imported resources.
-        :param pulumi.Input[int] token_id: The ID of the token.
-        """
-        if agent_id is not None:
-            pulumi.set(__self__, "agent_id", agent_id)
-        if created_at is not None:
-            pulumi.set(__self__, "created_at", created_at)
-        if created_by_user_id is not None:
-            pulumi.set(__self__, "created_by_user_id", created_by_user_id)
-        if description is not None:
-            pulumi.set(__self__, "description", description)
-        if last_used_at is not None:
-            pulumi.set(__self__, "last_used_at", last_used_at)
+                 protected: Optional[pulumi.Input[bool]] = None,
+                 ref: Optional[pulumi.Input[str]] = None,
+                 releases: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTagReleaseArgs']]]] = None,
+                 target: Optional[pulumi.Input[str]] = None):
+        """
+        Input properties used for looking up and filtering ProjectTag resources.
+        :param pulumi.Input[Sequence[pulumi.Input['ProjectTagCommitArgs']]] commits: The commit associated with the tag.
+        :param pulumi.Input[str] message: The message of the annotated tag.
+        :param pulumi.Input[str] name: The name of a tag.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of the project owned by the authenticated user.
+        :param pulumi.Input[bool] protected: Bool, true if tag has tag protection.
+        :param pulumi.Input[str] ref: Create tag using commit SHA, another tag name, or branch name. This attribute is not available for imported resources.
+        :param pulumi.Input[Sequence[pulumi.Input['ProjectTagReleaseArgs']]] releases: The release associated with the tag.
+        :param pulumi.Input[str] target: The unique id assigned to the commit by Gitlab.
+        """
+        if commits is not None:
+            pulumi.set(__self__, "commits", commits)
+        if message is not None:
+            pulumi.set(__self__, "message", message)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if project is not None:
             pulumi.set(__self__, "project", project)
-        if status is not None:
-            pulumi.set(__self__, "status", status)
-        if token is not None:
-            pulumi.set(__self__, "token", token)
-        if token_id is not None:
-            pulumi.set(__self__, "token_id", token_id)
-
-    @property
-    @pulumi.getter(name="agentId")
-    def agent_id(self) -> Optional[pulumi.Input[int]]:
-        """
-        The ID of the agent.
-        """
-        return pulumi.get(self, "agent_id")
-
-    @agent_id.setter
-    def agent_id(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "agent_id", value)
-
-    @property
-    @pulumi.getter(name="createdAt")
-    def created_at(self) -> Optional[pulumi.Input[str]]:
-        """
-        The ISO8601 datetime when the agent was created.
-        """
-        return pulumi.get(self, "created_at")
-
-    @created_at.setter
-    def created_at(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "created_at", value)
-
-    @property
-    @pulumi.getter(name="createdByUserId")
-    def created_by_user_id(self) -> Optional[pulumi.Input[int]]:
-        """
-        The ID of the user who created the agent.
-        """
-        return pulumi.get(self, "created_by_user_id")
-
-    @created_by_user_id.setter
-    def created_by_user_id(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "created_by_user_id", value)
+        if protected is not None:
+            pulumi.set(__self__, "protected", protected)
+        if ref is not None:
+            pulumi.set(__self__, "ref", ref)
+        if releases is not None:
+            pulumi.set(__self__, "releases", releases)
+        if target is not None:
+            pulumi.set(__self__, "target", target)
 
     @property
     @pulumi.getter
-    def description(self) -> Optional[pulumi.Input[str]]:
+    def commits(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTagCommitArgs']]]]:
         """
-        The Description for the agent.
+        The commit associated with the tag.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "commits")
 
-    @description.setter
-    def description(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "description", value)
+    @commits.setter
+    def commits(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTagCommitArgs']]]]):
+        pulumi.set(self, "commits", value)
 
     @property
-    @pulumi.getter(name="lastUsedAt")
-    def last_used_at(self) -> Optional[pulumi.Input[str]]:
+    @pulumi.getter
+    def message(self) -> Optional[pulumi.Input[str]]:
         """
-        The ISO8601 datetime when the token was last used.
+        The message of the annotated tag.
         """
-        return pulumi.get(self, "last_used_at")
+        return pulumi.get(self, "message")
 
-    @last_used_at.setter
-    def last_used_at(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "last_used_at", value)
+    @message.setter
+    def message(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "message", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The Name of the agent.
+        The name of a tag.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
     @property
     @pulumi.getter
     def project(self) -> Optional[pulumi.Input[str]]:
         """
-        ID or full path of the project maintained by the authenticated user.
+        The ID or URL-encoded path of the project owned by the authenticated user.
         """
         return pulumi.get(self, "project")
 
     @project.setter
     def project(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "project", value)
 
     @property
     @pulumi.getter
-    def status(self) -> Optional[pulumi.Input[str]]:
+    def protected(self) -> Optional[pulumi.Input[bool]]:
         """
-        The status of the token. Valid values are `active`, `revoked`.
+        Bool, true if tag has tag protection.
         """
-        return pulumi.get(self, "status")
+        return pulumi.get(self, "protected")
 
-    @status.setter
-    def status(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "status", value)
+    @protected.setter
+    def protected(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "protected", value)
 
     @property
     @pulumi.getter
-    def token(self) -> Optional[pulumi.Input[str]]:
+    def ref(self) -> Optional[pulumi.Input[str]]:
         """
-        The secret token for the agent. The `token` is not available in imported resources.
+        Create tag using commit SHA, another tag name, or branch name. This attribute is not available for imported resources.
         """
-        return pulumi.get(self, "token")
+        return pulumi.get(self, "ref")
 
-    @token.setter
-    def token(self, value: Optional[pulumi.Input[str]]):
-        pulumi.set(self, "token", value)
+    @ref.setter
+    def ref(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "ref", value)
 
     @property
-    @pulumi.getter(name="tokenId")
-    def token_id(self) -> Optional[pulumi.Input[int]]:
+    @pulumi.getter
+    def releases(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTagReleaseArgs']]]]:
         """
-        The ID of the token.
+        The release associated with the tag.
         """
-        return pulumi.get(self, "token_id")
+        return pulumi.get(self, "releases")
 
-    @token_id.setter
-    def token_id(self, value: Optional[pulumi.Input[int]]):
-        pulumi.set(self, "token_id", value)
+    @releases.setter
+    def releases(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['ProjectTagReleaseArgs']]]]):
+        pulumi.set(self, "releases", value)
 
+    @property
+    @pulumi.getter
+    def target(self) -> Optional[pulumi.Input[str]]:
+        """
+        The unique id assigned to the commit by Gitlab.
+        """
+        return pulumi.get(self, "target")
 
-class ClusterAgentToken(pulumi.CustomResource):
+    @target.setter
+    def target(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "target", value)
+
+
+class ProjectTag(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 agent_id: Optional[pulumi.Input[int]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
+                 message: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
+                 ref: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The `ClusterAgentToken` resource allows to manage the lifecycle of a token for a GitLab Agent for Kubernetes.
+        The `ProjectTag` resource allows to manage the lifecycle of a tag in a project.
 
-        > Requires at least maintainer permissions on the project.
+        **Upstream API**: [GitLab API docs](https://docs.gitlab.com/ee/api/tags.html)
 
-        > Requires at least GitLab 15.0
+        ## Example Usage
 
-        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/cluster_agents.html#create-an-agent-token)
+        ```python
+        import pulumi
+        import pulumi_gitlab as gitlab
+
+        # Create a project for the tag to use
+        example_project = gitlab.Project("exampleProject",
+            description="An example project",
+            namespace_id=gitlab_group["example"]["id"])
+        example_project_tag = gitlab.ProjectTag("exampleProjectTag",
+            ref="main",
+            project=example_project.id)
+        ```
 
         ## Import
 
-        A token for a GitLab Agent for Kubernetes can be imported with the following command and the id pattern `<project>:<agent-id>:<token-id>`
+        Gitlab project tags can be imported with a key composed of `<project_id>:<tag_name>`, e.g.
 
         ```sh
-         $ pulumi import gitlab:index/clusterAgentToken:ClusterAgentToken example '12345:42:1'
+         $ pulumi import gitlab:index/projectTag:ProjectTag example "12345:develop"
         ```
 
-         ATTENTIONthe `token` resource attribute is not available for imported resources as this information cannot be read from the GitLab API.
+         NOTEthe `ref` attribute won't be available for imported `gitlab_project_tag` resources.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[int] agent_id: The ID of the agent.
-        :param pulumi.Input[str] description: The Description for the agent.
-        :param pulumi.Input[str] name: The Name of the agent.
-        :param pulumi.Input[str] project: ID or full path of the project maintained by the authenticated user.
+        :param pulumi.Input[str] message: The message of the annotated tag.
+        :param pulumi.Input[str] name: The name of a tag.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of the project owned by the authenticated user.
+        :param pulumi.Input[str] ref: Create tag using commit SHA, another tag name, or branch name. This attribute is not available for imported resources.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
-                 args: ClusterAgentTokenArgs,
+                 args: ProjectTagArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The `ClusterAgentToken` resource allows to manage the lifecycle of a token for a GitLab Agent for Kubernetes.
+        The `ProjectTag` resource allows to manage the lifecycle of a tag in a project.
 
-        > Requires at least maintainer permissions on the project.
+        **Upstream API**: [GitLab API docs](https://docs.gitlab.com/ee/api/tags.html)
 
-        > Requires at least GitLab 15.0
+        ## Example Usage
 
-        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/cluster_agents.html#create-an-agent-token)
+        ```python
+        import pulumi
+        import pulumi_gitlab as gitlab
+
+        # Create a project for the tag to use
+        example_project = gitlab.Project("exampleProject",
+            description="An example project",
+            namespace_id=gitlab_group["example"]["id"])
+        example_project_tag = gitlab.ProjectTag("exampleProjectTag",
+            ref="main",
+            project=example_project.id)
+        ```
 
         ## Import
 
-        A token for a GitLab Agent for Kubernetes can be imported with the following command and the id pattern `<project>:<agent-id>:<token-id>`
+        Gitlab project tags can be imported with a key composed of `<project_id>:<tag_name>`, e.g.
 
         ```sh
-         $ pulumi import gitlab:index/clusterAgentToken:ClusterAgentToken example '12345:42:1'
+         $ pulumi import gitlab:index/projectTag:ProjectTag example "12345:develop"
         ```
 
-         ATTENTIONthe `token` resource attribute is not available for imported resources as this information cannot be read from the GitLab API.
+         NOTEthe `ref` attribute won't be available for imported `gitlab_project_tag` resources.
 
         :param str resource_name: The name of the resource.
-        :param ClusterAgentTokenArgs args: The arguments to use to populate this resource's properties.
+        :param ProjectTagArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
-        resource_args, opts = _utilities.get_resource_args_opts(ClusterAgentTokenArgs, pulumi.ResourceOptions, *args, **kwargs)
+        resource_args, opts = _utilities.get_resource_args_opts(ProjectTagArgs, pulumi.ResourceOptions, *args, **kwargs)
         if resource_args is not None:
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
-                 agent_id: Optional[pulumi.Input[int]] = None,
-                 description: Optional[pulumi.Input[str]] = None,
+                 message: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
+                 ref: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
-            __props__ = ClusterAgentTokenArgs.__new__(ClusterAgentTokenArgs)
+            __props__ = ProjectTagArgs.__new__(ProjectTagArgs)
 
-            if agent_id is None and not opts.urn:
-                raise TypeError("Missing required property 'agent_id'")
-            __props__.__dict__["agent_id"] = agent_id
-            __props__.__dict__["description"] = description
+            __props__.__dict__["message"] = message
             __props__.__dict__["name"] = name
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
-            __props__.__dict__["created_at"] = None
-            __props__.__dict__["created_by_user_id"] = None
-            __props__.__dict__["last_used_at"] = None
-            __props__.__dict__["status"] = None
-            __props__.__dict__["token"] = None
-            __props__.__dict__["token_id"] = None
-        super(ClusterAgentToken, __self__).__init__(
-            'gitlab:index/clusterAgentToken:ClusterAgentToken',
+            if ref is None and not opts.urn:
+                raise TypeError("Missing required property 'ref'")
+            __props__.__dict__["ref"] = ref
+            __props__.__dict__["commits"] = None
+            __props__.__dict__["protected"] = None
+            __props__.__dict__["releases"] = None
+            __props__.__dict__["target"] = None
+        super(ProjectTag, __self__).__init__(
+            'gitlab:index/projectTag:ProjectTag',
             resource_name,
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
-            agent_id: Optional[pulumi.Input[int]] = None,
-            created_at: Optional[pulumi.Input[str]] = None,
-            created_by_user_id: Optional[pulumi.Input[int]] = None,
-            description: Optional[pulumi.Input[str]] = None,
-            last_used_at: Optional[pulumi.Input[str]] = None,
+            commits: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectTagCommitArgs']]]]] = None,
+            message: Optional[pulumi.Input[str]] = None,
             name: Optional[pulumi.Input[str]] = None,
             project: Optional[pulumi.Input[str]] = None,
-            status: Optional[pulumi.Input[str]] = None,
-            token: Optional[pulumi.Input[str]] = None,
-            token_id: Optional[pulumi.Input[int]] = None) -> 'ClusterAgentToken':
+            protected: Optional[pulumi.Input[bool]] = None,
+            ref: Optional[pulumi.Input[str]] = None,
+            releases: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectTagReleaseArgs']]]]] = None,
+            target: Optional[pulumi.Input[str]] = None) -> 'ProjectTag':
         """
-        Get an existing ClusterAgentToken resource's state with the given name, id, and optional extra
+        Get an existing ProjectTag resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[int] agent_id: The ID of the agent.
-        :param pulumi.Input[str] created_at: The ISO8601 datetime when the agent was created.
-        :param pulumi.Input[int] created_by_user_id: The ID of the user who created the agent.
-        :param pulumi.Input[str] description: The Description for the agent.
-        :param pulumi.Input[str] last_used_at: The ISO8601 datetime when the token was last used.
-        :param pulumi.Input[str] name: The Name of the agent.
-        :param pulumi.Input[str] project: ID or full path of the project maintained by the authenticated user.
-        :param pulumi.Input[str] status: The status of the token. Valid values are `active`, `revoked`.
-        :param pulumi.Input[str] token: The secret token for the agent. The `token` is not available in imported resources.
-        :param pulumi.Input[int] token_id: The ID of the token.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectTagCommitArgs']]]] commits: The commit associated with the tag.
+        :param pulumi.Input[str] message: The message of the annotated tag.
+        :param pulumi.Input[str] name: The name of a tag.
+        :param pulumi.Input[str] project: The ID or URL-encoded path of the project owned by the authenticated user.
+        :param pulumi.Input[bool] protected: Bool, true if tag has tag protection.
+        :param pulumi.Input[str] ref: Create tag using commit SHA, another tag name, or branch name. This attribute is not available for imported resources.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['ProjectTagReleaseArgs']]]] releases: The release associated with the tag.
+        :param pulumi.Input[str] target: The unique id assigned to the commit by Gitlab.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
-        __props__ = _ClusterAgentTokenState.__new__(_ClusterAgentTokenState)
+        __props__ = _ProjectTagState.__new__(_ProjectTagState)
 
-        __props__.__dict__["agent_id"] = agent_id
-        __props__.__dict__["created_at"] = created_at
-        __props__.__dict__["created_by_user_id"] = created_by_user_id
-        __props__.__dict__["description"] = description
-        __props__.__dict__["last_used_at"] = last_used_at
+        __props__.__dict__["commits"] = commits
+        __props__.__dict__["message"] = message
         __props__.__dict__["name"] = name
         __props__.__dict__["project"] = project
-        __props__.__dict__["status"] = status
-        __props__.__dict__["token"] = token
-        __props__.__dict__["token_id"] = token_id
-        return ClusterAgentToken(resource_name, opts=opts, __props__=__props__)
-
-    @property
-    @pulumi.getter(name="agentId")
-    def agent_id(self) -> pulumi.Output[int]:
-        """
-        The ID of the agent.
-        """
-        return pulumi.get(self, "agent_id")
-
-    @property
-    @pulumi.getter(name="createdAt")
-    def created_at(self) -> pulumi.Output[str]:
-        """
-        The ISO8601 datetime when the agent was created.
-        """
-        return pulumi.get(self, "created_at")
-
-    @property
-    @pulumi.getter(name="createdByUserId")
-    def created_by_user_id(self) -> pulumi.Output[int]:
-        """
-        The ID of the user who created the agent.
-        """
-        return pulumi.get(self, "created_by_user_id")
+        __props__.__dict__["protected"] = protected
+        __props__.__dict__["ref"] = ref
+        __props__.__dict__["releases"] = releases
+        __props__.__dict__["target"] = target
+        return ProjectTag(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter
-    def description(self) -> pulumi.Output[Optional[str]]:
+    def commits(self) -> pulumi.Output[Sequence['outputs.ProjectTagCommit']]:
         """
-        The Description for the agent.
+        The commit associated with the tag.
         """
-        return pulumi.get(self, "description")
+        return pulumi.get(self, "commits")
 
     @property
-    @pulumi.getter(name="lastUsedAt")
-    def last_used_at(self) -> pulumi.Output[str]:
+    @pulumi.getter
+    def message(self) -> pulumi.Output[Optional[str]]:
         """
-        The ISO8601 datetime when the token was last used.
+        The message of the annotated tag.
         """
-        return pulumi.get(self, "last_used_at")
+        return pulumi.get(self, "message")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The Name of the agent.
+        The name of a tag.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def project(self) -> pulumi.Output[str]:
         """
-        ID or full path of the project maintained by the authenticated user.
+        The ID or URL-encoded path of the project owned by the authenticated user.
         """
         return pulumi.get(self, "project")
 
     @property
     @pulumi.getter
-    def status(self) -> pulumi.Output[str]:
+    def protected(self) -> pulumi.Output[bool]:
         """
-        The status of the token. Valid values are `active`, `revoked`.
+        Bool, true if tag has tag protection.
         """
-        return pulumi.get(self, "status")
+        return pulumi.get(self, "protected")
 
     @property
     @pulumi.getter
-    def token(self) -> pulumi.Output[str]:
+    def ref(self) -> pulumi.Output[str]:
         """
-        The secret token for the agent. The `token` is not available in imported resources.
+        Create tag using commit SHA, another tag name, or branch name. This attribute is not available for imported resources.
         """
-        return pulumi.get(self, "token")
+        return pulumi.get(self, "ref")
 
     @property
-    @pulumi.getter(name="tokenId")
-    def token_id(self) -> pulumi.Output[int]:
+    @pulumi.getter
+    def releases(self) -> pulumi.Output[Sequence['outputs.ProjectTagRelease']]:
+        """
+        The release associated with the tag.
+        """
+        return pulumi.get(self, "releases")
+
+    @property
+    @pulumi.getter
+    def target(self) -> pulumi.Output[str]:
         """
-        The ID of the token.
+        The unique id assigned to the commit by Gitlab.
         """
-        return pulumi.get(self, "token_id")
+        return pulumi.get(self, "target")
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/config/vars.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/deploy_key.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/deploy_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/deploy_key_enable.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/deploy_key_enable.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         parent_deploy_key = gitlab.DeployKey("parentDeployKey",
             project=parent_project.id,
             title="Example deploy key",
             key="ssh-ed25519 AAAA...")
         # Enable the deployment key on the second repo
         foo_deploy_key_enable = gitlab.DeployKeyEnable("fooDeployKeyEnable",
             project=foo_project.id,
-            key_id=parent_deploy_key.id)
+            key_id=parent_deploy_key.deploy_key_id)
         ```
 
         ## Import
 
         GitLab enabled deploy keys can be imported using an id made up of `{project_id}:{deploy_key_id}`, e.g. `project_id` can be whatever the [get single project api][get_single_project] takes for its `:id` value, so for example
 
         ```sh
@@ -267,15 +267,15 @@
         parent_deploy_key = gitlab.DeployKey("parentDeployKey",
             project=parent_project.id,
             title="Example deploy key",
             key="ssh-ed25519 AAAA...")
         # Enable the deployment key on the second repo
         foo_deploy_key_enable = gitlab.DeployKeyEnable("fooDeployKeyEnable",
             project=foo_project.id,
-            key_id=parent_deploy_key.id)
+            key_id=parent_deploy_key.deploy_key_id)
         ```
 
         ## Import
 
         GitLab enabled deploy keys can be imported using an id made up of `{project_id}:{deploy_key_id}`, e.g. `project_id` can be whatever the [get single project api][get_single_project] takes for its `:id` value, so for example
 
         ```sh
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/deploy_token.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/deploy_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_application.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_application.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,19 +98,19 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getApplication:getApplication', __args__, opts=opts, typ=GetApplicationResult).value
 
     return AwaitableGetApplicationResult(
-        application_id=__ret__.application_id,
-        confidential=__ret__.confidential,
-        id=__ret__.id,
-        name=__ret__.name,
-        redirect_url=__ret__.redirect_url)
+        application_id=pulumi.get(__ret__, 'application_id'),
+        confidential=pulumi.get(__ret__, 'confidential'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        redirect_url=pulumi.get(__ret__, 'redirect_url'))
 
 
 @_utilities.lift_output_func(get_application)
 def get_application_output(id: Optional[pulumi.Input[str]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetApplicationResult]:
     """
     The `Application` data source retrieves information about a gitlab application.
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_branch.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_branch.py`

 * *Files 8% similar despite different names*

```diff
@@ -190,25 +190,25 @@
     __args__ = dict()
     __args__['name'] = name
     __args__['project'] = project
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getBranch:getBranch', __args__, opts=opts, typ=GetBranchResult).value
 
     return AwaitableGetBranchResult(
-        can_push=__ret__.can_push,
-        commits=__ret__.commits,
-        default=__ret__.default,
-        developer_can_merge=__ret__.developer_can_merge,
-        developer_can_push=__ret__.developer_can_push,
-        id=__ret__.id,
-        merged=__ret__.merged,
-        name=__ret__.name,
-        project=__ret__.project,
-        protected=__ret__.protected,
-        web_url=__ret__.web_url)
+        can_push=pulumi.get(__ret__, 'can_push'),
+        commits=pulumi.get(__ret__, 'commits'),
+        default=pulumi.get(__ret__, 'default'),
+        developer_can_merge=pulumi.get(__ret__, 'developer_can_merge'),
+        developer_can_push=pulumi.get(__ret__, 'developer_can_push'),
+        id=pulumi.get(__ret__, 'id'),
+        merged=pulumi.get(__ret__, 'merged'),
+        name=pulumi.get(__ret__, 'name'),
+        project=pulumi.get(__ret__, 'project'),
+        protected=pulumi.get(__ret__, 'protected'),
+        web_url=pulumi.get(__ret__, 'web_url'))
 
 
 @_utilities.lift_output_func(get_branch)
 def get_branch_output(name: Optional[pulumi.Input[str]] = None,
                       project: Optional[pulumi.Input[str]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetBranchResult]:
     """
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_cluster_agent.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_cluster_agent.py`

 * *Files 12% similar despite different names*

```diff
@@ -131,20 +131,20 @@
     __args__ = dict()
     __args__['agentId'] = agent_id
     __args__['project'] = project
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getClusterAgent:getClusterAgent', __args__, opts=opts, typ=GetClusterAgentResult).value
 
     return AwaitableGetClusterAgentResult(
-        agent_id=__ret__.agent_id,
-        created_at=__ret__.created_at,
-        created_by_user_id=__ret__.created_by_user_id,
-        id=__ret__.id,
-        name=__ret__.name,
-        project=__ret__.project)
+        agent_id=pulumi.get(__ret__, 'agent_id'),
+        created_at=pulumi.get(__ret__, 'created_at'),
+        created_by_user_id=pulumi.get(__ret__, 'created_by_user_id'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        project=pulumi.get(__ret__, 'project'))
 
 
 @_utilities.lift_output_func(get_cluster_agent)
 def get_cluster_agent_output(agent_id: Optional[pulumi.Input[int]] = None,
                              project: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetClusterAgentResult]:
     """
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_cluster_agents.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_cluster_agents.py`

 * *Files 12% similar despite different names*

```diff
@@ -92,17 +92,17 @@
     """
     __args__ = dict()
     __args__['project'] = project
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getClusterAgents:getClusterAgents', __args__, opts=opts, typ=GetClusterAgentsResult).value
 
     return AwaitableGetClusterAgentsResult(
-        cluster_agents=__ret__.cluster_agents,
-        id=__ret__.id,
-        project=__ret__.project)
+        cluster_agents=pulumi.get(__ret__, 'cluster_agents'),
+        id=pulumi.get(__ret__, 'id'),
+        project=pulumi.get(__ret__, 'project'))
 
 
 @_utilities.lift_output_func(get_cluster_agents)
 def get_cluster_agents_output(project: Optional[pulumi.Input[str]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetClusterAgentsResult]:
     """
     The `get_cluster_agents` data source allows details of GitLab Agents for Kubernetes in a project.
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_current_user.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_current_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -155,16 +155,16 @@
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getCurrentUser:getCurrentUser', __args__, opts=opts, typ=GetCurrentUserResult).value
 
     return AwaitableGetCurrentUserResult(
-        bot=__ret__.bot,
-        global_id=__ret__.global_id,
-        global_namespace_id=__ret__.global_namespace_id,
-        group_count=__ret__.group_count,
-        id=__ret__.id,
-        name=__ret__.name,
-        namespace_id=__ret__.namespace_id,
-        public_email=__ret__.public_email,
-        username=__ret__.username)
+        bot=pulumi.get(__ret__, 'bot'),
+        global_id=pulumi.get(__ret__, 'global_id'),
+        global_namespace_id=pulumi.get(__ret__, 'global_namespace_id'),
+        group_count=pulumi.get(__ret__, 'group_count'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        namespace_id=pulumi.get(__ret__, 'namespace_id'),
+        public_email=pulumi.get(__ret__, 'public_email'),
+        username=pulumi.get(__ret__, 'username'))
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_group.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -272,32 +272,32 @@
     __args__ = dict()
     __args__['fullPath'] = full_path
     __args__['groupId'] = group_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getGroup:getGroup', __args__, opts=opts, typ=GetGroupResult).value
 
     return AwaitableGetGroupResult(
-        default_branch_protection=__ret__.default_branch_protection,
-        description=__ret__.description,
-        extra_shared_runners_minutes_limit=__ret__.extra_shared_runners_minutes_limit,
-        full_name=__ret__.full_name,
-        full_path=__ret__.full_path,
-        group_id=__ret__.group_id,
-        id=__ret__.id,
-        lfs_enabled=__ret__.lfs_enabled,
-        membership_lock=__ret__.membership_lock,
-        name=__ret__.name,
-        parent_id=__ret__.parent_id,
-        path=__ret__.path,
-        prevent_forking_outside_group=__ret__.prevent_forking_outside_group,
-        request_access_enabled=__ret__.request_access_enabled,
-        runners_token=__ret__.runners_token,
-        shared_runners_minutes_limit=__ret__.shared_runners_minutes_limit,
-        visibility_level=__ret__.visibility_level,
-        web_url=__ret__.web_url)
+        default_branch_protection=pulumi.get(__ret__, 'default_branch_protection'),
+        description=pulumi.get(__ret__, 'description'),
+        extra_shared_runners_minutes_limit=pulumi.get(__ret__, 'extra_shared_runners_minutes_limit'),
+        full_name=pulumi.get(__ret__, 'full_name'),
+        full_path=pulumi.get(__ret__, 'full_path'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'),
+        lfs_enabled=pulumi.get(__ret__, 'lfs_enabled'),
+        membership_lock=pulumi.get(__ret__, 'membership_lock'),
+        name=pulumi.get(__ret__, 'name'),
+        parent_id=pulumi.get(__ret__, 'parent_id'),
+        path=pulumi.get(__ret__, 'path'),
+        prevent_forking_outside_group=pulumi.get(__ret__, 'prevent_forking_outside_group'),
+        request_access_enabled=pulumi.get(__ret__, 'request_access_enabled'),
+        runners_token=pulumi.get(__ret__, 'runners_token'),
+        shared_runners_minutes_limit=pulumi.get(__ret__, 'shared_runners_minutes_limit'),
+        visibility_level=pulumi.get(__ret__, 'visibility_level'),
+        web_url=pulumi.get(__ret__, 'web_url'))
 
 
 @_utilities.lift_output_func(get_group)
 def get_group_output(full_path: Optional[pulumi.Input[Optional[str]]] = None,
                      group_id: Optional[pulumi.Input[Optional[int]]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGroupResult]:
     """
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_group_hook.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_group_hook.py`

 * *Files 8% similar despite different names*

```diff
@@ -299,35 +299,35 @@
     __args__ = dict()
     __args__['group'] = group
     __args__['hookId'] = hook_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getGroupHook:getGroupHook', __args__, opts=opts, typ=GetGroupHookResult).value
 
     return AwaitableGetGroupHookResult(
-        confidential_issues_events=__ret__.confidential_issues_events,
-        confidential_note_events=__ret__.confidential_note_events,
-        deployment_events=__ret__.deployment_events,
-        enable_ssl_verification=__ret__.enable_ssl_verification,
-        group=__ret__.group,
-        group_id=__ret__.group_id,
-        hook_id=__ret__.hook_id,
-        id=__ret__.id,
-        issues_events=__ret__.issues_events,
-        job_events=__ret__.job_events,
-        merge_requests_events=__ret__.merge_requests_events,
-        note_events=__ret__.note_events,
-        pipeline_events=__ret__.pipeline_events,
-        push_events=__ret__.push_events,
-        push_events_branch_filter=__ret__.push_events_branch_filter,
-        releases_events=__ret__.releases_events,
-        subgroup_events=__ret__.subgroup_events,
-        tag_push_events=__ret__.tag_push_events,
-        token=__ret__.token,
-        url=__ret__.url,
-        wiki_page_events=__ret__.wiki_page_events)
+        confidential_issues_events=pulumi.get(__ret__, 'confidential_issues_events'),
+        confidential_note_events=pulumi.get(__ret__, 'confidential_note_events'),
+        deployment_events=pulumi.get(__ret__, 'deployment_events'),
+        enable_ssl_verification=pulumi.get(__ret__, 'enable_ssl_verification'),
+        group=pulumi.get(__ret__, 'group'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        hook_id=pulumi.get(__ret__, 'hook_id'),
+        id=pulumi.get(__ret__, 'id'),
+        issues_events=pulumi.get(__ret__, 'issues_events'),
+        job_events=pulumi.get(__ret__, 'job_events'),
+        merge_requests_events=pulumi.get(__ret__, 'merge_requests_events'),
+        note_events=pulumi.get(__ret__, 'note_events'),
+        pipeline_events=pulumi.get(__ret__, 'pipeline_events'),
+        push_events=pulumi.get(__ret__, 'push_events'),
+        push_events_branch_filter=pulumi.get(__ret__, 'push_events_branch_filter'),
+        releases_events=pulumi.get(__ret__, 'releases_events'),
+        subgroup_events=pulumi.get(__ret__, 'subgroup_events'),
+        tag_push_events=pulumi.get(__ret__, 'tag_push_events'),
+        token=pulumi.get(__ret__, 'token'),
+        url=pulumi.get(__ret__, 'url'),
+        wiki_page_events=pulumi.get(__ret__, 'wiki_page_events'))
 
 
 @_utilities.lift_output_func(get_group_hook)
 def get_group_hook_output(group: Optional[pulumi.Input[str]] = None,
                           hook_id: Optional[pulumi.Input[int]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGroupHookResult]:
     """
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_group_hooks.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_group_hooks.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,17 +81,17 @@
     """
     __args__ = dict()
     __args__['group'] = group
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getGroupHooks:getGroupHooks', __args__, opts=opts, typ=GetGroupHooksResult).value
 
     return AwaitableGetGroupHooksResult(
-        group=__ret__.group,
-        hooks=__ret__.hooks,
-        id=__ret__.id)
+        group=pulumi.get(__ret__, 'group'),
+        hooks=pulumi.get(__ret__, 'hooks'),
+        id=pulumi.get(__ret__, 'id'))
 
 
 @_utilities.lift_output_func(get_group_hooks)
 def get_group_hooks_output(group: Optional[pulumi.Input[str]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGroupHooksResult]:
     """
     The `get_group_hooks` data source allows to retrieve details about hooks in a group.
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_group_membership.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_group_membership.py`

 * *Files 5% similar despite different names*

```diff
@@ -135,20 +135,20 @@
     __args__['fullPath'] = full_path
     __args__['groupId'] = group_id
     __args__['inherited'] = inherited
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getGroupMembership:getGroupMembership', __args__, opts=opts, typ=GetGroupMembershipResult).value
 
     return AwaitableGetGroupMembershipResult(
-        access_level=__ret__.access_level,
-        full_path=__ret__.full_path,
-        group_id=__ret__.group_id,
-        id=__ret__.id,
-        inherited=__ret__.inherited,
-        members=__ret__.members)
+        access_level=pulumi.get(__ret__, 'access_level'),
+        full_path=pulumi.get(__ret__, 'full_path'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'),
+        inherited=pulumi.get(__ret__, 'inherited'),
+        members=pulumi.get(__ret__, 'members'))
 
 
 @_utilities.lift_output_func(get_group_membership)
 def get_group_membership_output(access_level: Optional[pulumi.Input[Optional[str]]] = None,
                                 full_path: Optional[pulumi.Input[Optional[str]]] = None,
                                 group_id: Optional[pulumi.Input[Optional[int]]] = None,
                                 inherited: Optional[pulumi.Input[Optional[bool]]] = None,
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_group_subgroups.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_group_subgroups.py`

 * *Files 7% similar despite different names*

```diff
@@ -226,26 +226,26 @@
     __args__['sort'] = sort
     __args__['statistics'] = statistics
     __args__['withCustomAttributes'] = with_custom_attributes
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getGroupSubgroups:getGroupSubgroups', __args__, opts=opts, typ=GetGroupSubgroupsResult).value
 
     return AwaitableGetGroupSubgroupsResult(
-        all_available=__ret__.all_available,
-        group_id=__ret__.group_id,
-        id=__ret__.id,
-        min_access_level=__ret__.min_access_level,
-        order_by=__ret__.order_by,
-        owned=__ret__.owned,
-        search=__ret__.search,
-        skip_groups=__ret__.skip_groups,
-        sort=__ret__.sort,
-        statistics=__ret__.statistics,
-        subgroups=__ret__.subgroups,
-        with_custom_attributes=__ret__.with_custom_attributes)
+        all_available=pulumi.get(__ret__, 'all_available'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'),
+        min_access_level=pulumi.get(__ret__, 'min_access_level'),
+        order_by=pulumi.get(__ret__, 'order_by'),
+        owned=pulumi.get(__ret__, 'owned'),
+        search=pulumi.get(__ret__, 'search'),
+        skip_groups=pulumi.get(__ret__, 'skip_groups'),
+        sort=pulumi.get(__ret__, 'sort'),
+        statistics=pulumi.get(__ret__, 'statistics'),
+        subgroups=pulumi.get(__ret__, 'subgroups'),
+        with_custom_attributes=pulumi.get(__ret__, 'with_custom_attributes'))
 
 
 @_utilities.lift_output_func(get_group_subgroups)
 def get_group_subgroups_output(all_available: Optional[pulumi.Input[Optional[bool]]] = None,
                                group_id: Optional[pulumi.Input[int]] = None,
                                min_access_level: Optional[pulumi.Input[Optional[str]]] = None,
                                order_by: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_group_variable.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_group_variable.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,23 +171,23 @@
     __args__['environmentScope'] = environment_scope
     __args__['group'] = group
     __args__['key'] = key
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getGroupVariable:getGroupVariable', __args__, opts=opts, typ=GetGroupVariableResult).value
 
     return AwaitableGetGroupVariableResult(
-        environment_scope=__ret__.environment_scope,
-        group=__ret__.group,
-        id=__ret__.id,
-        key=__ret__.key,
-        masked=__ret__.masked,
-        protected=__ret__.protected,
-        raw=__ret__.raw,
-        value=__ret__.value,
-        variable_type=__ret__.variable_type)
+        environment_scope=pulumi.get(__ret__, 'environment_scope'),
+        group=pulumi.get(__ret__, 'group'),
+        id=pulumi.get(__ret__, 'id'),
+        key=pulumi.get(__ret__, 'key'),
+        masked=pulumi.get(__ret__, 'masked'),
+        protected=pulumi.get(__ret__, 'protected'),
+        raw=pulumi.get(__ret__, 'raw'),
+        value=pulumi.get(__ret__, 'value'),
+        variable_type=pulumi.get(__ret__, 'variable_type'))
 
 
 @_utilities.lift_output_func(get_group_variable)
 def get_group_variable_output(environment_scope: Optional[pulumi.Input[Optional[str]]] = None,
                               group: Optional[pulumi.Input[str]] = None,
                               key: Optional[pulumi.Input[str]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGroupVariableResult]:
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_group_variables.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_group_variables.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,18 +107,18 @@
     __args__ = dict()
     __args__['environmentScope'] = environment_scope
     __args__['group'] = group
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getGroupVariables:getGroupVariables', __args__, opts=opts, typ=GetGroupVariablesResult).value
 
     return AwaitableGetGroupVariablesResult(
-        environment_scope=__ret__.environment_scope,
-        group=__ret__.group,
-        id=__ret__.id,
-        variables=__ret__.variables)
+        environment_scope=pulumi.get(__ret__, 'environment_scope'),
+        group=pulumi.get(__ret__, 'group'),
+        id=pulumi.get(__ret__, 'id'),
+        variables=pulumi.get(__ret__, 'variables'))
 
 
 @_utilities.lift_output_func(get_group_variables)
 def get_group_variables_output(environment_scope: Optional[pulumi.Input[Optional[str]]] = None,
                                group: Optional[pulumi.Input[str]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGroupVariablesResult]:
     """
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_groups.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_groups.py`

 * *Files 5% similar despite different names*

```diff
@@ -126,19 +126,19 @@
     __args__['orderBy'] = order_by
     __args__['search'] = search
     __args__['sort'] = sort
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getGroups:getGroups', __args__, opts=opts, typ=GetGroupsResult).value
 
     return AwaitableGetGroupsResult(
-        groups=__ret__.groups,
-        id=__ret__.id,
-        order_by=__ret__.order_by,
-        search=__ret__.search,
-        sort=__ret__.sort)
+        groups=pulumi.get(__ret__, 'groups'),
+        id=pulumi.get(__ret__, 'id'),
+        order_by=pulumi.get(__ret__, 'order_by'),
+        search=pulumi.get(__ret__, 'search'),
+        sort=pulumi.get(__ret__, 'sort'))
 
 
 @_utilities.lift_output_func(get_groups)
 def get_groups_output(order_by: Optional[pulumi.Input[Optional[str]]] = None,
                       search: Optional[pulumi.Input[Optional[str]]] = None,
                       sort: Optional[pulumi.Input[Optional[str]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGroupsResult]:
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_instance_deploy_keys.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_instance_deploy_keys.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,17 +92,17 @@
     """
     __args__ = dict()
     __args__['public'] = public
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getInstanceDeployKeys:getInstanceDeployKeys', __args__, opts=opts, typ=GetInstanceDeployKeysResult).value
 
     return AwaitableGetInstanceDeployKeysResult(
-        deploy_keys=__ret__.deploy_keys,
-        id=__ret__.id,
-        public=__ret__.public)
+        deploy_keys=pulumi.get(__ret__, 'deploy_keys'),
+        id=pulumi.get(__ret__, 'id'),
+        public=pulumi.get(__ret__, 'public'))
 
 
 @_utilities.lift_output_func(get_instance_deploy_keys)
 def get_instance_deploy_keys_output(public: Optional[pulumi.Input[Optional[bool]]] = None,
                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstanceDeployKeysResult]:
     """
     The `get_instance_deploy_keys` data source allows to retrieve a list of deploy keys for a GitLab instance.
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_instance_variable.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_instance_variable.py`

 * *Files 8% similar despite different names*

```diff
@@ -137,21 +137,21 @@
     """
     __args__ = dict()
     __args__['key'] = key
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getInstanceVariable:getInstanceVariable', __args__, opts=opts, typ=GetInstanceVariableResult).value
 
     return AwaitableGetInstanceVariableResult(
-        id=__ret__.id,
-        key=__ret__.key,
-        masked=__ret__.masked,
-        protected=__ret__.protected,
-        raw=__ret__.raw,
-        value=__ret__.value,
-        variable_type=__ret__.variable_type)
+        id=pulumi.get(__ret__, 'id'),
+        key=pulumi.get(__ret__, 'key'),
+        masked=pulumi.get(__ret__, 'masked'),
+        protected=pulumi.get(__ret__, 'protected'),
+        raw=pulumi.get(__ret__, 'raw'),
+        value=pulumi.get(__ret__, 'value'),
+        variable_type=pulumi.get(__ret__, 'variable_type'))
 
 
 @_utilities.lift_output_func(get_instance_variable)
 def get_instance_variable_output(key: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetInstanceVariableResult]:
     """
     The `InstanceVariable` data source allows to retrieve details about an instance-level CI/CD variable.
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_instance_variables.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_instance_variables.py`

 * *Files 5% similar despite different names*

```diff
@@ -72,9 +72,9 @@
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getInstanceVariables:getInstanceVariables', __args__, opts=opts, typ=GetInstanceVariablesResult).value
 
     return AwaitableGetInstanceVariablesResult(
-        id=__ret__.id,
-        variables=__ret__.variables)
+        id=pulumi.get(__ret__, 'id'),
+        variables=pulumi.get(__ret__, 'variables'))
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_metadata.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_metadata.py`

 * *Files 16% similar despite different names*

```diff
@@ -108,12 +108,12 @@
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getMetadata:getMetadata', __args__, opts=opts, typ=GetMetadataResult).value
 
     return AwaitableGetMetadataResult(
-        enterprise=__ret__.enterprise,
-        id=__ret__.id,
-        kas=__ret__.kas,
-        revision=__ret__.revision,
-        version=__ret__.version)
+        enterprise=pulumi.get(__ret__, 'enterprise'),
+        id=pulumi.get(__ret__, 'id'),
+        kas=pulumi.get(__ret__, 'kas'),
+        revision=pulumi.get(__ret__, 'revision'),
+        version=pulumi.get(__ret__, 'version'))
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project.py`

 * *Files 16% similar despite different names*

```diff
@@ -819,77 +819,77 @@
     __args__['id'] = id
     __args__['pathWithNamespace'] = path_with_namespace
     __args__['publicBuilds'] = public_builds
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getProject:getProject', __args__, opts=opts, typ=GetProjectResult).value
 
     return AwaitableGetProjectResult(
-        analytics_access_level=__ret__.analytics_access_level,
-        archived=__ret__.archived,
-        auto_cancel_pending_pipelines=__ret__.auto_cancel_pending_pipelines,
-        auto_devops_deploy_strategy=__ret__.auto_devops_deploy_strategy,
-        auto_devops_enabled=__ret__.auto_devops_enabled,
-        autoclose_referenced_issues=__ret__.autoclose_referenced_issues,
-        build_git_strategy=__ret__.build_git_strategy,
-        build_timeout=__ret__.build_timeout,
-        builds_access_level=__ret__.builds_access_level,
-        ci_config_path=__ret__.ci_config_path,
-        ci_default_git_depth=__ret__.ci_default_git_depth,
-        ci_separated_caches=__ret__.ci_separated_caches,
-        container_expiration_policies=__ret__.container_expiration_policies,
-        container_registry_access_level=__ret__.container_registry_access_level,
-        default_branch=__ret__.default_branch,
-        description=__ret__.description,
-        emails_disabled=__ret__.emails_disabled,
-        environments_access_level=__ret__.environments_access_level,
-        external_authorization_classification_label=__ret__.external_authorization_classification_label,
-        feature_flags_access_level=__ret__.feature_flags_access_level,
-        forking_access_level=__ret__.forking_access_level,
-        http_url_to_repo=__ret__.http_url_to_repo,
-        id=__ret__.id,
-        import_url=__ret__.import_url,
-        infrastructure_access_level=__ret__.infrastructure_access_level,
-        issues_access_level=__ret__.issues_access_level,
-        issues_enabled=__ret__.issues_enabled,
-        keep_latest_artifact=__ret__.keep_latest_artifact,
-        lfs_enabled=__ret__.lfs_enabled,
-        merge_commit_template=__ret__.merge_commit_template,
-        merge_pipelines_enabled=__ret__.merge_pipelines_enabled,
-        merge_requests_access_level=__ret__.merge_requests_access_level,
-        merge_requests_enabled=__ret__.merge_requests_enabled,
-        merge_trains_enabled=__ret__.merge_trains_enabled,
-        monitor_access_level=__ret__.monitor_access_level,
-        name=__ret__.name,
-        namespace_id=__ret__.namespace_id,
-        path=__ret__.path,
-        path_with_namespace=__ret__.path_with_namespace,
-        pipelines_enabled=__ret__.pipelines_enabled,
-        printing_merge_request_link_enabled=__ret__.printing_merge_request_link_enabled,
-        public_builds=__ret__.public_builds,
-        push_rules=__ret__.push_rules,
-        releases_access_level=__ret__.releases_access_level,
-        remove_source_branch_after_merge=__ret__.remove_source_branch_after_merge,
-        repository_access_level=__ret__.repository_access_level,
-        repository_storage=__ret__.repository_storage,
-        request_access_enabled=__ret__.request_access_enabled,
-        requirements_access_level=__ret__.requirements_access_level,
-        resolve_outdated_diff_discussions=__ret__.resolve_outdated_diff_discussions,
-        restrict_user_defined_variables=__ret__.restrict_user_defined_variables,
-        runners_token=__ret__.runners_token,
-        security_and_compliance_access_level=__ret__.security_and_compliance_access_level,
-        snippets_access_level=__ret__.snippets_access_level,
-        snippets_enabled=__ret__.snippets_enabled,
-        squash_commit_template=__ret__.squash_commit_template,
-        ssh_url_to_repo=__ret__.ssh_url_to_repo,
-        suggestion_commit_message=__ret__.suggestion_commit_message,
-        topics=__ret__.topics,
-        visibility_level=__ret__.visibility_level,
-        web_url=__ret__.web_url,
-        wiki_access_level=__ret__.wiki_access_level,
-        wiki_enabled=__ret__.wiki_enabled)
+        analytics_access_level=pulumi.get(__ret__, 'analytics_access_level'),
+        archived=pulumi.get(__ret__, 'archived'),
+        auto_cancel_pending_pipelines=pulumi.get(__ret__, 'auto_cancel_pending_pipelines'),
+        auto_devops_deploy_strategy=pulumi.get(__ret__, 'auto_devops_deploy_strategy'),
+        auto_devops_enabled=pulumi.get(__ret__, 'auto_devops_enabled'),
+        autoclose_referenced_issues=pulumi.get(__ret__, 'autoclose_referenced_issues'),
+        build_git_strategy=pulumi.get(__ret__, 'build_git_strategy'),
+        build_timeout=pulumi.get(__ret__, 'build_timeout'),
+        builds_access_level=pulumi.get(__ret__, 'builds_access_level'),
+        ci_config_path=pulumi.get(__ret__, 'ci_config_path'),
+        ci_default_git_depth=pulumi.get(__ret__, 'ci_default_git_depth'),
+        ci_separated_caches=pulumi.get(__ret__, 'ci_separated_caches'),
+        container_expiration_policies=pulumi.get(__ret__, 'container_expiration_policies'),
+        container_registry_access_level=pulumi.get(__ret__, 'container_registry_access_level'),
+        default_branch=pulumi.get(__ret__, 'default_branch'),
+        description=pulumi.get(__ret__, 'description'),
+        emails_disabled=pulumi.get(__ret__, 'emails_disabled'),
+        environments_access_level=pulumi.get(__ret__, 'environments_access_level'),
+        external_authorization_classification_label=pulumi.get(__ret__, 'external_authorization_classification_label'),
+        feature_flags_access_level=pulumi.get(__ret__, 'feature_flags_access_level'),
+        forking_access_level=pulumi.get(__ret__, 'forking_access_level'),
+        http_url_to_repo=pulumi.get(__ret__, 'http_url_to_repo'),
+        id=pulumi.get(__ret__, 'id'),
+        import_url=pulumi.get(__ret__, 'import_url'),
+        infrastructure_access_level=pulumi.get(__ret__, 'infrastructure_access_level'),
+        issues_access_level=pulumi.get(__ret__, 'issues_access_level'),
+        issues_enabled=pulumi.get(__ret__, 'issues_enabled'),
+        keep_latest_artifact=pulumi.get(__ret__, 'keep_latest_artifact'),
+        lfs_enabled=pulumi.get(__ret__, 'lfs_enabled'),
+        merge_commit_template=pulumi.get(__ret__, 'merge_commit_template'),
+        merge_pipelines_enabled=pulumi.get(__ret__, 'merge_pipelines_enabled'),
+        merge_requests_access_level=pulumi.get(__ret__, 'merge_requests_access_level'),
+        merge_requests_enabled=pulumi.get(__ret__, 'merge_requests_enabled'),
+        merge_trains_enabled=pulumi.get(__ret__, 'merge_trains_enabled'),
+        monitor_access_level=pulumi.get(__ret__, 'monitor_access_level'),
+        name=pulumi.get(__ret__, 'name'),
+        namespace_id=pulumi.get(__ret__, 'namespace_id'),
+        path=pulumi.get(__ret__, 'path'),
+        path_with_namespace=pulumi.get(__ret__, 'path_with_namespace'),
+        pipelines_enabled=pulumi.get(__ret__, 'pipelines_enabled'),
+        printing_merge_request_link_enabled=pulumi.get(__ret__, 'printing_merge_request_link_enabled'),
+        public_builds=pulumi.get(__ret__, 'public_builds'),
+        push_rules=pulumi.get(__ret__, 'push_rules'),
+        releases_access_level=pulumi.get(__ret__, 'releases_access_level'),
+        remove_source_branch_after_merge=pulumi.get(__ret__, 'remove_source_branch_after_merge'),
+        repository_access_level=pulumi.get(__ret__, 'repository_access_level'),
+        repository_storage=pulumi.get(__ret__, 'repository_storage'),
+        request_access_enabled=pulumi.get(__ret__, 'request_access_enabled'),
+        requirements_access_level=pulumi.get(__ret__, 'requirements_access_level'),
+        resolve_outdated_diff_discussions=pulumi.get(__ret__, 'resolve_outdated_diff_discussions'),
+        restrict_user_defined_variables=pulumi.get(__ret__, 'restrict_user_defined_variables'),
+        runners_token=pulumi.get(__ret__, 'runners_token'),
+        security_and_compliance_access_level=pulumi.get(__ret__, 'security_and_compliance_access_level'),
+        snippets_access_level=pulumi.get(__ret__, 'snippets_access_level'),
+        snippets_enabled=pulumi.get(__ret__, 'snippets_enabled'),
+        squash_commit_template=pulumi.get(__ret__, 'squash_commit_template'),
+        ssh_url_to_repo=pulumi.get(__ret__, 'ssh_url_to_repo'),
+        suggestion_commit_message=pulumi.get(__ret__, 'suggestion_commit_message'),
+        topics=pulumi.get(__ret__, 'topics'),
+        visibility_level=pulumi.get(__ret__, 'visibility_level'),
+        web_url=pulumi.get(__ret__, 'web_url'),
+        wiki_access_level=pulumi.get(__ret__, 'wiki_access_level'),
+        wiki_enabled=pulumi.get(__ret__, 'wiki_enabled'))
 
 
 @_utilities.lift_output_func(get_project)
 def get_project_output(ci_default_git_depth: Optional[pulumi.Input[Optional[int]]] = None,
                        id: Optional[pulumi.Input[Optional[str]]] = None,
                        path_with_namespace: Optional[pulumi.Input[Optional[str]]] = None,
                        public_builds: Optional[pulumi.Input[Optional[bool]]] = None,
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_branches.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_branches.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,17 +90,17 @@
     """
     __args__ = dict()
     __args__['project'] = project
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getProjectBranches:getProjectBranches', __args__, opts=opts, typ=GetProjectBranchesResult).value
 
     return AwaitableGetProjectBranchesResult(
-        branches=__ret__.branches,
-        id=__ret__.id,
-        project=__ret__.project)
+        branches=pulumi.get(__ret__, 'branches'),
+        id=pulumi.get(__ret__, 'id'),
+        project=pulumi.get(__ret__, 'project'))
 
 
 @_utilities.lift_output_func(get_project_branches)
 def get_project_branches_output(project: Optional[pulumi.Input[str]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectBranchesResult]:
     """
     The `get_project_branches` data source allows details of the branches of a given project to be retrieved.
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_hook.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_hook.py`

 * *Files 6% similar despite different names*

```diff
@@ -298,34 +298,34 @@
     __args__ = dict()
     __args__['hookId'] = hook_id
     __args__['project'] = project
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getProjectHook:getProjectHook', __args__, opts=opts, typ=GetProjectHookResult).value
 
     return AwaitableGetProjectHookResult(
-        confidential_issues_events=__ret__.confidential_issues_events,
-        confidential_note_events=__ret__.confidential_note_events,
-        deployment_events=__ret__.deployment_events,
-        enable_ssl_verification=__ret__.enable_ssl_verification,
-        hook_id=__ret__.hook_id,
-        id=__ret__.id,
-        issues_events=__ret__.issues_events,
-        job_events=__ret__.job_events,
-        merge_requests_events=__ret__.merge_requests_events,
-        note_events=__ret__.note_events,
-        pipeline_events=__ret__.pipeline_events,
-        project=__ret__.project,
-        project_id=__ret__.project_id,
-        push_events=__ret__.push_events,
-        push_events_branch_filter=__ret__.push_events_branch_filter,
-        releases_events=__ret__.releases_events,
-        tag_push_events=__ret__.tag_push_events,
-        token=__ret__.token,
-        url=__ret__.url,
-        wiki_page_events=__ret__.wiki_page_events)
+        confidential_issues_events=pulumi.get(__ret__, 'confidential_issues_events'),
+        confidential_note_events=pulumi.get(__ret__, 'confidential_note_events'),
+        deployment_events=pulumi.get(__ret__, 'deployment_events'),
+        enable_ssl_verification=pulumi.get(__ret__, 'enable_ssl_verification'),
+        hook_id=pulumi.get(__ret__, 'hook_id'),
+        id=pulumi.get(__ret__, 'id'),
+        issues_events=pulumi.get(__ret__, 'issues_events'),
+        job_events=pulumi.get(__ret__, 'job_events'),
+        merge_requests_events=pulumi.get(__ret__, 'merge_requests_events'),
+        note_events=pulumi.get(__ret__, 'note_events'),
+        pipeline_events=pulumi.get(__ret__, 'pipeline_events'),
+        project=pulumi.get(__ret__, 'project'),
+        project_id=pulumi.get(__ret__, 'project_id'),
+        push_events=pulumi.get(__ret__, 'push_events'),
+        push_events_branch_filter=pulumi.get(__ret__, 'push_events_branch_filter'),
+        releases_events=pulumi.get(__ret__, 'releases_events'),
+        tag_push_events=pulumi.get(__ret__, 'tag_push_events'),
+        token=pulumi.get(__ret__, 'token'),
+        url=pulumi.get(__ret__, 'url'),
+        wiki_page_events=pulumi.get(__ret__, 'wiki_page_events'))
 
 
 @_utilities.lift_output_func(get_project_hook)
 def get_project_hook_output(hook_id: Optional[pulumi.Input[int]] = None,
                             project: Optional[pulumi.Input[str]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectHookResult]:
     """
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_hooks.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,17 +91,17 @@
     """
     __args__ = dict()
     __args__['project'] = project
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getProjectHooks:getProjectHooks', __args__, opts=opts, typ=GetProjectHooksResult).value
 
     return AwaitableGetProjectHooksResult(
-        hooks=__ret__.hooks,
-        id=__ret__.id,
-        project=__ret__.project)
+        hooks=pulumi.get(__ret__, 'hooks'),
+        id=pulumi.get(__ret__, 'id'),
+        project=pulumi.get(__ret__, 'project'))
 
 
 @_utilities.lift_output_func(get_project_hooks)
 def get_project_hooks_output(project: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectHooksResult]:
     """
     The `get_project_hooks` data source allows to retrieve details about hooks in a project.
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_issue.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_issue.py`

 * *Files 7% similar despite different names*

```diff
@@ -540,54 +540,54 @@
     __args__ = dict()
     __args__['iid'] = iid
     __args__['project'] = project
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getProjectIssue:getProjectIssue', __args__, opts=opts, typ=GetProjectIssueResult).value
 
     return AwaitableGetProjectIssueResult(
-        assignee_ids=__ret__.assignee_ids,
-        author_id=__ret__.author_id,
-        closed_at=__ret__.closed_at,
-        closed_by_user_id=__ret__.closed_by_user_id,
-        confidential=__ret__.confidential,
-        created_at=__ret__.created_at,
-        description=__ret__.description,
-        discussion_locked=__ret__.discussion_locked,
-        discussion_to_resolve=__ret__.discussion_to_resolve,
-        downvotes=__ret__.downvotes,
-        due_date=__ret__.due_date,
-        epic_id=__ret__.epic_id,
-        epic_issue_id=__ret__.epic_issue_id,
-        external_id=__ret__.external_id,
-        human_time_estimate=__ret__.human_time_estimate,
-        human_total_time_spent=__ret__.human_total_time_spent,
-        id=__ret__.id,
-        iid=__ret__.iid,
-        issue_id=__ret__.issue_id,
-        issue_link_id=__ret__.issue_link_id,
-        issue_type=__ret__.issue_type,
-        labels=__ret__.labels,
-        links=__ret__.links,
-        merge_request_to_resolve_discussions_of=__ret__.merge_request_to_resolve_discussions_of,
-        merge_requests_count=__ret__.merge_requests_count,
-        milestone_id=__ret__.milestone_id,
-        moved_to_id=__ret__.moved_to_id,
-        project=__ret__.project,
-        references=__ret__.references,
-        state=__ret__.state,
-        subscribed=__ret__.subscribed,
-        task_completion_statuses=__ret__.task_completion_statuses,
-        time_estimate=__ret__.time_estimate,
-        title=__ret__.title,
-        total_time_spent=__ret__.total_time_spent,
-        updated_at=__ret__.updated_at,
-        upvotes=__ret__.upvotes,
-        user_notes_count=__ret__.user_notes_count,
-        web_url=__ret__.web_url,
-        weight=__ret__.weight)
+        assignee_ids=pulumi.get(__ret__, 'assignee_ids'),
+        author_id=pulumi.get(__ret__, 'author_id'),
+        closed_at=pulumi.get(__ret__, 'closed_at'),
+        closed_by_user_id=pulumi.get(__ret__, 'closed_by_user_id'),
+        confidential=pulumi.get(__ret__, 'confidential'),
+        created_at=pulumi.get(__ret__, 'created_at'),
+        description=pulumi.get(__ret__, 'description'),
+        discussion_locked=pulumi.get(__ret__, 'discussion_locked'),
+        discussion_to_resolve=pulumi.get(__ret__, 'discussion_to_resolve'),
+        downvotes=pulumi.get(__ret__, 'downvotes'),
+        due_date=pulumi.get(__ret__, 'due_date'),
+        epic_id=pulumi.get(__ret__, 'epic_id'),
+        epic_issue_id=pulumi.get(__ret__, 'epic_issue_id'),
+        external_id=pulumi.get(__ret__, 'external_id'),
+        human_time_estimate=pulumi.get(__ret__, 'human_time_estimate'),
+        human_total_time_spent=pulumi.get(__ret__, 'human_total_time_spent'),
+        id=pulumi.get(__ret__, 'id'),
+        iid=pulumi.get(__ret__, 'iid'),
+        issue_id=pulumi.get(__ret__, 'issue_id'),
+        issue_link_id=pulumi.get(__ret__, 'issue_link_id'),
+        issue_type=pulumi.get(__ret__, 'issue_type'),
+        labels=pulumi.get(__ret__, 'labels'),
+        links=pulumi.get(__ret__, 'links'),
+        merge_request_to_resolve_discussions_of=pulumi.get(__ret__, 'merge_request_to_resolve_discussions_of'),
+        merge_requests_count=pulumi.get(__ret__, 'merge_requests_count'),
+        milestone_id=pulumi.get(__ret__, 'milestone_id'),
+        moved_to_id=pulumi.get(__ret__, 'moved_to_id'),
+        project=pulumi.get(__ret__, 'project'),
+        references=pulumi.get(__ret__, 'references'),
+        state=pulumi.get(__ret__, 'state'),
+        subscribed=pulumi.get(__ret__, 'subscribed'),
+        task_completion_statuses=pulumi.get(__ret__, 'task_completion_statuses'),
+        time_estimate=pulumi.get(__ret__, 'time_estimate'),
+        title=pulumi.get(__ret__, 'title'),
+        total_time_spent=pulumi.get(__ret__, 'total_time_spent'),
+        updated_at=pulumi.get(__ret__, 'updated_at'),
+        upvotes=pulumi.get(__ret__, 'upvotes'),
+        user_notes_count=pulumi.get(__ret__, 'user_notes_count'),
+        web_url=pulumi.get(__ret__, 'web_url'),
+        weight=pulumi.get(__ret__, 'weight'))
 
 
 @_utilities.lift_output_func(get_project_issue)
 def get_project_issue_output(iid: Optional[pulumi.Input[int]] = None,
                              project: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectIssueResult]:
     """
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_issues.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_issues.py`

 * *Files 4% similar despite different names*

```diff
@@ -467,42 +467,42 @@
     __args__['updatedBefore'] = updated_before
     __args__['weight'] = weight
     __args__['withLabelsDetails'] = with_labels_details
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getProjectIssues:getProjectIssues', __args__, opts=opts, typ=GetProjectIssuesResult).value
 
     return AwaitableGetProjectIssuesResult(
-        assignee_id=__ret__.assignee_id,
-        assignee_username=__ret__.assignee_username,
-        author_id=__ret__.author_id,
-        confidential=__ret__.confidential,
-        created_after=__ret__.created_after,
-        created_before=__ret__.created_before,
-        due_date=__ret__.due_date,
-        id=__ret__.id,
-        iids=__ret__.iids,
-        issue_type=__ret__.issue_type,
-        issues=__ret__.issues,
-        labels=__ret__.labels,
-        milestone=__ret__.milestone,
-        my_reaction_emoji=__ret__.my_reaction_emoji,
-        not_assignee_ids=__ret__.not_assignee_ids,
-        not_author_ids=__ret__.not_author_ids,
-        not_labels=__ret__.not_labels,
-        not_milestone=__ret__.not_milestone,
-        not_my_reaction_emojis=__ret__.not_my_reaction_emojis,
-        order_by=__ret__.order_by,
-        project=__ret__.project,
-        scope=__ret__.scope,
-        search=__ret__.search,
-        sort=__ret__.sort,
-        updated_after=__ret__.updated_after,
-        updated_before=__ret__.updated_before,
-        weight=__ret__.weight,
-        with_labels_details=__ret__.with_labels_details)
+        assignee_id=pulumi.get(__ret__, 'assignee_id'),
+        assignee_username=pulumi.get(__ret__, 'assignee_username'),
+        author_id=pulumi.get(__ret__, 'author_id'),
+        confidential=pulumi.get(__ret__, 'confidential'),
+        created_after=pulumi.get(__ret__, 'created_after'),
+        created_before=pulumi.get(__ret__, 'created_before'),
+        due_date=pulumi.get(__ret__, 'due_date'),
+        id=pulumi.get(__ret__, 'id'),
+        iids=pulumi.get(__ret__, 'iids'),
+        issue_type=pulumi.get(__ret__, 'issue_type'),
+        issues=pulumi.get(__ret__, 'issues'),
+        labels=pulumi.get(__ret__, 'labels'),
+        milestone=pulumi.get(__ret__, 'milestone'),
+        my_reaction_emoji=pulumi.get(__ret__, 'my_reaction_emoji'),
+        not_assignee_ids=pulumi.get(__ret__, 'not_assignee_ids'),
+        not_author_ids=pulumi.get(__ret__, 'not_author_ids'),
+        not_labels=pulumi.get(__ret__, 'not_labels'),
+        not_milestone=pulumi.get(__ret__, 'not_milestone'),
+        not_my_reaction_emojis=pulumi.get(__ret__, 'not_my_reaction_emojis'),
+        order_by=pulumi.get(__ret__, 'order_by'),
+        project=pulumi.get(__ret__, 'project'),
+        scope=pulumi.get(__ret__, 'scope'),
+        search=pulumi.get(__ret__, 'search'),
+        sort=pulumi.get(__ret__, 'sort'),
+        updated_after=pulumi.get(__ret__, 'updated_after'),
+        updated_before=pulumi.get(__ret__, 'updated_before'),
+        weight=pulumi.get(__ret__, 'weight'),
+        with_labels_details=pulumi.get(__ret__, 'with_labels_details'))
 
 
 @_utilities.lift_output_func(get_project_issues)
 def get_project_issues_output(assignee_id: Optional[pulumi.Input[Optional[int]]] = None,
                               assignee_username: Optional[pulumi.Input[Optional[str]]] = None,
                               author_id: Optional[pulumi.Input[Optional[int]]] = None,
                               confidential: Optional[pulumi.Input[Optional[bool]]] = None,
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_membership.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_membership.py`

 * *Files 6% similar despite different names*

```diff
@@ -138,20 +138,20 @@
     __args__['inherited'] = inherited
     __args__['projectId'] = project_id
     __args__['query'] = query
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getProjectMembership:getProjectMembership', __args__, opts=opts, typ=GetProjectMembershipResult).value
 
     return AwaitableGetProjectMembershipResult(
-        full_path=__ret__.full_path,
-        id=__ret__.id,
-        inherited=__ret__.inherited,
-        members=__ret__.members,
-        project_id=__ret__.project_id,
-        query=__ret__.query)
+        full_path=pulumi.get(__ret__, 'full_path'),
+        id=pulumi.get(__ret__, 'id'),
+        inherited=pulumi.get(__ret__, 'inherited'),
+        members=pulumi.get(__ret__, 'members'),
+        project_id=pulumi.get(__ret__, 'project_id'),
+        query=pulumi.get(__ret__, 'query'))
 
 
 @_utilities.lift_output_func(get_project_membership)
 def get_project_membership_output(full_path: Optional[pulumi.Input[Optional[str]]] = None,
                                   inherited: Optional[pulumi.Input[Optional[bool]]] = None,
                                   project_id: Optional[pulumi.Input[Optional[int]]] = None,
                                   query: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_milestone.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_milestone.py`

 * *Files 4% similar despite different names*

```diff
@@ -225,28 +225,28 @@
     __args__ = dict()
     __args__['milestoneId'] = milestone_id
     __args__['project'] = project
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getProjectMilestone:getProjectMilestone', __args__, opts=opts, typ=GetProjectMilestoneResult).value
 
     return AwaitableGetProjectMilestoneResult(
-        created_at=__ret__.created_at,
-        description=__ret__.description,
-        due_date=__ret__.due_date,
-        expired=__ret__.expired,
-        id=__ret__.id,
-        iid=__ret__.iid,
-        milestone_id=__ret__.milestone_id,
-        project=__ret__.project,
-        project_id=__ret__.project_id,
-        start_date=__ret__.start_date,
-        state=__ret__.state,
-        title=__ret__.title,
-        updated_at=__ret__.updated_at,
-        web_url=__ret__.web_url)
+        created_at=pulumi.get(__ret__, 'created_at'),
+        description=pulumi.get(__ret__, 'description'),
+        due_date=pulumi.get(__ret__, 'due_date'),
+        expired=pulumi.get(__ret__, 'expired'),
+        id=pulumi.get(__ret__, 'id'),
+        iid=pulumi.get(__ret__, 'iid'),
+        milestone_id=pulumi.get(__ret__, 'milestone_id'),
+        project=pulumi.get(__ret__, 'project'),
+        project_id=pulumi.get(__ret__, 'project_id'),
+        start_date=pulumi.get(__ret__, 'start_date'),
+        state=pulumi.get(__ret__, 'state'),
+        title=pulumi.get(__ret__, 'title'),
+        updated_at=pulumi.get(__ret__, 'updated_at'),
+        web_url=pulumi.get(__ret__, 'web_url'))
 
 
 @_utilities.lift_output_func(get_project_milestone)
 def get_project_milestone_output(milestone_id: Optional[pulumi.Input[int]] = None,
                                  project: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectMilestoneResult]:
     """
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_milestones.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_milestones.py`

 * *Files 6% similar despite different names*

```diff
@@ -165,22 +165,22 @@
     __args__['search'] = search
     __args__['state'] = state
     __args__['title'] = title
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getProjectMilestones:getProjectMilestones', __args__, opts=opts, typ=GetProjectMilestonesResult).value
 
     return AwaitableGetProjectMilestonesResult(
-        id=__ret__.id,
-        iids=__ret__.iids,
-        include_parent_milestones=__ret__.include_parent_milestones,
-        milestones=__ret__.milestones,
-        project=__ret__.project,
-        search=__ret__.search,
-        state=__ret__.state,
-        title=__ret__.title)
+        id=pulumi.get(__ret__, 'id'),
+        iids=pulumi.get(__ret__, 'iids'),
+        include_parent_milestones=pulumi.get(__ret__, 'include_parent_milestones'),
+        milestones=pulumi.get(__ret__, 'milestones'),
+        project=pulumi.get(__ret__, 'project'),
+        search=pulumi.get(__ret__, 'search'),
+        state=pulumi.get(__ret__, 'state'),
+        title=pulumi.get(__ret__, 'title'))
 
 
 @_utilities.lift_output_func(get_project_milestones)
 def get_project_milestones_output(iids: Optional[pulumi.Input[Optional[Sequence[int]]]] = None,
                                   include_parent_milestones: Optional[pulumi.Input[Optional[bool]]] = None,
                                   project: Optional[pulumi.Input[str]] = None,
                                   search: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_protected_branch.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_protected_branch.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,21 +142,21 @@
     __args__ = dict()
     __args__['name'] = name
     __args__['projectId'] = project_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getProjectProtectedBranch:getProjectProtectedBranch', __args__, opts=opts, typ=GetProjectProtectedBranchResult).value
 
     return AwaitableGetProjectProtectedBranchResult(
-        allow_force_push=__ret__.allow_force_push,
-        code_owner_approval_required=__ret__.code_owner_approval_required,
-        id=__ret__.id,
-        merge_access_levels=__ret__.merge_access_levels,
-        name=__ret__.name,
-        project_id=__ret__.project_id,
-        push_access_levels=__ret__.push_access_levels)
+        allow_force_push=pulumi.get(__ret__, 'allow_force_push'),
+        code_owner_approval_required=pulumi.get(__ret__, 'code_owner_approval_required'),
+        id=pulumi.get(__ret__, 'id'),
+        merge_access_levels=pulumi.get(__ret__, 'merge_access_levels'),
+        name=pulumi.get(__ret__, 'name'),
+        project_id=pulumi.get(__ret__, 'project_id'),
+        push_access_levels=pulumi.get(__ret__, 'push_access_levels'))
 
 
 @_utilities.lift_output_func(get_project_protected_branch)
 def get_project_protected_branch_output(name: Optional[pulumi.Input[str]] = None,
                                         project_id: Optional[pulumi.Input[str]] = None,
                                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectProtectedBranchResult]:
     """
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_protected_branches.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_protected_branches.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,17 +90,17 @@
     """
     __args__ = dict()
     __args__['projectId'] = project_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getProjectProtectedBranches:getProjectProtectedBranches', __args__, opts=opts, typ=GetProjectProtectedBranchesResult).value
 
     return AwaitableGetProjectProtectedBranchesResult(
-        id=__ret__.id,
-        project_id=__ret__.project_id,
-        protected_branches=__ret__.protected_branches)
+        id=pulumi.get(__ret__, 'id'),
+        project_id=pulumi.get(__ret__, 'project_id'),
+        protected_branches=pulumi.get(__ret__, 'protected_branches'))
 
 
 @_utilities.lift_output_func(get_project_protected_branches)
 def get_project_protected_branches_output(project_id: Optional[pulumi.Input[str]] = None,
                                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectProtectedBranchesResult]:
     """
     The `get_project_protected_branches` data source allows details of the protected branches of a given project.
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_tag.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_tag.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,22 +154,22 @@
     __args__ = dict()
     __args__['name'] = name
     __args__['project'] = project
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getProjectTag:getProjectTag', __args__, opts=opts, typ=GetProjectTagResult).value
 
     return AwaitableGetProjectTagResult(
-        commits=__ret__.commits,
-        id=__ret__.id,
-        message=__ret__.message,
-        name=__ret__.name,
-        project=__ret__.project,
-        protected=__ret__.protected,
-        releases=__ret__.releases,
-        target=__ret__.target)
+        commits=pulumi.get(__ret__, 'commits'),
+        id=pulumi.get(__ret__, 'id'),
+        message=pulumi.get(__ret__, 'message'),
+        name=pulumi.get(__ret__, 'name'),
+        project=pulumi.get(__ret__, 'project'),
+        protected=pulumi.get(__ret__, 'protected'),
+        releases=pulumi.get(__ret__, 'releases'),
+        target=pulumi.get(__ret__, 'target'))
 
 
 @_utilities.lift_output_func(get_project_tag)
 def get_project_tag_output(name: Optional[pulumi.Input[str]] = None,
                            project: Optional[pulumi.Input[str]] = None,
                            opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectTagResult]:
     """
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_tags.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,20 +135,20 @@
     __args__['project'] = project
     __args__['search'] = search
     __args__['sort'] = sort
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getProjectTags:getProjectTags', __args__, opts=opts, typ=GetProjectTagsResult).value
 
     return AwaitableGetProjectTagsResult(
-        id=__ret__.id,
-        order_by=__ret__.order_by,
-        project=__ret__.project,
-        search=__ret__.search,
-        sort=__ret__.sort,
-        tags=__ret__.tags)
+        id=pulumi.get(__ret__, 'id'),
+        order_by=pulumi.get(__ret__, 'order_by'),
+        project=pulumi.get(__ret__, 'project'),
+        search=pulumi.get(__ret__, 'search'),
+        sort=pulumi.get(__ret__, 'sort'),
+        tags=pulumi.get(__ret__, 'tags'))
 
 
 @_utilities.lift_output_func(get_project_tags)
 def get_project_tags_output(order_by: Optional[pulumi.Input[Optional[str]]] = None,
                             project: Optional[pulumi.Input[str]] = None,
                             search: Optional[pulumi.Input[Optional[str]]] = None,
                             sort: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_variable.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_variable.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,23 +171,23 @@
     __args__['environmentScope'] = environment_scope
     __args__['key'] = key
     __args__['project'] = project
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getProjectVariable:getProjectVariable', __args__, opts=opts, typ=GetProjectVariableResult).value
 
     return AwaitableGetProjectVariableResult(
-        environment_scope=__ret__.environment_scope,
-        id=__ret__.id,
-        key=__ret__.key,
-        masked=__ret__.masked,
-        project=__ret__.project,
-        protected=__ret__.protected,
-        raw=__ret__.raw,
-        value=__ret__.value,
-        variable_type=__ret__.variable_type)
+        environment_scope=pulumi.get(__ret__, 'environment_scope'),
+        id=pulumi.get(__ret__, 'id'),
+        key=pulumi.get(__ret__, 'key'),
+        masked=pulumi.get(__ret__, 'masked'),
+        project=pulumi.get(__ret__, 'project'),
+        protected=pulumi.get(__ret__, 'protected'),
+        raw=pulumi.get(__ret__, 'raw'),
+        value=pulumi.get(__ret__, 'value'),
+        variable_type=pulumi.get(__ret__, 'variable_type'))
 
 
 @_utilities.lift_output_func(get_project_variable)
 def get_project_variable_output(environment_scope: Optional[pulumi.Input[Optional[str]]] = None,
                                 key: Optional[pulumi.Input[str]] = None,
                                 project: Optional[pulumi.Input[str]] = None,
                                 opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectVariableResult]:
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_project_variables.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_project_variables.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,18 +107,18 @@
     __args__ = dict()
     __args__['environmentScope'] = environment_scope
     __args__['project'] = project
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getProjectVariables:getProjectVariables', __args__, opts=opts, typ=GetProjectVariablesResult).value
 
     return AwaitableGetProjectVariablesResult(
-        environment_scope=__ret__.environment_scope,
-        id=__ret__.id,
-        project=__ret__.project,
-        variables=__ret__.variables)
+        environment_scope=pulumi.get(__ret__, 'environment_scope'),
+        id=pulumi.get(__ret__, 'id'),
+        project=pulumi.get(__ret__, 'project'),
+        variables=pulumi.get(__ret__, 'variables'))
 
 
 @_utilities.lift_output_func(get_project_variables)
 def get_project_variables_output(environment_scope: Optional[pulumi.Input[Optional[str]]] = None,
                                  project: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetProjectVariablesResult]:
     """
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_projects.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_projects.py`

 * *Files 4% similar despite different names*

```diff
@@ -400,37 +400,37 @@
     __args__['withMergeRequestsEnabled'] = with_merge_requests_enabled
     __args__['withProgrammingLanguage'] = with_programming_language
     __args__['withShared'] = with_shared
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getProjects:getProjects', __args__, opts=opts, typ=GetProjectsResult).value
 
     return AwaitableGetProjectsResult(
-        archived=__ret__.archived,
-        group_id=__ret__.group_id,
-        id=__ret__.id,
-        include_subgroups=__ret__.include_subgroups,
-        max_queryable_pages=__ret__.max_queryable_pages,
-        membership=__ret__.membership,
-        min_access_level=__ret__.min_access_level,
-        order_by=__ret__.order_by,
-        owned=__ret__.owned,
-        page=__ret__.page,
-        per_page=__ret__.per_page,
-        projects=__ret__.projects,
-        search=__ret__.search,
-        simple=__ret__.simple,
-        sort=__ret__.sort,
-        starred=__ret__.starred,
-        statistics=__ret__.statistics,
-        visibility=__ret__.visibility,
-        with_custom_attributes=__ret__.with_custom_attributes,
-        with_issues_enabled=__ret__.with_issues_enabled,
-        with_merge_requests_enabled=__ret__.with_merge_requests_enabled,
-        with_programming_language=__ret__.with_programming_language,
-        with_shared=__ret__.with_shared)
+        archived=pulumi.get(__ret__, 'archived'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'),
+        include_subgroups=pulumi.get(__ret__, 'include_subgroups'),
+        max_queryable_pages=pulumi.get(__ret__, 'max_queryable_pages'),
+        membership=pulumi.get(__ret__, 'membership'),
+        min_access_level=pulumi.get(__ret__, 'min_access_level'),
+        order_by=pulumi.get(__ret__, 'order_by'),
+        owned=pulumi.get(__ret__, 'owned'),
+        page=pulumi.get(__ret__, 'page'),
+        per_page=pulumi.get(__ret__, 'per_page'),
+        projects=pulumi.get(__ret__, 'projects'),
+        search=pulumi.get(__ret__, 'search'),
+        simple=pulumi.get(__ret__, 'simple'),
+        sort=pulumi.get(__ret__, 'sort'),
+        starred=pulumi.get(__ret__, 'starred'),
+        statistics=pulumi.get(__ret__, 'statistics'),
+        visibility=pulumi.get(__ret__, 'visibility'),
+        with_custom_attributes=pulumi.get(__ret__, 'with_custom_attributes'),
+        with_issues_enabled=pulumi.get(__ret__, 'with_issues_enabled'),
+        with_merge_requests_enabled=pulumi.get(__ret__, 'with_merge_requests_enabled'),
+        with_programming_language=pulumi.get(__ret__, 'with_programming_language'),
+        with_shared=pulumi.get(__ret__, 'with_shared'))
 
 
 @_utilities.lift_output_func(get_projects)
 def get_projects_output(archived: Optional[pulumi.Input[Optional[bool]]] = None,
                         group_id: Optional[pulumi.Input[Optional[int]]] = None,
                         include_subgroups: Optional[pulumi.Input[Optional[bool]]] = None,
                         max_queryable_pages: Optional[pulumi.Input[Optional[int]]] = None,
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_release_link.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_release_link.py`

 * *Files 4% similar despite different names*

```diff
@@ -181,24 +181,24 @@
     __args__['linkId'] = link_id
     __args__['project'] = project
     __args__['tagName'] = tag_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getReleaseLink:getReleaseLink', __args__, opts=opts, typ=GetReleaseLinkResult).value
 
     return AwaitableGetReleaseLinkResult(
-        direct_asset_url=__ret__.direct_asset_url,
-        external=__ret__.external,
-        filepath=__ret__.filepath,
-        id=__ret__.id,
-        link_id=__ret__.link_id,
-        link_type=__ret__.link_type,
-        name=__ret__.name,
-        project=__ret__.project,
-        tag_name=__ret__.tag_name,
-        url=__ret__.url)
+        direct_asset_url=pulumi.get(__ret__, 'direct_asset_url'),
+        external=pulumi.get(__ret__, 'external'),
+        filepath=pulumi.get(__ret__, 'filepath'),
+        id=pulumi.get(__ret__, 'id'),
+        link_id=pulumi.get(__ret__, 'link_id'),
+        link_type=pulumi.get(__ret__, 'link_type'),
+        name=pulumi.get(__ret__, 'name'),
+        project=pulumi.get(__ret__, 'project'),
+        tag_name=pulumi.get(__ret__, 'tag_name'),
+        url=pulumi.get(__ret__, 'url'))
 
 
 @_utilities.lift_output_func(get_release_link)
 def get_release_link_output(link_id: Optional[pulumi.Input[int]] = None,
                             project: Optional[pulumi.Input[str]] = None,
                             tag_name: Optional[pulumi.Input[str]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetReleaseLinkResult]:
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_release_links.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_release_links.py`

 * *Files 12% similar despite different names*

```diff
@@ -106,18 +106,18 @@
     __args__ = dict()
     __args__['project'] = project
     __args__['tagName'] = tag_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getReleaseLinks:getReleaseLinks', __args__, opts=opts, typ=GetReleaseLinksResult).value
 
     return AwaitableGetReleaseLinksResult(
-        id=__ret__.id,
-        project=__ret__.project,
-        release_links=__ret__.release_links,
-        tag_name=__ret__.tag_name)
+        id=pulumi.get(__ret__, 'id'),
+        project=pulumi.get(__ret__, 'project'),
+        release_links=pulumi.get(__ret__, 'release_links'),
+        tag_name=pulumi.get(__ret__, 'tag_name'))
 
 
 @_utilities.lift_output_func(get_release_links)
 def get_release_links_output(project: Optional[pulumi.Input[str]] = None,
                              tag_name: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetReleaseLinksResult]:
     """
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_repository_file.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_repository_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -217,27 +217,27 @@
     __args__['filePath'] = file_path
     __args__['project'] = project
     __args__['ref'] = ref
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getRepositoryFile:getRepositoryFile', __args__, opts=opts, typ=GetRepositoryFileResult).value
 
     return AwaitableGetRepositoryFileResult(
-        blob_id=__ret__.blob_id,
-        commit_id=__ret__.commit_id,
-        content=__ret__.content,
-        content_sha256=__ret__.content_sha256,
-        encoding=__ret__.encoding,
-        execute_filemode=__ret__.execute_filemode,
-        file_name=__ret__.file_name,
-        file_path=__ret__.file_path,
-        id=__ret__.id,
-        last_commit_id=__ret__.last_commit_id,
-        project=__ret__.project,
-        ref=__ret__.ref,
-        size=__ret__.size)
+        blob_id=pulumi.get(__ret__, 'blob_id'),
+        commit_id=pulumi.get(__ret__, 'commit_id'),
+        content=pulumi.get(__ret__, 'content'),
+        content_sha256=pulumi.get(__ret__, 'content_sha256'),
+        encoding=pulumi.get(__ret__, 'encoding'),
+        execute_filemode=pulumi.get(__ret__, 'execute_filemode'),
+        file_name=pulumi.get(__ret__, 'file_name'),
+        file_path=pulumi.get(__ret__, 'file_path'),
+        id=pulumi.get(__ret__, 'id'),
+        last_commit_id=pulumi.get(__ret__, 'last_commit_id'),
+        project=pulumi.get(__ret__, 'project'),
+        ref=pulumi.get(__ret__, 'ref'),
+        size=pulumi.get(__ret__, 'size'))
 
 
 @_utilities.lift_output_func(get_repository_file)
 def get_repository_file_output(file_path: Optional[pulumi.Input[str]] = None,
                                project: Optional[pulumi.Input[str]] = None,
                                ref: Optional[pulumi.Input[str]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRepositoryFileResult]:
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_repository_tree.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_repository_tree.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,20 +138,20 @@
     __args__['project'] = project
     __args__['recursive'] = recursive
     __args__['ref'] = ref
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getRepositoryTree:getRepositoryTree', __args__, opts=opts, typ=GetRepositoryTreeResult).value
 
     return AwaitableGetRepositoryTreeResult(
-        id=__ret__.id,
-        path=__ret__.path,
-        project=__ret__.project,
-        recursive=__ret__.recursive,
-        ref=__ret__.ref,
-        trees=__ret__.trees)
+        id=pulumi.get(__ret__, 'id'),
+        path=pulumi.get(__ret__, 'path'),
+        project=pulumi.get(__ret__, 'project'),
+        recursive=pulumi.get(__ret__, 'recursive'),
+        ref=pulumi.get(__ret__, 'ref'),
+        trees=pulumi.get(__ret__, 'trees'))
 
 
 @_utilities.lift_output_func(get_repository_tree)
 def get_repository_tree_output(path: Optional[pulumi.Input[Optional[str]]] = None,
                                project: Optional[pulumi.Input[str]] = None,
                                recursive: Optional[pulumi.Input[Optional[bool]]] = None,
                                ref: Optional[pulumi.Input[str]] = None,
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_user.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_user.py`

 * *Files 10% similar despite different names*

```diff
@@ -403,43 +403,43 @@
     __args__['namespaceId'] = namespace_id
     __args__['userId'] = user_id
     __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getUser:getUser', __args__, opts=opts, typ=GetUserResult).value
 
     return AwaitableGetUserResult(
-        avatar_url=__ret__.avatar_url,
-        bio=__ret__.bio,
-        can_create_group=__ret__.can_create_group,
-        can_create_project=__ret__.can_create_project,
-        color_scheme_id=__ret__.color_scheme_id,
-        created_at=__ret__.created_at,
-        current_sign_in_at=__ret__.current_sign_in_at,
-        email=__ret__.email,
-        extern_uid=__ret__.extern_uid,
-        external=__ret__.external,
-        id=__ret__.id,
-        is_admin=__ret__.is_admin,
-        last_sign_in_at=__ret__.last_sign_in_at,
-        linkedin=__ret__.linkedin,
-        location=__ret__.location,
-        name=__ret__.name,
-        namespace_id=__ret__.namespace_id,
-        note=__ret__.note,
-        organization=__ret__.organization,
-        projects_limit=__ret__.projects_limit,
-        skype=__ret__.skype,
-        state=__ret__.state,
-        theme_id=__ret__.theme_id,
-        twitter=__ret__.twitter,
-        two_factor_enabled=__ret__.two_factor_enabled,
-        user_id=__ret__.user_id,
-        user_provider=__ret__.user_provider,
-        username=__ret__.username,
-        website_url=__ret__.website_url)
+        avatar_url=pulumi.get(__ret__, 'avatar_url'),
+        bio=pulumi.get(__ret__, 'bio'),
+        can_create_group=pulumi.get(__ret__, 'can_create_group'),
+        can_create_project=pulumi.get(__ret__, 'can_create_project'),
+        color_scheme_id=pulumi.get(__ret__, 'color_scheme_id'),
+        created_at=pulumi.get(__ret__, 'created_at'),
+        current_sign_in_at=pulumi.get(__ret__, 'current_sign_in_at'),
+        email=pulumi.get(__ret__, 'email'),
+        extern_uid=pulumi.get(__ret__, 'extern_uid'),
+        external=pulumi.get(__ret__, 'external'),
+        id=pulumi.get(__ret__, 'id'),
+        is_admin=pulumi.get(__ret__, 'is_admin'),
+        last_sign_in_at=pulumi.get(__ret__, 'last_sign_in_at'),
+        linkedin=pulumi.get(__ret__, 'linkedin'),
+        location=pulumi.get(__ret__, 'location'),
+        name=pulumi.get(__ret__, 'name'),
+        namespace_id=pulumi.get(__ret__, 'namespace_id'),
+        note=pulumi.get(__ret__, 'note'),
+        organization=pulumi.get(__ret__, 'organization'),
+        projects_limit=pulumi.get(__ret__, 'projects_limit'),
+        skype=pulumi.get(__ret__, 'skype'),
+        state=pulumi.get(__ret__, 'state'),
+        theme_id=pulumi.get(__ret__, 'theme_id'),
+        twitter=pulumi.get(__ret__, 'twitter'),
+        two_factor_enabled=pulumi.get(__ret__, 'two_factor_enabled'),
+        user_id=pulumi.get(__ret__, 'user_id'),
+        user_provider=pulumi.get(__ret__, 'user_provider'),
+        username=pulumi.get(__ret__, 'username'),
+        website_url=pulumi.get(__ret__, 'website_url'))
 
 
 @_utilities.lift_output_func(get_user)
 def get_user_output(email: Optional[pulumi.Input[Optional[str]]] = None,
                     namespace_id: Optional[pulumi.Input[Optional[int]]] = None,
                     user_id: Optional[pulumi.Input[Optional[int]]] = None,
                     username: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_user_sshkeys.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_user_sshkeys.py`

 * *Files 7% similar despite different names*

```diff
@@ -96,18 +96,18 @@
     __args__ = dict()
     __args__['userId'] = user_id
     __args__['username'] = username
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getUserSshkeys:getUserSshkeys', __args__, opts=opts, typ=GetUserSshkeysResult).value
 
     return AwaitableGetUserSshkeysResult(
-        id=__ret__.id,
-        keys=__ret__.keys,
-        user_id=__ret__.user_id,
-        username=__ret__.username)
+        id=pulumi.get(__ret__, 'id'),
+        keys=pulumi.get(__ret__, 'keys'),
+        user_id=pulumi.get(__ret__, 'user_id'),
+        username=pulumi.get(__ret__, 'username'))
 
 
 @_utilities.lift_output_func(get_user_sshkeys)
 def get_user_sshkeys_output(user_id: Optional[pulumi.Input[Optional[int]]] = None,
                             username: Optional[pulumi.Input[Optional[str]]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserSshkeysResult]:
     """
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/get_users.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/get_users.py`

 * *Files 4% similar despite different names*

```diff
@@ -217,25 +217,25 @@
     __args__['orderBy'] = order_by
     __args__['search'] = search
     __args__['sort'] = sort
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('gitlab:index/getUsers:getUsers', __args__, opts=opts, typ=GetUsersResult).value
 
     return AwaitableGetUsersResult(
-        active=__ret__.active,
-        blocked=__ret__.blocked,
-        created_after=__ret__.created_after,
-        created_before=__ret__.created_before,
-        extern_provider=__ret__.extern_provider,
-        extern_uid=__ret__.extern_uid,
-        id=__ret__.id,
-        order_by=__ret__.order_by,
-        search=__ret__.search,
-        sort=__ret__.sort,
-        users=__ret__.users)
+        active=pulumi.get(__ret__, 'active'),
+        blocked=pulumi.get(__ret__, 'blocked'),
+        created_after=pulumi.get(__ret__, 'created_after'),
+        created_before=pulumi.get(__ret__, 'created_before'),
+        extern_provider=pulumi.get(__ret__, 'extern_provider'),
+        extern_uid=pulumi.get(__ret__, 'extern_uid'),
+        id=pulumi.get(__ret__, 'id'),
+        order_by=pulumi.get(__ret__, 'order_by'),
+        search=pulumi.get(__ret__, 'search'),
+        sort=pulumi.get(__ret__, 'sort'),
+        users=pulumi.get(__ret__, 'users'))
 
 
 @_utilities.lift_output_func(get_users)
 def get_users_output(active: Optional[pulumi.Input[Optional[bool]]] = None,
                      blocked: Optional[pulumi.Input[Optional[bool]]] = None,
                      created_after: Optional[pulumi.Input[Optional[str]]] = None,
                      created_before: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_access_token.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_badge.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_badge.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_cluster.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_custom_attribute.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_hook.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_label.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_label.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_ldap_link.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_ldap_link.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,17 @@
 
     @property
     @pulumi.getter(name="accessLevel")
     def access_level(self) -> Optional[pulumi.Input[str]]:
         """
         Minimum access level for members of the LDAP group. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         """
+        warnings.warn("""Use `group_access` instead of the `access_level` attribute.""", DeprecationWarning)
+        pulumi.log.warn("""access_level is deprecated: Use `group_access` instead of the `access_level` attribute.""")
+
         return pulumi.get(self, "access_level")
 
     @access_level.setter
     def access_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "access_level", value)
 
     @property
@@ -172,14 +175,17 @@
 
     @property
     @pulumi.getter(name="accessLevel")
     def access_level(self) -> Optional[pulumi.Input[str]]:
         """
         Minimum access level for members of the LDAP group. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         """
+        warnings.warn("""Use `group_access` instead of the `access_level` attribute.""", DeprecationWarning)
+        pulumi.log.warn("""access_level is deprecated: Use `group_access` instead of the `access_level` attribute.""")
+
         return pulumi.get(self, "access_level")
 
     @access_level.setter
     def access_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "access_level", value)
 
     @property
@@ -414,14 +420,17 @@
 
     @property
     @pulumi.getter(name="accessLevel")
     def access_level(self) -> pulumi.Output[Optional[str]]:
         """
         Minimum access level for members of the LDAP group. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         """
+        warnings.warn("""Use `group_access` instead of the `access_level` attribute.""", DeprecationWarning)
+        pulumi.log.warn("""access_level is deprecated: Use `group_access` instead of the `access_level` attribute.""")
+
         return pulumi.get(self, "access_level")
 
     @property
     @pulumi.getter
     def cn(self) -> pulumi.Output[str]:
         """
         The CN of the LDAP group to link with. Required if `filter` is not provided.
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_membership.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_project_file_template.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_project_file_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_saml_link.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_saml_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_share_group.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_share_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/group_variable.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/group_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/instance_cluster.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/instance_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/instance_variable.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/instance_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/integration_custom_issue_tracker.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/integration_custom_issue_tracker.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/integration_emails_on_push.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/integration_emails_on_push.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/integration_external_wiki.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/integration_external_wiki.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/integration_github.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/integration_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/integration_jira.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/integration_jira.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/integration_microsoft_teams.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/integration_microsoft_teams.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/integration_pipelines_email.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/integration_pipelines_email.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/integration_slack.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/integration_slack.py`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,17 @@
 
     @property
     @pulumi.getter(name="notifyOnlyDefaultBranch")
     def notify_only_default_branch(self) -> Optional[pulumi.Input[bool]]:
         """
         This parameter has been replaced with `branches_to_be_notified`.
         """
+        warnings.warn("""use 'branches_to_be_notified' argument instead""", DeprecationWarning)
+        pulumi.log.warn("""notify_only_default_branch is deprecated: use 'branches_to_be_notified' argument instead""")
+
         return pulumi.get(self, "notify_only_default_branch")
 
     @notify_only_default_branch.setter
     def notify_only_default_branch(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "notify_only_default_branch", value)
 
     @property
@@ -640,14 +643,17 @@
 
     @property
     @pulumi.getter(name="notifyOnlyDefaultBranch")
     def notify_only_default_branch(self) -> Optional[pulumi.Input[bool]]:
         """
         This parameter has been replaced with `branches_to_be_notified`.
         """
+        warnings.warn("""use 'branches_to_be_notified' argument instead""", DeprecationWarning)
+        pulumi.log.warn("""notify_only_default_branch is deprecated: use 'branches_to_be_notified' argument instead""")
+
         return pulumi.get(self, "notify_only_default_branch")
 
     @notify_only_default_branch.setter
     def notify_only_default_branch(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "notify_only_default_branch", value)
 
     @property
@@ -1176,14 +1182,17 @@
 
     @property
     @pulumi.getter(name="notifyOnlyDefaultBranch")
     def notify_only_default_branch(self) -> pulumi.Output[bool]:
         """
         This parameter has been replaced with `branches_to_be_notified`.
         """
+        warnings.warn("""use 'branches_to_be_notified' argument instead""", DeprecationWarning)
+        pulumi.log.warn("""notify_only_default_branch is deprecated: use 'branches_to_be_notified' argument instead""")
+
         return pulumi.get(self, "notify_only_default_branch")
 
     @property
     @pulumi.getter(name="pipelineChannel")
     def pipeline_channel(self) -> pulumi.Output[Optional[str]]:
         """
         The name of the channel to receive pipeline events notifications.
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/label.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/label.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/outputs.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
     'ProjectContainerExpirationPolicy',
     'ProjectIssueBoardList',
     'ProjectIssueTaskCompletionStatus',
     'ProjectProtectedEnvironmentDeployAccessLevel',
     'ProjectPushRules',
     'ProjectTagCommit',
     'ProjectTagRelease',
+    'TagProtectionAllowedToCreate',
     'GetBranchCommitResult',
     'GetClusterAgentsClusterAgentResult',
     'GetGroupHooksHookResult',
     'GetGroupMembershipMemberResult',
     'GetGroupSubgroupsSubgroupResult',
     'GetGroupVariablesVariableResult',
     'GetGroupsGroupResult',
@@ -522,14 +523,17 @@
 
     @property
     @pulumi.getter(name="nameRegex")
     def name_regex(self) -> Optional[str]:
         """
         The regular expression to match image names to delete.
         """
+        warnings.warn("""`name_regex` has been deprecated. Use `name_regex_delete` instead.""", DeprecationWarning)
+        pulumi.log.warn("""name_regex is deprecated: `name_regex` has been deprecated. Use `name_regex_delete` instead.""")
+
         return pulumi.get(self, "name_regex")
 
     @property
     @pulumi.getter(name="nameRegexDelete")
     def name_regex_delete(self) -> Optional[str]:
         """
         The regular expression to match image names to delete.
@@ -1124,14 +1128,92 @@
     @property
     @pulumi.getter(name="tagName")
     def tag_name(self) -> Optional[str]:
         return pulumi.get(self, "tag_name")
 
 
 @pulumi.output_type
+class TagProtectionAllowedToCreate(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "accessLevel":
+            suggest = "access_level"
+        elif key == "accessLevelDescription":
+            suggest = "access_level_description"
+        elif key == "groupId":
+            suggest = "group_id"
+        elif key == "userId":
+            suggest = "user_id"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in TagProtectionAllowedToCreate. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        TagProtectionAllowedToCreate.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        TagProtectionAllowedToCreate.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 access_level: Optional[str] = None,
+                 access_level_description: Optional[str] = None,
+                 group_id: Optional[int] = None,
+                 user_id: Optional[int] = None):
+        """
+        :param str access_level: Level of access.
+        :param str access_level_description: Readable description of level of access.
+        :param int group_id: The ID of a GitLab group allowed to perform the relevant action. Mutually exclusive with `user_id`.
+        :param int user_id: The ID of a GitLab user allowed to perform the relevant action. Mutually exclusive with `group_id`.
+        """
+        if access_level is not None:
+            pulumi.set(__self__, "access_level", access_level)
+        if access_level_description is not None:
+            pulumi.set(__self__, "access_level_description", access_level_description)
+        if group_id is not None:
+            pulumi.set(__self__, "group_id", group_id)
+        if user_id is not None:
+            pulumi.set(__self__, "user_id", user_id)
+
+    @property
+    @pulumi.getter(name="accessLevel")
+    def access_level(self) -> Optional[str]:
+        """
+        Level of access.
+        """
+        return pulumi.get(self, "access_level")
+
+    @property
+    @pulumi.getter(name="accessLevelDescription")
+    def access_level_description(self) -> Optional[str]:
+        """
+        Readable description of level of access.
+        """
+        return pulumi.get(self, "access_level_description")
+
+    @property
+    @pulumi.getter(name="groupId")
+    def group_id(self) -> Optional[int]:
+        """
+        The ID of a GitLab group allowed to perform the relevant action. Mutually exclusive with `user_id`.
+        """
+        return pulumi.get(self, "group_id")
+
+    @property
+    @pulumi.getter(name="userId")
+    def user_id(self) -> Optional[int]:
+        """
+        The ID of a GitLab user allowed to perform the relevant action. Mutually exclusive with `group_id`.
+        """
+        return pulumi.get(self, "user_id")
+
+
+@pulumi.output_type
 class GetBranchCommitResult(dict):
     def __init__(__self__, *,
                  author_email: str,
                  author_name: str,
                  authored_date: str,
                  committed_date: str,
                  committer_email: str,
@@ -2237,14 +2319,17 @@
     @pulumi.getter(name="keepN")
     def keep_n(self) -> int:
         return pulumi.get(self, "keep_n")
 
     @property
     @pulumi.getter(name="nameRegex")
     def name_regex(self) -> str:
+        warnings.warn("""`name_regex` has been deprecated. Use `name_regex_delete` instead.""", DeprecationWarning)
+        pulumi.log.warn("""name_regex is deprecated: `name_regex` has been deprecated. Use `name_regex_delete` instead.""")
+
         return pulumi.get(self, "name_regex")
 
     @property
     @pulumi.getter(name="nameRegexDelete")
     def name_regex_delete(self) -> str:
         return pulumi.get(self, "name_regex_delete")
 
@@ -4249,14 +4334,17 @@
     @pulumi.getter(name="keepN")
     def keep_n(self) -> int:
         return pulumi.get(self, "keep_n")
 
     @property
     @pulumi.getter(name="nameRegex")
     def name_regex(self) -> str:
+        warnings.warn("""`name_regex` has been deprecated. Use `name_regex_delete` instead.""", DeprecationWarning)
+        pulumi.log.warn("""name_regex is deprecated: `name_regex` has been deprecated. Use `name_regex_delete` instead.""")
+
         return pulumi.get(self, "name_regex")
 
     @property
     @pulumi.getter(name="nameRegexDelete")
     def name_regex_delete(self) -> str:
         return pulumi.get(self, "name_regex_delete")
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/pages_domain.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/pages_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/personal_access_token.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/personal_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/pipeline_schedule.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/pipeline_schedule_variable.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/pipeline_schedule_variable.py`

 * *Files 4% similar despite different names*

```diff
@@ -162,32 +162,14 @@
                  value: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         The `PipelineScheduleVariable` resource allows to manage the lifecycle of a variable for a pipeline schedule.
 
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/pipeline_schedules.html#pipeline-schedule-variables)
 
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_gitlab as gitlab
-
-        example_pipeline_schedule = gitlab.PipelineSchedule("examplePipelineSchedule",
-            project="12345",
-            description="Used to schedule builds",
-            ref="master",
-            cron="0 1 * * *")
-        example_pipeline_schedule_variable = gitlab.PipelineScheduleVariable("examplePipelineScheduleVariable",
-            project=example_pipeline_schedule.project,
-            pipeline_schedule_id=example_pipeline_schedule.id,
-            key="EXAMPLE_KEY",
-            value="example")
-        ```
-
         ## Import
 
         Pipeline schedule variables can be imported using an id made up of `project_id:pipeline_schedule_id:key`, e.g.
 
         ```sh
          $ pulumi import gitlab:index/pipelineScheduleVariable:PipelineScheduleVariable example 123456789:13:mykey
         ```
@@ -206,32 +188,14 @@
                  args: PipelineScheduleVariableArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
         The `PipelineScheduleVariable` resource allows to manage the lifecycle of a variable for a pipeline schedule.
 
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/pipeline_schedules.html#pipeline-schedule-variables)
 
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import pulumi_gitlab as gitlab
-
-        example_pipeline_schedule = gitlab.PipelineSchedule("examplePipelineSchedule",
-            project="12345",
-            description="Used to schedule builds",
-            ref="master",
-            cron="0 1 * * *")
-        example_pipeline_schedule_variable = gitlab.PipelineScheduleVariable("examplePipelineScheduleVariable",
-            project=example_pipeline_schedule.project,
-            pipeline_schedule_id=example_pipeline_schedule.id,
-            key="EXAMPLE_KEY",
-            value="example")
-        ```
-
         ## Import
 
         Pipeline schedule variables can be imported using an id made up of `project_id:pipeline_schedule_id:key`, e.g.
 
         ```sh
          $ pulumi import gitlab:index/pipelineScheduleVariable:PipelineScheduleVariable example 123456789:13:mykey
         ```
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/pipeline_trigger.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/pipeline_trigger.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project.py`

 * *Files 0% similar despite different names*

```diff
@@ -537,14 +537,17 @@
 
     @property
     @pulumi.getter(name="buildCoverageRegex")
     def build_coverage_regex(self) -> Optional[pulumi.Input[str]]:
         """
         Test coverage parsing for the project. This is deprecated feature in GitLab 15.0.
         """
+        warnings.warn("""build_coverage_regex is removed in GitLab 15.0.""", DeprecationWarning)
+        pulumi.log.warn("""build_coverage_regex is deprecated: build_coverage_regex is removed in GitLab 15.0.""")
+
         return pulumi.get(self, "build_coverage_regex")
 
     @build_coverage_regex.setter
     def build_coverage_regex(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "build_coverage_regex", value)
 
     @property
@@ -657,14 +660,17 @@
 
     @property
     @pulumi.getter(name="containerRegistryEnabled")
     def container_registry_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
         Enable container registry for the project.
         """
+        warnings.warn("""Use `container_registry_access_level` instead.""", DeprecationWarning)
+        pulumi.log.warn("""container_registry_enabled is deprecated: Use `container_registry_access_level` instead.""")
+
         return pulumi.get(self, "container_registry_enabled")
 
     @container_registry_enabled.setter
     def container_registry_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "container_registry_enabled", value)
 
     @property
@@ -1145,14 +1151,17 @@
 
     @property
     @pulumi.getter(name="pipelinesEnabled")
     def pipelines_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
         Enable pipelines for the project. The `pipelines_enabled` field is being sent as `jobs_enabled` in the GitLab API calls.
         """
+        warnings.warn("""Deprecated in favor of `builds_access_level`""", DeprecationWarning)
+        pulumi.log.warn("""pipelines_enabled is deprecated: Deprecated in favor of `builds_access_level`""")
+
         return pulumi.get(self, "pipelines_enabled")
 
     @pipelines_enabled.setter
     def pipelines_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "pipelines_enabled", value)
 
     @property
@@ -2044,14 +2053,17 @@
 
     @property
     @pulumi.getter(name="buildCoverageRegex")
     def build_coverage_regex(self) -> Optional[pulumi.Input[str]]:
         """
         Test coverage parsing for the project. This is deprecated feature in GitLab 15.0.
         """
+        warnings.warn("""build_coverage_regex is removed in GitLab 15.0.""", DeprecationWarning)
+        pulumi.log.warn("""build_coverage_regex is deprecated: build_coverage_regex is removed in GitLab 15.0.""")
+
         return pulumi.get(self, "build_coverage_regex")
 
     @build_coverage_regex.setter
     def build_coverage_regex(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "build_coverage_regex", value)
 
     @property
@@ -2164,14 +2176,17 @@
 
     @property
     @pulumi.getter(name="containerRegistryEnabled")
     def container_registry_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
         Enable container registry for the project.
         """
+        warnings.warn("""Use `container_registry_access_level` instead.""", DeprecationWarning)
+        pulumi.log.warn("""container_registry_enabled is deprecated: Use `container_registry_access_level` instead.""")
+
         return pulumi.get(self, "container_registry_enabled")
 
     @container_registry_enabled.setter
     def container_registry_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "container_registry_enabled", value)
 
     @property
@@ -2676,14 +2691,17 @@
 
     @property
     @pulumi.getter(name="pipelinesEnabled")
     def pipelines_enabled(self) -> Optional[pulumi.Input[bool]]:
         """
         Enable pipelines for the project. The `pipelines_enabled` field is being sent as `jobs_enabled` in the GitLab API calls.
         """
+        warnings.warn("""Deprecated in favor of `builds_access_level`""", DeprecationWarning)
+        pulumi.log.warn("""pipelines_enabled is deprecated: Deprecated in favor of `builds_access_level`""")
+
         return pulumi.get(self, "pipelines_enabled")
 
     @pipelines_enabled.setter
     def pipelines_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "pipelines_enabled", value)
 
     @property
@@ -4039,14 +4057,17 @@
 
     @property
     @pulumi.getter(name="buildCoverageRegex")
     def build_coverage_regex(self) -> pulumi.Output[Optional[str]]:
         """
         Test coverage parsing for the project. This is deprecated feature in GitLab 15.0.
         """
+        warnings.warn("""build_coverage_regex is removed in GitLab 15.0.""", DeprecationWarning)
+        pulumi.log.warn("""build_coverage_regex is deprecated: build_coverage_regex is removed in GitLab 15.0.""")
+
         return pulumi.get(self, "build_coverage_regex")
 
     @property
     @pulumi.getter(name="buildGitStrategy")
     def build_git_strategy(self) -> pulumi.Output[str]:
         """
         The Git strategy. Defaults to fetch.
@@ -4119,14 +4140,17 @@
 
     @property
     @pulumi.getter(name="containerRegistryEnabled")
     def container_registry_enabled(self) -> pulumi.Output[bool]:
         """
         Enable container registry for the project.
         """
+        warnings.warn("""Use `container_registry_access_level` instead.""", DeprecationWarning)
+        pulumi.log.warn("""container_registry_enabled is deprecated: Use `container_registry_access_level` instead.""")
+
         return pulumi.get(self, "container_registry_enabled")
 
     @property
     @pulumi.getter(name="defaultBranch")
     def default_branch(self) -> pulumi.Output[str]:
         """
         The default branch for the project.
@@ -4463,14 +4487,17 @@
 
     @property
     @pulumi.getter(name="pipelinesEnabled")
     def pipelines_enabled(self) -> pulumi.Output[bool]:
         """
         Enable pipelines for the project. The `pipelines_enabled` field is being sent as `jobs_enabled` in the GitLab API calls.
         """
+        warnings.warn("""Deprecated in favor of `builds_access_level`""", DeprecationWarning)
+        pulumi.log.warn("""pipelines_enabled is deprecated: Deprecated in favor of `builds_access_level`""")
+
         return pulumi.get(self, "pipelines_enabled")
 
     @property
     @pulumi.getter(name="printingMergeRequestLinkEnabled")
     def printing_merge_request_link_enabled(self) -> pulumi.Output[bool]:
         """
         Show link to create/view merge request when pushing from the command line
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_access_token.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_access_token.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_approval_rule.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_approval_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_badge.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_badge.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_cluster.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_custom_attribute.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_environment.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_freeze_period.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_freeze_period.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_hook.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_issue.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_issue.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_issue_board.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_issue_board.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_label.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_label.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_level_mr_approvals.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_level_mr_approvals.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_membership.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_membership.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_milestone.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_milestone.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_mirror.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_mirror.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_protected_environment.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_protected_environment.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_runner_enablement.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_runner_enablement.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_share_group.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_share_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,17 @@
 
     @property
     @pulumi.getter(name="accessLevel")
     def access_level(self) -> Optional[pulumi.Input[str]]:
         """
         The access level to grant the group for the project. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         """
+        warnings.warn("""Use `group_access` instead of the `access_level` attribute.""", DeprecationWarning)
+        pulumi.log.warn("""access_level is deprecated: Use `group_access` instead of the `access_level` attribute.""")
+
         return pulumi.get(self, "access_level")
 
     @access_level.setter
     def access_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "access_level", value)
 
     @property
@@ -112,14 +115,17 @@
 
     @property
     @pulumi.getter(name="accessLevel")
     def access_level(self) -> Optional[pulumi.Input[str]]:
         """
         The access level to grant the group for the project. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         """
+        warnings.warn("""Use `group_access` instead of the `access_level` attribute.""", DeprecationWarning)
+        pulumi.log.warn("""access_level is deprecated: Use `group_access` instead of the `access_level` attribute.""")
+
         return pulumi.get(self, "access_level")
 
     @access_level.setter
     def access_level(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "access_level", value)
 
     @property
@@ -309,14 +315,17 @@
 
     @property
     @pulumi.getter(name="accessLevel")
     def access_level(self) -> pulumi.Output[Optional[str]]:
         """
         The access level to grant the group for the project. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
         """
+        warnings.warn("""Use `group_access` instead of the `access_level` attribute.""", DeprecationWarning)
+        pulumi.log.warn("""access_level is deprecated: Use `group_access` instead of the `access_level` attribute.""")
+
         return pulumi.get(self, "access_level")
 
     @property
     @pulumi.getter(name="groupAccess")
     def group_access(self) -> pulumi.Output[Optional[str]]:
         """
         The access level to grant the group for the project. Valid values are: `no one`, `minimal`, `guest`, `reporter`, `developer`, `maintainer`, `owner`, `master`
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/project_variable.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/project_variable.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/provider.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/release_link.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/release_link.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/repository_file.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/repository_file.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/runner.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/runner.py`

 * *Files 11% similar despite different names*

```diff
@@ -334,14 +334,59 @@
         The `Runner` resource allows to manage the lifecycle of a runner.
 
         A runner can either be registered at an instance level or group level.
         The runner will be registered at a group level if the token used is from a group, or at an instance level if the token used is for the instance.
 
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/runners.html#register-a-new-runner)
 
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_gitlab as gitlab
+        import pulumi_local as local
+
+        # Basic GitLab Group Runner
+        my_group = gitlab.Group("myGroup", description="group that holds the runners")
+        basic_runner = gitlab.Runner("basicRunner", registration_token=my_group.runners_token)
+        # GitLab Runner that runs only tagged jobs
+        tagged_only = gitlab.Runner("taggedOnly",
+            registration_token=my_group.runners_token,
+            description="I only run tagged jobs",
+            run_untagged=False,
+            tag_lists=[
+                "tag_one",
+                "tag_two",
+            ])
+        # GitLab Runner that only runs on protected branches
+        protected = gitlab.Runner("protected",
+            registration_token=my_group.runners_token,
+            description="I only run protected jobs",
+            access_level="ref_protected")
+        # Generate a `config.toml` file that you can use to create a runner
+        # This is the typical workflow for this resource, using it to create an authentication_token which can then be used
+        # to generate the `config.toml` file to prevent re-registering the runner every time new hardware is created.
+        my_custom_group = gitlab.Group("myCustomGroup", description="group that holds the custom runners")
+        my_runner = gitlab.Runner("myRunner", registration_token=my_custom_group.runners_token)
+        # This creates a configuration for a local "shell" runner, but can be changed to generate whatever is needed.
+        # Place this configuration file on a server at `/etc/gitlab-runner/config.toml`, then run `gitlab-runner start`.
+        # See https://docs.gitlab.com/runner/configuration/advanced-configuration.html for more information.
+        config = local.File("config",
+            filename=f"{path['module']}/config.toml",
+            content=my_runner.authentication_token.apply(lambda authentication_token: f\"\"\"  concurrent = 1
+
+          [[runners]]
+            name = "Hello Terraform"
+            url = "https://example.gitlab.com/"
+            token = "{authentication_token}"
+            executor = "shell"
+            
+        \"\"\"))
+        ```
+
         ## Import
 
         A GitLab Runner can be imported using the runner's ID, eg
 
         ```sh
          $ pulumi import gitlab:index/runner:Runner this 1
         ```
@@ -367,14 +412,59 @@
         The `Runner` resource allows to manage the lifecycle of a runner.
 
         A runner can either be registered at an instance level or group level.
         The runner will be registered at a group level if the token used is from a group, or at an instance level if the token used is for the instance.
 
         **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/runners.html#register-a-new-runner)
 
+        ## Example Usage
+
+        ```python
+        import pulumi
+        import pulumi_gitlab as gitlab
+        import pulumi_local as local
+
+        # Basic GitLab Group Runner
+        my_group = gitlab.Group("myGroup", description="group that holds the runners")
+        basic_runner = gitlab.Runner("basicRunner", registration_token=my_group.runners_token)
+        # GitLab Runner that runs only tagged jobs
+        tagged_only = gitlab.Runner("taggedOnly",
+            registration_token=my_group.runners_token,
+            description="I only run tagged jobs",
+            run_untagged=False,
+            tag_lists=[
+                "tag_one",
+                "tag_two",
+            ])
+        # GitLab Runner that only runs on protected branches
+        protected = gitlab.Runner("protected",
+            registration_token=my_group.runners_token,
+            description="I only run protected jobs",
+            access_level="ref_protected")
+        # Generate a `config.toml` file that you can use to create a runner
+        # This is the typical workflow for this resource, using it to create an authentication_token which can then be used
+        # to generate the `config.toml` file to prevent re-registering the runner every time new hardware is created.
+        my_custom_group = gitlab.Group("myCustomGroup", description="group that holds the custom runners")
+        my_runner = gitlab.Runner("myRunner", registration_token=my_custom_group.runners_token)
+        # This creates a configuration for a local "shell" runner, but can be changed to generate whatever is needed.
+        # Place this configuration file on a server at `/etc/gitlab-runner/config.toml`, then run `gitlab-runner start`.
+        # See https://docs.gitlab.com/runner/configuration/advanced-configuration.html for more information.
+        config = local.File("config",
+            filename=f"{path['module']}/config.toml",
+            content=my_runner.authentication_token.apply(lambda authentication_token: f\"\"\"  concurrent = 1
+
+          [[runners]]
+            name = "Hello Terraform"
+            url = "https://example.gitlab.com/"
+            token = "{authentication_token}"
+            executor = "shell"
+            
+        \"\"\"))
+        ```
+
         ## Import
 
         A GitLab Runner can be imported using the runner's ID, eg
 
         ```sh
          $ pulumi import gitlab:index/runner:Runner this 1
         ```
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/service_custom_issue_tracker.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/service_custom_issue_tracker.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/service_emails_on_push.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/service_emails_on_push.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/service_external_wiki.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/service_external_wiki.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/service_github.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/service_github.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/service_jira.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/service_jira.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/service_microsoft_teams.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/service_microsoft_teams.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/service_pipelines_email.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/service_pipelines_email.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/service_slack.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/service_slack.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,14 +269,17 @@
 
     @property
     @pulumi.getter(name="notifyOnlyDefaultBranch")
     def notify_only_default_branch(self) -> Optional[pulumi.Input[bool]]:
         """
         This parameter has been replaced with `branches_to_be_notified`.
         """
+        warnings.warn("""use 'branches_to_be_notified' argument instead""", DeprecationWarning)
+        pulumi.log.warn("""notify_only_default_branch is deprecated: use 'branches_to_be_notified' argument instead""")
+
         return pulumi.get(self, "notify_only_default_branch")
 
     @notify_only_default_branch.setter
     def notify_only_default_branch(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "notify_only_default_branch", value)
 
     @property
@@ -640,14 +643,17 @@
 
     @property
     @pulumi.getter(name="notifyOnlyDefaultBranch")
     def notify_only_default_branch(self) -> Optional[pulumi.Input[bool]]:
         """
         This parameter has been replaced with `branches_to_be_notified`.
         """
+        warnings.warn("""use 'branches_to_be_notified' argument instead""", DeprecationWarning)
+        pulumi.log.warn("""notify_only_default_branch is deprecated: use 'branches_to_be_notified' argument instead""")
+
         return pulumi.get(self, "notify_only_default_branch")
 
     @notify_only_default_branch.setter
     def notify_only_default_branch(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "notify_only_default_branch", value)
 
     @property
@@ -1180,14 +1186,17 @@
 
     @property
     @pulumi.getter(name="notifyOnlyDefaultBranch")
     def notify_only_default_branch(self) -> pulumi.Output[bool]:
         """
         This parameter has been replaced with `branches_to_be_notified`.
         """
+        warnings.warn("""use 'branches_to_be_notified' argument instead""", DeprecationWarning)
+        pulumi.log.warn("""notify_only_default_branch is deprecated: use 'branches_to_be_notified' argument instead""")
+
         return pulumi.get(self, "notify_only_default_branch")
 
     @property
     @pulumi.getter(name="pipelineChannel")
     def pipeline_channel(self) -> pulumi.Output[Optional[str]]:
         """
         The name of the channel to receive pipeline events notifications.
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/system_hook.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/system_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/tag_protection.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/tag_protection.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,32 +4,38 @@
 
 import copy
 import warnings
 import pulumi
 import pulumi.runtime
 from typing import Any, Mapping, Optional, Sequence, Union, overload
 from . import _utilities
+from . import outputs
+from ._inputs import *
 
 __all__ = ['TagProtectionArgs', 'TagProtection']
 
 @pulumi.input_type
 class TagProtectionArgs:
     def __init__(__self__, *,
                  create_access_level: pulumi.Input[str],
                  project: pulumi.Input[str],
-                 tag: pulumi.Input[str]):
+                 tag: pulumi.Input[str],
+                 allowed_to_creates: Optional[pulumi.Input[Sequence[pulumi.Input['TagProtectionAllowedToCreateArgs']]]] = None):
         """
         The set of arguments for constructing a TagProtection resource.
         :param pulumi.Input[str] create_access_level: Access levels which are allowed to create. Valid values are: `no one`, `developer`, `maintainer`.
         :param pulumi.Input[str] project: The id of the project.
         :param pulumi.Input[str] tag: Name of the tag or wildcard.
+        :param pulumi.Input[Sequence[pulumi.Input['TagProtectionAllowedToCreateArgs']]] allowed_to_creates: User or group which are allowed to create.
         """
         pulumi.set(__self__, "create_access_level", create_access_level)
         pulumi.set(__self__, "project", project)
         pulumi.set(__self__, "tag", tag)
+        if allowed_to_creates is not None:
+            pulumi.set(__self__, "allowed_to_creates", allowed_to_creates)
 
     @property
     @pulumi.getter(name="createAccessLevel")
     def create_access_level(self) -> pulumi.Input[str]:
         """
         Access levels which are allowed to create. Valid values are: `no one`, `developer`, `maintainer`.
         """
@@ -59,35 +65,63 @@
         """
         return pulumi.get(self, "tag")
 
     @tag.setter
     def tag(self, value: pulumi.Input[str]):
         pulumi.set(self, "tag", value)
 
+    @property
+    @pulumi.getter(name="allowedToCreates")
+    def allowed_to_creates(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['TagProtectionAllowedToCreateArgs']]]]:
+        """
+        User or group which are allowed to create.
+        """
+        return pulumi.get(self, "allowed_to_creates")
+
+    @allowed_to_creates.setter
+    def allowed_to_creates(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['TagProtectionAllowedToCreateArgs']]]]):
+        pulumi.set(self, "allowed_to_creates", value)
+
 
 @pulumi.input_type
 class _TagProtectionState:
     def __init__(__self__, *,
+                 allowed_to_creates: Optional[pulumi.Input[Sequence[pulumi.Input['TagProtectionAllowedToCreateArgs']]]] = None,
                  create_access_level: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  tag: Optional[pulumi.Input[str]] = None):
         """
         Input properties used for looking up and filtering TagProtection resources.
+        :param pulumi.Input[Sequence[pulumi.Input['TagProtectionAllowedToCreateArgs']]] allowed_to_creates: User or group which are allowed to create.
         :param pulumi.Input[str] create_access_level: Access levels which are allowed to create. Valid values are: `no one`, `developer`, `maintainer`.
         :param pulumi.Input[str] project: The id of the project.
         :param pulumi.Input[str] tag: Name of the tag or wildcard.
         """
+        if allowed_to_creates is not None:
+            pulumi.set(__self__, "allowed_to_creates", allowed_to_creates)
         if create_access_level is not None:
             pulumi.set(__self__, "create_access_level", create_access_level)
         if project is not None:
             pulumi.set(__self__, "project", project)
         if tag is not None:
             pulumi.set(__self__, "tag", tag)
 
     @property
+    @pulumi.getter(name="allowedToCreates")
+    def allowed_to_creates(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['TagProtectionAllowedToCreateArgs']]]]:
+        """
+        User or group which are allowed to create.
+        """
+        return pulumi.get(self, "allowed_to_creates")
+
+    @allowed_to_creates.setter
+    def allowed_to_creates(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['TagProtectionAllowedToCreateArgs']]]]):
+        pulumi.set(self, "allowed_to_creates", value)
+
+    @property
     @pulumi.getter(name="createAccessLevel")
     def create_access_level(self) -> Optional[pulumi.Input[str]]:
         """
         Access levels which are allowed to create. Valid values are: `no one`, `developer`, `maintainer`.
         """
         return pulumi.get(self, "create_access_level")
 
@@ -121,30 +155,35 @@
 
 
 class TagProtection(pulumi.CustomResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 allowed_to_creates: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TagProtectionAllowedToCreateArgs']]]]] = None,
                  create_access_level: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  tag: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
-        The `TagProtection` resource allows to manage the lifecycle of a tag protection.
-
-        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/protected_tags.html)
-
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
         tag_protect = gitlab.TagProtection("tagProtect",
+            allowed_to_creates=[
+                gitlab.TagProtectionAllowedToCreateArgs(
+                    user_id=42,
+                ),
+                gitlab.TagProtectionAllowedToCreateArgs(
+                    group_id=43,
+                ),
+            ],
             create_access_level="developer",
             project="12345",
             tag="TagProtected")
         ```
 
         ## Import
 
@@ -152,36 +191,41 @@
 
         ```sh
          $ pulumi import gitlab:index/tagProtection:TagProtection example 123456789:v1.0.0
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TagProtectionAllowedToCreateArgs']]]] allowed_to_creates: User or group which are allowed to create.
         :param pulumi.Input[str] create_access_level: Access levels which are allowed to create. Valid values are: `no one`, `developer`, `maintainer`.
         :param pulumi.Input[str] project: The id of the project.
         :param pulumi.Input[str] tag: Name of the tag or wildcard.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: TagProtectionArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
-        The `TagProtection` resource allows to manage the lifecycle of a tag protection.
-
-        **Upstream API**: [GitLab REST API docs](https://docs.gitlab.com/ee/api/protected_tags.html)
-
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_gitlab as gitlab
 
         tag_protect = gitlab.TagProtection("tagProtect",
+            allowed_to_creates=[
+                gitlab.TagProtectionAllowedToCreateArgs(
+                    user_id=42,
+                ),
+                gitlab.TagProtectionAllowedToCreateArgs(
+                    group_id=43,
+                ),
+            ],
             create_access_level="developer",
             project="12345",
             tag="TagProtected")
         ```
 
         ## Import
 
@@ -202,26 +246,28 @@
             __self__._internal_init(resource_name, opts, **resource_args.__dict__)
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
+                 allowed_to_creates: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TagProtectionAllowedToCreateArgs']]]]] = None,
                  create_access_level: Optional[pulumi.Input[str]] = None,
                  project: Optional[pulumi.Input[str]] = None,
                  tag: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is None:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = TagProtectionArgs.__new__(TagProtectionArgs)
 
+            __props__.__dict__["allowed_to_creates"] = allowed_to_creates
             if create_access_level is None and not opts.urn:
                 raise TypeError("Missing required property 'create_access_level'")
             __props__.__dict__["create_access_level"] = create_access_level
             if project is None and not opts.urn:
                 raise TypeError("Missing required property 'project'")
             __props__.__dict__["project"] = project
             if tag is None and not opts.urn:
@@ -233,38 +279,49 @@
             __props__,
             opts)
 
     @staticmethod
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
+            allowed_to_creates: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TagProtectionAllowedToCreateArgs']]]]] = None,
             create_access_level: Optional[pulumi.Input[str]] = None,
             project: Optional[pulumi.Input[str]] = None,
             tag: Optional[pulumi.Input[str]] = None) -> 'TagProtection':
         """
         Get an existing TagProtection resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['TagProtectionAllowedToCreateArgs']]]] allowed_to_creates: User or group which are allowed to create.
         :param pulumi.Input[str] create_access_level: Access levels which are allowed to create. Valid values are: `no one`, `developer`, `maintainer`.
         :param pulumi.Input[str] project: The id of the project.
         :param pulumi.Input[str] tag: Name of the tag or wildcard.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _TagProtectionState.__new__(_TagProtectionState)
 
+        __props__.__dict__["allowed_to_creates"] = allowed_to_creates
         __props__.__dict__["create_access_level"] = create_access_level
         __props__.__dict__["project"] = project
         __props__.__dict__["tag"] = tag
         return TagProtection(resource_name, opts=opts, __props__=__props__)
 
     @property
+    @pulumi.getter(name="allowedToCreates")
+    def allowed_to_creates(self) -> pulumi.Output[Optional[Sequence['outputs.TagProtectionAllowedToCreate']]]:
+        """
+        User or group which are allowed to create.
+        """
+        return pulumi.get(self, "allowed_to_creates")
+
+    @property
     @pulumi.getter(name="createAccessLevel")
     def create_access_level(self) -> pulumi.Output[str]:
         """
         Access levels which are allowed to create. Valid values are: `no one`, `developer`, `maintainer`.
         """
         return pulumi.get(self, "create_access_level")
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/topic.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/topic.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,17 @@
 
     @property
     @pulumi.getter(name="softDestroy")
     def soft_destroy(self) -> Optional[pulumi.Input[bool]]:
         """
         Empty the topics fields instead of deleting it.
         """
+        warnings.warn("""GitLab 14.9 introduced the proper deletion of topics. This field is no longer needed.""", DeprecationWarning)
+        pulumi.log.warn("""soft_destroy is deprecated: GitLab 14.9 introduced the proper deletion of topics. This field is no longer needed.""")
+
         return pulumi.get(self, "soft_destroy")
 
     @soft_destroy.setter
     def soft_destroy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "soft_destroy", value)
 
     @property
@@ -218,14 +221,17 @@
 
     @property
     @pulumi.getter(name="softDestroy")
     def soft_destroy(self) -> Optional[pulumi.Input[bool]]:
         """
         Empty the topics fields instead of deleting it.
         """
+        warnings.warn("""GitLab 14.9 introduced the proper deletion of topics. This field is no longer needed.""", DeprecationWarning)
+        pulumi.log.warn("""soft_destroy is deprecated: GitLab 14.9 introduced the proper deletion of topics. This field is no longer needed.""")
+
         return pulumi.get(self, "soft_destroy")
 
     @soft_destroy.setter
     def soft_destroy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "soft_destroy", value)
 
     @property
@@ -437,14 +443,17 @@
 
     @property
     @pulumi.getter(name="softDestroy")
     def soft_destroy(self) -> pulumi.Output[Optional[bool]]:
         """
         Empty the topics fields instead of deleting it.
         """
+        warnings.warn("""GitLab 14.9 introduced the proper deletion of topics. This field is no longer needed.""", DeprecationWarning)
+        pulumi.log.warn("""soft_destroy is deprecated: GitLab 14.9 introduced the proper deletion of topics. This field is no longer needed.""")
+
         return pulumi.get(self, "soft_destroy")
 
     @property
     @pulumi.getter
     def title(self) -> pulumi.Output[Optional[str]]:
         """
         The topic's description. Requires at least GitLab 15.0 for which it's a required argument.
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/user.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/user_custom_attribute.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/user_custom_attribute.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/user_gpg_key.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/user_gpg_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab/user_ssh_key.py` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab/user_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab.egg-info/PKG-INFO` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-gitlab
-Version: 6.1.0a1687929913
+Version: 6.1.0a1688977388
 Summary: A Pulumi package for creating and managing GitLab resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-gitlab
 Keywords: pulumi gitlab
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_gitlab-6.1.0a1687929913/pulumi_gitlab.egg-info/SOURCES.txt` & `pulumi_gitlab-6.1.0a1688977388/pulumi_gitlab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_gitlab-6.1.0a1687929913/setup.py` & `pulumi_gitlab-6.1.0a1688977388/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.1.0a1687929913"
-PLUGIN_VERSION = "6.1.0-alpha.1687929913+7611ebce"
+VERSION = "6.1.0a1688977388"
+PLUGIN_VERSION = "6.1.0-alpha.1688977388+74bb1cc3"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'gitlab', PLUGIN_VERSION])
         except OSError as error:
```

