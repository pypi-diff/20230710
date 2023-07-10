# Comparing `tmp/pulumi_okta-4.1.0a1687800548.tar.gz` & `tmp/pulumi_okta-4.1.0a1689006772.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_okta-4.1.0a1687800548.tar", last modified: Mon Jun 26 17:34:11 2023, max compression
+gzip compressed data, was "pulumi_okta-4.1.0a1689006772.tar", last modified: Mon Jul 10 16:38:34 2023, max compression
```

## Comparing `pulumi_okta-4.1.0a1687800548.tar` & `pulumi_okta-4.1.0a1689006772.tar`

### file list

```diff
@@ -1,192 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.892634 pulumi_okta-4.1.0a1687800548/
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-26 17:34:11.892634 pulumi_okta-4.1.0a1687800548/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.880634 pulumi_okta-4.1.0a1687800548/pulumi_okta/
--rw-r--r--   0 runner    (1001) docker     (123)    19391 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20901 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    21364 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/admin_role_custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/admin_role_custom_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/admin_role_targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.884634 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    63359 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/auto_login.py
--rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    39876 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/bookmark.py
--rw-r--r--   0 runner    (1001) docker     (123)    10317 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/get_app.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    17697 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/get_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)    31761 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    14665 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/group_assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)   139451 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/o_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/o_auth_redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)   137444 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    72331 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/secure_password_store.py
--rw-r--r--   0 runner    (1001) docker     (123)    58966 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/swa.py
--rw-r--r--   0 runner    (1001) docker     (123)    66578 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/three_field.py
--rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app/user.py
--rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app_oauth_api_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app_saml_app_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    65611 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app_shared_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    81293 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app_signon_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    23561 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app_user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    50905 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/app_user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.884634 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/get_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     5306 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/get_server_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/get_server_scopes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23427 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server.py
--rw-r--r--   0 runner    (1001) docker     (123)    24590 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    46621 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server_policy_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)    46368 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server_policy_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server_scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    19984 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth_server_claim_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    23207 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/auth_server_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    46170 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/behaviour.py
--rw-r--r--   0 runner    (1001) docker     (123)    16966 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/brand.py
--rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/captcha.py
--rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/captcha_org_wide_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.884634 pulumi_okta-4.1.0a1687800548/pulumi_okta/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/domain_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)    37986 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/email_customization.py
--rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/email_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     6853 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/email_sender_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/event_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/event_hook_verification.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.884634 pulumi_okta-4.1.0a1687800548/pulumi_okta/factor/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/factor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/factor/factor.py
--rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/factor_totp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_app_group_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_app_signon_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3204 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_app_user_assignments.py
--rw-r--r--   0 runner    (1001) docker     (123)     7092 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_auth_server_claim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_auth_server_claims.py
--rw-r--r--   0 runner    (1001) docker     (123)     9027 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_authenticator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_behaviour.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_behaviours.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_brand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_brands.py
--rw-r--r--   0 runner    (1001) docker     (123)     6722 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_email_customization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4540 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_email_customizations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_network_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)     5603 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    11110 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_themes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3810 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_trusted_origins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/get_user_security_questions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.888635 pulumi_okta-4.1.0a1687800548/pulumi_okta/group/
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/group/get_everyone_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/group/get_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/group/group.py
--rw-r--r--   0 runner    (1001) docker     (123)    23973 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/group/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/group/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)    47214 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/group_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.888635 pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7608 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/get_metadata_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    11448 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/get_oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8836 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/get_saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    17510 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/get_social.py
--rw-r--r--   0 runner    (1001) docker     (123)    87339 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/oidc.py
--rw-r--r--   0 runner    (1001) docker     (123)    83358 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/saml.py
--rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/saml_key.py
--rw-r--r--   0 runner    (1001) docker     (123)    72824 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/social.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.888635 pulumi_okta-4.1.0a1687800548/pulumi_okta/index/
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/index/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/index/email_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/index/email_domain_verification.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/index/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/index/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.888635 pulumi_okta-4.1.0a1687800548/pulumi_okta/inline/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/inline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/inline/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/inline/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/inline/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18793 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/link_definition.py
--rw-r--r--   0 runner    (1001) docker     (123)    14673 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/link_value.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.888635 pulumi_okta-4.1.0a1687800548/pulumi_okta/network/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26167 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/network/zone.py
--rw-r--r--   0 runner    (1001) docker     (123)    35387 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/org_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/org_support.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.892634 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/get_default_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/get_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    69146 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/mfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    79587 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/password.py
--rw-r--r--   0 runner    (1001) docker     (123)    48541 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/rule_idp_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)    30922 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/rule_mfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    30689 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/rule_password.py
--rw-r--r--   0 runner    (1001) docker     (123)    66350 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/rule_signon.py
--rw-r--r--   0 runner    (1001) docker     (123)    13691 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/signon.py
--rw-r--r--   0 runner    (1001) docker     (123)    65319 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy_mfa_default.py
--rw-r--r--   0 runner    (1001) docker     (123)    71401 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy_password_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy_profile_enrollment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy_profile_enrollment_apps.py
--rw-r--r--   0 runner    (1001) docker     (123)    31670 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/policy_rule_profile_enrollment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.892634 pulumi_okta-4.1.0a1687800548/pulumi_okta/profile/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/profile/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    22298 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/profile/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/profile/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23808 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/rate_limiting.py
--rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/resource_set.py
--rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/role_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/security_notification_emails.py
--rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/template_sms.py
--rw-r--r--   0 runner    (1001) docker     (123)    42242 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/theme.py
--rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/threat_insight_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.892634 pulumi_okta-4.1.0a1687800548/pulumi_okta/trustedorigin/
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/trustedorigin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/trustedorigin/origin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.892634 pulumi_okta-4.1.0a1687800548/pulumi_okta/user/
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24937 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     2849 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user/get_user_profile_mapping_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3765 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user/get_user_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     9551 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user/get_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    22177 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    98382 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user/user_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user_admin_roles.py
--rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user_base_schema_property.py
--rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user_factor_question.py
--rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user_group_memberships.py
--rw-r--r--   0 runner    (1001) docker     (123)    51704 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta/user_schema_property.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-26 17:34:11.880634 pulumi_okta-4.1.0a1687800548/pulumi_okta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5572 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/pulumi_okta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-26 17:34:11.892634 pulumi_okta-4.1.0a1687800548/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-26 17:34:11.000000 pulumi_okta-4.1.0a1687800548/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:38:34.347193 pulumi_okta-4.1.0a1689006772/
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-10 16:38:34.347193 pulumi_okta-4.1.0a1689006772/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:38:34.339193 pulumi_okta-4.1.0a1689006772/pulumi_okta/
+-rw-r--r--   0 runner    (1001) docker     (123)    19391 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20927 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21364 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/admin_role_custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11761 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/admin_role_custom_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15334 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/admin_role_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:38:34.339193 pulumi_okta-4.1.0a1689006772/pulumi_okta/app/
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14870 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63359 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app/auto_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36563 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app/basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39876 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app/bookmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10318 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app/get_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app/get_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32302 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14665 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app/group_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)   139451 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app/o_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9341 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app/o_auth_post_logout_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app/o_auth_redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14858 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)   137230 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app/saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72331 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app/secure_password_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58966 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app/swa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66578 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app/three_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18034 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12536 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10964 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app_oauth_api_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app_saml_app_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65611 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app_shared_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9532 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81293 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app_signon_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23561 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app_user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50905 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/app_user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:38:34.343193 pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/get_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/get_server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3656 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/get_server_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23427 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24590 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17542 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/server_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46621 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/server_policy_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46368 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/server_policy_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20705 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/server_scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19984 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/auth_server_claim_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23945 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/auth_server_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46170 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18251 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12840 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/captcha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11158 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/captcha_org_wide_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:38:34.343193 pulumi_okta-4.1.0a1689006772/pulumi_okta/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4218 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12369 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15106 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/domain_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39997 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12867 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/email_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/email_sender_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17972 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/event_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7884 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/event_hook_verification.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:38:34.343193 pulumi_okta-4.1.0a1689006772/pulumi_okta/factor/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/factor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/factor/factor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19375 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/factor_totp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_app_group_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_app_signon_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3234 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_app_user_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_auth_server_claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_auth_server_claims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9207 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_authenticator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_behaviour.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3285 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_behaviours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_brand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_brands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6857 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_email_customization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_email_customizations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5389 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_network_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_themes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_trusted_origins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4161 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/get_user_security_questions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:38:34.343193 pulumi_okta-4.1.0a1689006772/pulumi_okta/group/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/group/get_everyone_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6871 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/group/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/group/get_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15323 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/group/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23973 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/group/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21025 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/group/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13237 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47214 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/group_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:38:34.343193 pulumi_okta-4.1.0a1689006772/pulumi_okta/idp/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/idp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7758 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/idp/get_metadata_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11718 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/idp/get_oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/idp/get_saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17915 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/idp/get_social.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87339 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/idp/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    83358 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/idp/saml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11806 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/idp/saml_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72824 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/idp/social.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:38:34.343193 pulumi_okta-4.1.0a1689006772/pulumi_okta/index/
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/index/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15177 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/index/email_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7129 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/index/email_domain_verification.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6554 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/index/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/index/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:38:34.343193 pulumi_okta-4.1.0a1689006772/pulumi_okta/inline/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/inline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/inline/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18690 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/inline/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/inline/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18793 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/link_definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14673 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/link_value.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:38:34.343193 pulumi_okta-4.1.0a1689006772/pulumi_okta/network/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26167 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/network/zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35387 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/org_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8652 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/org_support.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33089 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:38:34.347193 pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15700 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/get_default_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4071 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/get_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69146 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/mfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14772 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79587 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48541 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/rule_idp_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30922 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/rule_mfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30689 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/rule_password.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66350 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/rule_signon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13691 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/signon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65319 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/policy_mfa_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71401 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/policy_password_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/policy_profile_enrollment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/policy_profile_enrollment_apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31670 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/policy_rule_profile_enrollment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:38:34.347193 pulumi_okta-4.1.0a1689006772/pulumi_okta/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/profile/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22298 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/profile/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/profile/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23808 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13786 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/rate_limiting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11747 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/resource_set.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21062 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/role_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21408 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/security_notification_emails.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11510 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/template_sms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42242 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14794 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/threat_insight_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:38:34.347193 pulumi_okta-4.1.0a1689006772/pulumi_okta/trustedorigin/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/trustedorigin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/trustedorigin/origin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:38:34.347193 pulumi_okta-4.1.0a1689006772/pulumi_okta/user/
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9652 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/user/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25582 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/user/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/user/get_user_profile_mapping_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/user/get_user_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9671 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/user/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22177 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/user/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99207 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/user/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9913 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/user/user_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14009 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/user_admin_roles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22925 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/user_base_schema_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14108 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/user_factor_question.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8972 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/user_group_memberships.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51704 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta/user_schema_property.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 16:38:34.339193 pulumi_okta-4.1.0a1689006772/pulumi_okta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3265 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/pulumi_okta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 16:38:34.347193 pulumi_okta-4.1.0a1689006772/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-10 16:38:34.000000 pulumi_okta-4.1.0a1689006772/setup.py
```

### Comparing `pulumi_okta-4.1.0a1687800548/PKG-INFO` & `pulumi_okta-4.1.0a1689006772/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_okta
-Version: 4.1.0a1687800548
+Version: 4.1.0a1689006772
 Summary: A Pulumi package for creating and managing okta resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi okta
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_okta-4.1.0a1687800548/README.md` & `pulumi_okta-4.1.0a1689006772/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/__init__.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/_inputs.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,30 +83,30 @@
 @pulumi.input_type
 class AppSignonPolicyRulePlatformIncludeArgs:
     def __init__(__self__, *,
                  os_expression: Optional[pulumi.Input[str]] = None,
                  os_type: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None):
         """
-        :param pulumi.Input[str] os_expression: Only available when using `os_type = "OTHER"`
+        :param pulumi.Input[str] os_expression: Only available and required when using `os_type = "OTHER"`
         :param pulumi.Input[str] os_type: One of: `"ANY"`, `"IOS"`, `"WINDOWS"`, `"ANDROID"`, `"OTHER"`, `"OSX"`, `"MACOS"`
         :param pulumi.Input[str] type: The Verification Method type. It can be set to `"ASSURANCE"`. Default is `"ASSURANCE"`.
         """
         if os_expression is not None:
             pulumi.set(__self__, "os_expression", os_expression)
         if os_type is not None:
             pulumi.set(__self__, "os_type", os_type)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter(name="osExpression")
     def os_expression(self) -> Optional[pulumi.Input[str]]:
         """
-        Only available when using `os_type = "OTHER"`
+        Only available and required when using `os_type = "OTHER"`
         """
         return pulumi.get(self, "os_expression")
 
     @os_expression.setter
     def os_expression(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "os_expression", value)
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/_utilities.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/admin_role_custom.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/admin_role_custom.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/admin_role_custom_assignments.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/admin_role_custom_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/admin_role_targets.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/admin_role_targets.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/__init__.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/_inputs.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/auto_login.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app/auto_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/basic_auth.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app/basic_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/bookmark.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app/bookmark.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/get_app.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app/get_app.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,14 @@
     """
     def __init__(__self__, active_only=None, groups=None, id=None, label=None, label_prefix=None, links=None, name=None, skip_groups=None, skip_users=None, status=None, users=None):
         if active_only and not isinstance(active_only, bool):
             raise TypeError("Expected argument 'active_only' to be a bool")
         pulumi.set(__self__, "active_only", active_only)
         if groups and not isinstance(groups, list):
             raise TypeError("Expected argument 'groups' to be a list")
-        if groups is not None:
-            warnings.warn("""The `groups` field is now deprecated for the data source `okta_app`, please replace all uses of this with: `okta_app_group_assignments`""", DeprecationWarning)
-            pulumi.log.warn("""groups is deprecated: The `groups` field is now deprecated for the data source `okta_app`, please replace all uses of this with: `okta_app_group_assignments`""")
-
         pulumi.set(__self__, "groups", groups)
         if id and not isinstance(id, str):
             raise TypeError("Expected argument 'id' to be a str")
         pulumi.set(__self__, "id", id)
         if label and not isinstance(label, str):
             raise TypeError("Expected argument 'label' to be a str")
         pulumi.set(__self__, "label", label)
@@ -45,45 +41,36 @@
             raise TypeError("Expected argument 'links' to be a str")
         pulumi.set(__self__, "links", links)
         if name and not isinstance(name, str):
             raise TypeError("Expected argument 'name' to be a str")
         pulumi.set(__self__, "name", name)
         if skip_groups and not isinstance(skip_groups, bool):
             raise TypeError("Expected argument 'skip_groups' to be a bool")
-        if skip_groups is not None:
-            warnings.warn("""Because groups has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
-            pulumi.log.warn("""skip_groups is deprecated: Because groups has been removed, this attribute is a no op and will be removed""")
-
         pulumi.set(__self__, "skip_groups", skip_groups)
         if skip_users and not isinstance(skip_users, bool):
             raise TypeError("Expected argument 'skip_users' to be a bool")
-        if skip_users is not None:
-            warnings.warn("""Because users has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
-            pulumi.log.warn("""skip_users is deprecated: Because users has been removed, this attribute is a no op and will be removed""")
-
         pulumi.set(__self__, "skip_users", skip_users)
         if status and not isinstance(status, str):
             raise TypeError("Expected argument 'status' to be a str")
         pulumi.set(__self__, "status", status)
         if users and not isinstance(users, list):
             raise TypeError("Expected argument 'users' to be a list")
-        if users is not None:
-            warnings.warn("""The `users` field is now deprecated for the data source `okta_app`, please replace all uses of this with: `okta_app_user_assignments`""", DeprecationWarning)
-            pulumi.log.warn("""users is deprecated: The `users` field is now deprecated for the data source `okta_app`, please replace all uses of this with: `okta_app_user_assignments`""")
-
         pulumi.set(__self__, "users", users)
 
     @property
     @pulumi.getter(name="activeOnly")
     def active_only(self) -> Optional[bool]:
         return pulumi.get(self, "active_only")
 
     @property
     @pulumi.getter
     def groups(self) -> Sequence[str]:
+        warnings.warn("""The `groups` field is now deprecated for the data source `okta_app`, please replace all uses of this with: `okta_app_group_assignments`""", DeprecationWarning)
+        pulumi.log.warn("""groups is deprecated: The `groups` field is now deprecated for the data source `okta_app`, please replace all uses of this with: `okta_app_group_assignments`""")
+
         return pulumi.get(self, "groups")
 
     @property
     @pulumi.getter
     def id(self) -> Optional[str]:
         """
         Application ID.
@@ -118,32 +105,41 @@
         Application name.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter(name="skipGroups")
     def skip_groups(self) -> Optional[bool]:
+        warnings.warn("""Because groups has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+        pulumi.log.warn("""skip_groups is deprecated: Because groups has been removed, this attribute is a no op and will be removed""")
+
         return pulumi.get(self, "skip_groups")
 
     @property
     @pulumi.getter(name="skipUsers")
     def skip_users(self) -> Optional[bool]:
+        warnings.warn("""Because users has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+        pulumi.log.warn("""skip_users is deprecated: Because users has been removed, this attribute is a no op and will be removed""")
+
         return pulumi.get(self, "skip_users")
 
     @property
     @pulumi.getter
     def status(self) -> str:
         """
         Application status.
         """
         return pulumi.get(self, "status")
 
     @property
     @pulumi.getter
     def users(self) -> Sequence[str]:
+        warnings.warn("""The `users` field is now deprecated for the data source `okta_app`, please replace all uses of this with: `okta_app_user_assignments`""", DeprecationWarning)
+        pulumi.log.warn("""users is deprecated: The `users` field is now deprecated for the data source `okta_app`, please replace all uses of this with: `okta_app_user_assignments`""")
+
         return pulumi.get(self, "users")
 
 
 class AwaitableGetAppResult(GetAppResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -199,25 +195,25 @@
     __args__['labelPrefix'] = label_prefix
     __args__['skipGroups'] = skip_groups
     __args__['skipUsers'] = skip_users
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:app/getApp:getApp', __args__, opts=opts, typ=GetAppResult).value
 
     return AwaitableGetAppResult(
-        active_only=__ret__.active_only,
-        groups=__ret__.groups,
-        id=__ret__.id,
-        label=__ret__.label,
-        label_prefix=__ret__.label_prefix,
-        links=__ret__.links,
-        name=__ret__.name,
-        skip_groups=__ret__.skip_groups,
-        skip_users=__ret__.skip_users,
-        status=__ret__.status,
-        users=__ret__.users)
+        active_only=pulumi.get(__ret__, 'active_only'),
+        groups=pulumi.get(__ret__, 'groups'),
+        id=pulumi.get(__ret__, 'id'),
+        label=pulumi.get(__ret__, 'label'),
+        label_prefix=pulumi.get(__ret__, 'label_prefix'),
+        links=pulumi.get(__ret__, 'links'),
+        name=pulumi.get(__ret__, 'name'),
+        skip_groups=pulumi.get(__ret__, 'skip_groups'),
+        skip_users=pulumi.get(__ret__, 'skip_users'),
+        status=pulumi.get(__ret__, 'status'),
+        users=pulumi.get(__ret__, 'users'))
 
 
 @_utilities.lift_output_func(get_app)
 def get_app_output(active_only: Optional[pulumi.Input[Optional[bool]]] = None,
                    id: Optional[pulumi.Input[Optional[str]]] = None,
                    label: Optional[pulumi.Input[Optional[str]]] = None,
                    label_prefix: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/get_metadata_saml.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app/get_metadata_saml.py`

 * *Files 8% similar despite different names*

```diff
@@ -157,23 +157,23 @@
     __args__ = dict()
     __args__['appId'] = app_id
     __args__['keyId'] = key_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:app/getMetadataSaml:getMetadataSaml', __args__, opts=opts, typ=GetMetadataSamlResult).value
 
     return AwaitableGetMetadataSamlResult(
-        app_id=__ret__.app_id,
-        certificate=__ret__.certificate,
-        entity_id=__ret__.entity_id,
-        http_post_binding=__ret__.http_post_binding,
-        http_redirect_binding=__ret__.http_redirect_binding,
-        id=__ret__.id,
-        key_id=__ret__.key_id,
-        metadata=__ret__.metadata,
-        want_authn_requests_signed=__ret__.want_authn_requests_signed)
+        app_id=pulumi.get(__ret__, 'app_id'),
+        certificate=pulumi.get(__ret__, 'certificate'),
+        entity_id=pulumi.get(__ret__, 'entity_id'),
+        http_post_binding=pulumi.get(__ret__, 'http_post_binding'),
+        http_redirect_binding=pulumi.get(__ret__, 'http_redirect_binding'),
+        id=pulumi.get(__ret__, 'id'),
+        key_id=pulumi.get(__ret__, 'key_id'),
+        metadata=pulumi.get(__ret__, 'metadata'),
+        want_authn_requests_signed=pulumi.get(__ret__, 'want_authn_requests_signed'))
 
 
 @_utilities.lift_output_func(get_metadata_saml)
 def get_metadata_saml_output(app_id: Optional[pulumi.Input[str]] = None,
                              key_id: Optional[pulumi.Input[Optional[str]]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMetadataSamlResult]:
     """
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/get_oauth.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app/get_oauth.py`

 * *Files 12% similar despite different names*

```diff
@@ -83,25 +83,17 @@
             raise TypeError("Expected argument 'redirect_uris' to be a list")
         pulumi.set(__self__, "redirect_uris", redirect_uris)
         if response_types and not isinstance(response_types, list):
             raise TypeError("Expected argument 'response_types' to be a list")
         pulumi.set(__self__, "response_types", response_types)
         if skip_groups and not isinstance(skip_groups, bool):
             raise TypeError("Expected argument 'skip_groups' to be a bool")
-        if skip_groups is not None:
-            warnings.warn("""Because groups has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
-            pulumi.log.warn("""skip_groups is deprecated: Because groups has been removed, this attribute is a no op and will be removed""")
-
         pulumi.set(__self__, "skip_groups", skip_groups)
         if skip_users and not isinstance(skip_users, bool):
             raise TypeError("Expected argument 'skip_users' to be a bool")
-        if skip_users is not None:
-            warnings.warn("""Because users has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
-            pulumi.log.warn("""skip_users is deprecated: Because users has been removed, this attribute is a no op and will be removed""")
-
         pulumi.set(__self__, "skip_users", skip_users)
         if status and not isinstance(status, str):
             raise TypeError("Expected argument 'status' to be a str")
         pulumi.set(__self__, "status", status)
         if type and not isinstance(type, str):
             raise TypeError("Expected argument 'type' to be a str")
         pulumi.set(__self__, "type", type)
@@ -270,19 +262,25 @@
         List of OAuth 2.0 response type strings.
         """
         return pulumi.get(self, "response_types")
 
     @property
     @pulumi.getter(name="skipGroups")
     def skip_groups(self) -> Optional[bool]:
+        warnings.warn("""Because groups has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+        pulumi.log.warn("""skip_groups is deprecated: Because groups has been removed, this attribute is a no op and will be removed""")
+
         return pulumi.get(self, "skip_groups")
 
     @property
     @pulumi.getter(name="skipUsers")
     def skip_users(self) -> Optional[bool]:
+        warnings.warn("""Because users has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+        pulumi.log.warn("""skip_users is deprecated: Because users has been removed, this attribute is a no op and will be removed""")
+
         return pulumi.get(self, "skip_users")
 
     @property
     @pulumi.getter
     def status(self) -> str:
         """
         Status of application.
@@ -376,40 +374,40 @@
     __args__['labelPrefix'] = label_prefix
     __args__['skipGroups'] = skip_groups
     __args__['skipUsers'] = skip_users
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:app/getOauth:getOauth', __args__, opts=opts, typ=GetOauthResult).value
 
     return AwaitableGetOauthResult(
-        active_only=__ret__.active_only,
-        auto_submit_toolbar=__ret__.auto_submit_toolbar,
-        client_id=__ret__.client_id,
-        client_secret=__ret__.client_secret,
-        client_uri=__ret__.client_uri,
-        grant_types=__ret__.grant_types,
-        hide_ios=__ret__.hide_ios,
-        hide_web=__ret__.hide_web,
-        id=__ret__.id,
-        label=__ret__.label,
-        label_prefix=__ret__.label_prefix,
-        links=__ret__.links,
-        login_mode=__ret__.login_mode,
-        login_scopes=__ret__.login_scopes,
-        login_uri=__ret__.login_uri,
-        logo_uri=__ret__.logo_uri,
-        name=__ret__.name,
-        policy_uri=__ret__.policy_uri,
-        post_logout_redirect_uris=__ret__.post_logout_redirect_uris,
-        redirect_uris=__ret__.redirect_uris,
-        response_types=__ret__.response_types,
-        skip_groups=__ret__.skip_groups,
-        skip_users=__ret__.skip_users,
-        status=__ret__.status,
-        type=__ret__.type,
-        wildcard_redirect=__ret__.wildcard_redirect)
+        active_only=pulumi.get(__ret__, 'active_only'),
+        auto_submit_toolbar=pulumi.get(__ret__, 'auto_submit_toolbar'),
+        client_id=pulumi.get(__ret__, 'client_id'),
+        client_secret=pulumi.get(__ret__, 'client_secret'),
+        client_uri=pulumi.get(__ret__, 'client_uri'),
+        grant_types=pulumi.get(__ret__, 'grant_types'),
+        hide_ios=pulumi.get(__ret__, 'hide_ios'),
+        hide_web=pulumi.get(__ret__, 'hide_web'),
+        id=pulumi.get(__ret__, 'id'),
+        label=pulumi.get(__ret__, 'label'),
+        label_prefix=pulumi.get(__ret__, 'label_prefix'),
+        links=pulumi.get(__ret__, 'links'),
+        login_mode=pulumi.get(__ret__, 'login_mode'),
+        login_scopes=pulumi.get(__ret__, 'login_scopes'),
+        login_uri=pulumi.get(__ret__, 'login_uri'),
+        logo_uri=pulumi.get(__ret__, 'logo_uri'),
+        name=pulumi.get(__ret__, 'name'),
+        policy_uri=pulumi.get(__ret__, 'policy_uri'),
+        post_logout_redirect_uris=pulumi.get(__ret__, 'post_logout_redirect_uris'),
+        redirect_uris=pulumi.get(__ret__, 'redirect_uris'),
+        response_types=pulumi.get(__ret__, 'response_types'),
+        skip_groups=pulumi.get(__ret__, 'skip_groups'),
+        skip_users=pulumi.get(__ret__, 'skip_users'),
+        status=pulumi.get(__ret__, 'status'),
+        type=pulumi.get(__ret__, 'type'),
+        wildcard_redirect=pulumi.get(__ret__, 'wildcard_redirect'))
 
 
 @_utilities.lift_output_func(get_oauth)
 def get_oauth_output(active_only: Optional[pulumi.Input[Optional[bool]]] = None,
                      id: Optional[pulumi.Input[Optional[str]]] = None,
                      label: Optional[pulumi.Input[Optional[str]]] = None,
                      label_prefix: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/get_saml.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app/get_saml.py`

 * *Files 11% similar despite different names*

```diff
@@ -66,18 +66,14 @@
             raise TypeError("Expected argument 'digest_algorithm' to be a str")
         pulumi.set(__self__, "digest_algorithm", digest_algorithm)
         if features and not isinstance(features, list):
             raise TypeError("Expected argument 'features' to be a list")
         pulumi.set(__self__, "features", features)
         if groups and not isinstance(groups, list):
             raise TypeError("Expected argument 'groups' to be a list")
-        if groups is not None:
-            warnings.warn("""The `groups` field is now deprecated for the data source `okta_app_saml`, please replace all uses of this with: `okta_app_group_assignments`""", DeprecationWarning)
-            pulumi.log.warn("""groups is deprecated: The `groups` field is now deprecated for the data source `okta_app_saml`, please replace all uses of this with: `okta_app_group_assignments`""")
-
         pulumi.set(__self__, "groups", groups)
         if hide_ios and not isinstance(hide_ios, bool):
             raise TypeError("Expected argument 'hide_ios' to be a bool")
         pulumi.set(__self__, "hide_ios", hide_ios)
         if hide_web and not isinstance(hide_web, bool):
             raise TypeError("Expected argument 'hide_web' to be a bool")
         pulumi.set(__self__, "hide_web", hide_web)
@@ -130,25 +126,17 @@
             raise TypeError("Expected argument 'single_logout_issuer' to be a str")
         pulumi.set(__self__, "single_logout_issuer", single_logout_issuer)
         if single_logout_url and not isinstance(single_logout_url, str):
             raise TypeError("Expected argument 'single_logout_url' to be a str")
         pulumi.set(__self__, "single_logout_url", single_logout_url)
         if skip_groups and not isinstance(skip_groups, bool):
             raise TypeError("Expected argument 'skip_groups' to be a bool")
-        if skip_groups is not None:
-            warnings.warn("""Because groups has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
-            pulumi.log.warn("""skip_groups is deprecated: Because groups has been removed, this attribute is a no op and will be removed""")
-
         pulumi.set(__self__, "skip_groups", skip_groups)
         if skip_users and not isinstance(skip_users, bool):
             raise TypeError("Expected argument 'skip_users' to be a bool")
-        if skip_users is not None:
-            warnings.warn("""Because users has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
-            pulumi.log.warn("""skip_users is deprecated: Because users has been removed, this attribute is a no op and will be removed""")
-
         pulumi.set(__self__, "skip_users", skip_users)
         if sp_issuer and not isinstance(sp_issuer, str):
             raise TypeError("Expected argument 'sp_issuer' to be a str")
         pulumi.set(__self__, "sp_issuer", sp_issuer)
         if sso_url and not isinstance(sso_url, str):
             raise TypeError("Expected argument 'sso_url' to be a str")
         pulumi.set(__self__, "sso_url", sso_url)
@@ -171,18 +159,14 @@
             raise TypeError("Expected argument 'user_name_template_suffix' to be a str")
         pulumi.set(__self__, "user_name_template_suffix", user_name_template_suffix)
         if user_name_template_type and not isinstance(user_name_template_type, str):
             raise TypeError("Expected argument 'user_name_template_type' to be a str")
         pulumi.set(__self__, "user_name_template_type", user_name_template_type)
         if users and not isinstance(users, list):
             raise TypeError("Expected argument 'users' to be a list")
-        if users is not None:
-            warnings.warn("""The `users` field is now deprecated for the data source `okta_app_saml`, please replace all uses of this with: `okta_app_user_assignments`""", DeprecationWarning)
-            pulumi.log.warn("""users is deprecated: The `users` field is now deprecated for the data source `okta_app_saml`, please replace all uses of this with: `okta_app_user_assignments`""")
-
         pulumi.set(__self__, "users", users)
 
     @property
     @pulumi.getter(name="accessibilityErrorRedirectUrl")
     def accessibility_error_redirect_url(self) -> str:
         """
         Custom error page URL.
@@ -300,14 +284,17 @@
 
     @property
     @pulumi.getter
     def groups(self) -> Sequence[str]:
         """
         List of groups IDs assigned to the application.
         """
+        warnings.warn("""The `groups` field is now deprecated for the data source `okta_app_saml`, please replace all uses of this with: `okta_app_group_assignments`""", DeprecationWarning)
+        pulumi.log.warn("""groups is deprecated: The `groups` field is now deprecated for the data source `okta_app_saml`, please replace all uses of this with: `okta_app_group_assignments`""")
+
         return pulumi.get(self, "groups")
 
     @property
     @pulumi.getter(name="hideIos")
     def hide_ios(self) -> bool:
         """
         Do not display application icon on mobile app.
@@ -454,19 +441,25 @@
         The location where the logout response is sent.
         """
         return pulumi.get(self, "single_logout_url")
 
     @property
     @pulumi.getter(name="skipGroups")
     def skip_groups(self) -> Optional[bool]:
+        warnings.warn("""Because groups has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+        pulumi.log.warn("""skip_groups is deprecated: Because groups has been removed, this attribute is a no op and will be removed""")
+
         return pulumi.get(self, "skip_groups")
 
     @property
     @pulumi.getter(name="skipUsers")
     def skip_users(self) -> Optional[bool]:
+        warnings.warn("""Because users has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+        pulumi.log.warn("""skip_users is deprecated: Because users has been removed, this attribute is a no op and will be removed""")
+
         return pulumi.get(self, "skip_users")
 
     @property
     @pulumi.getter(name="spIssuer")
     def sp_issuer(self) -> str:
         """
         SAML service provider issuer.
@@ -536,14 +529,17 @@
         Username template type.
         """
         return pulumi.get(self, "user_name_template_type")
 
     @property
     @pulumi.getter
     def users(self) -> Sequence[str]:
+        warnings.warn("""The `users` field is now deprecated for the data source `okta_app_saml`, please replace all uses of this with: `okta_app_user_assignments`""", DeprecationWarning)
+        pulumi.log.warn("""users is deprecated: The `users` field is now deprecated for the data source `okta_app_saml`, please replace all uses of this with: `okta_app_user_assignments`""")
+
         return pulumi.get(self, "users")
 
 
 class AwaitableGetSamlResult(GetSamlResult):
     # pylint: disable=using-constant-test
     def __await__(self):
         if False:
@@ -636,61 +632,61 @@
     __args__['requestCompressed'] = request_compressed
     __args__['skipGroups'] = skip_groups
     __args__['skipUsers'] = skip_users
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:app/getSaml:getSaml', __args__, opts=opts, typ=GetSamlResult).value
 
     return AwaitableGetSamlResult(
-        accessibility_error_redirect_url=__ret__.accessibility_error_redirect_url,
-        accessibility_login_redirect_url=__ret__.accessibility_login_redirect_url,
-        accessibility_self_service=__ret__.accessibility_self_service,
-        acs_endpoints=__ret__.acs_endpoints,
-        active_only=__ret__.active_only,
-        app_settings_json=__ret__.app_settings_json,
-        assertion_signed=__ret__.assertion_signed,
-        attribute_statements=__ret__.attribute_statements,
-        audience=__ret__.audience,
-        authn_context_class_ref=__ret__.authn_context_class_ref,
-        auto_submit_toolbar=__ret__.auto_submit_toolbar,
-        default_relay_state=__ret__.default_relay_state,
-        destination=__ret__.destination,
-        digest_algorithm=__ret__.digest_algorithm,
-        features=__ret__.features,
-        groups=__ret__.groups,
-        hide_ios=__ret__.hide_ios,
-        hide_web=__ret__.hide_web,
-        honor_force_authn=__ret__.honor_force_authn,
-        id=__ret__.id,
-        idp_issuer=__ret__.idp_issuer,
-        inline_hook_id=__ret__.inline_hook_id,
-        key_id=__ret__.key_id,
-        label=__ret__.label,
-        label_prefix=__ret__.label_prefix,
-        links=__ret__.links,
-        name=__ret__.name,
-        recipient=__ret__.recipient,
-        request_compressed=__ret__.request_compressed,
-        response_signed=__ret__.response_signed,
-        saml_signed_request_enabled=__ret__.saml_signed_request_enabled,
-        signature_algorithm=__ret__.signature_algorithm,
-        single_logout_certificate=__ret__.single_logout_certificate,
-        single_logout_issuer=__ret__.single_logout_issuer,
-        single_logout_url=__ret__.single_logout_url,
-        skip_groups=__ret__.skip_groups,
-        skip_users=__ret__.skip_users,
-        sp_issuer=__ret__.sp_issuer,
-        sso_url=__ret__.sso_url,
-        status=__ret__.status,
-        subject_name_id_format=__ret__.subject_name_id_format,
-        subject_name_id_template=__ret__.subject_name_id_template,
-        user_name_template=__ret__.user_name_template,
-        user_name_template_push_status=__ret__.user_name_template_push_status,
-        user_name_template_suffix=__ret__.user_name_template_suffix,
-        user_name_template_type=__ret__.user_name_template_type,
-        users=__ret__.users)
+        accessibility_error_redirect_url=pulumi.get(__ret__, 'accessibility_error_redirect_url'),
+        accessibility_login_redirect_url=pulumi.get(__ret__, 'accessibility_login_redirect_url'),
+        accessibility_self_service=pulumi.get(__ret__, 'accessibility_self_service'),
+        acs_endpoints=pulumi.get(__ret__, 'acs_endpoints'),
+        active_only=pulumi.get(__ret__, 'active_only'),
+        app_settings_json=pulumi.get(__ret__, 'app_settings_json'),
+        assertion_signed=pulumi.get(__ret__, 'assertion_signed'),
+        attribute_statements=pulumi.get(__ret__, 'attribute_statements'),
+        audience=pulumi.get(__ret__, 'audience'),
+        authn_context_class_ref=pulumi.get(__ret__, 'authn_context_class_ref'),
+        auto_submit_toolbar=pulumi.get(__ret__, 'auto_submit_toolbar'),
+        default_relay_state=pulumi.get(__ret__, 'default_relay_state'),
+        destination=pulumi.get(__ret__, 'destination'),
+        digest_algorithm=pulumi.get(__ret__, 'digest_algorithm'),
+        features=pulumi.get(__ret__, 'features'),
+        groups=pulumi.get(__ret__, 'groups'),
+        hide_ios=pulumi.get(__ret__, 'hide_ios'),
+        hide_web=pulumi.get(__ret__, 'hide_web'),
+        honor_force_authn=pulumi.get(__ret__, 'honor_force_authn'),
+        id=pulumi.get(__ret__, 'id'),
+        idp_issuer=pulumi.get(__ret__, 'idp_issuer'),
+        inline_hook_id=pulumi.get(__ret__, 'inline_hook_id'),
+        key_id=pulumi.get(__ret__, 'key_id'),
+        label=pulumi.get(__ret__, 'label'),
+        label_prefix=pulumi.get(__ret__, 'label_prefix'),
+        links=pulumi.get(__ret__, 'links'),
+        name=pulumi.get(__ret__, 'name'),
+        recipient=pulumi.get(__ret__, 'recipient'),
+        request_compressed=pulumi.get(__ret__, 'request_compressed'),
+        response_signed=pulumi.get(__ret__, 'response_signed'),
+        saml_signed_request_enabled=pulumi.get(__ret__, 'saml_signed_request_enabled'),
+        signature_algorithm=pulumi.get(__ret__, 'signature_algorithm'),
+        single_logout_certificate=pulumi.get(__ret__, 'single_logout_certificate'),
+        single_logout_issuer=pulumi.get(__ret__, 'single_logout_issuer'),
+        single_logout_url=pulumi.get(__ret__, 'single_logout_url'),
+        skip_groups=pulumi.get(__ret__, 'skip_groups'),
+        skip_users=pulumi.get(__ret__, 'skip_users'),
+        sp_issuer=pulumi.get(__ret__, 'sp_issuer'),
+        sso_url=pulumi.get(__ret__, 'sso_url'),
+        status=pulumi.get(__ret__, 'status'),
+        subject_name_id_format=pulumi.get(__ret__, 'subject_name_id_format'),
+        subject_name_id_template=pulumi.get(__ret__, 'subject_name_id_template'),
+        user_name_template=pulumi.get(__ret__, 'user_name_template'),
+        user_name_template_push_status=pulumi.get(__ret__, 'user_name_template_push_status'),
+        user_name_template_suffix=pulumi.get(__ret__, 'user_name_template_suffix'),
+        user_name_template_type=pulumi.get(__ret__, 'user_name_template_type'),
+        users=pulumi.get(__ret__, 'users'))
 
 
 @_utilities.lift_output_func(get_saml)
 def get_saml_output(active_only: Optional[pulumi.Input[Optional[bool]]] = None,
                     id: Optional[pulumi.Input[Optional[str]]] = None,
                     label: Optional[pulumi.Input[Optional[str]]] = None,
                     label_prefix: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/group_assignment.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app/group_assignment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/o_auth.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app/o_auth.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/o_auth_post_logout_redirect_uri.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app/o_auth_post_logout_redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/o_auth_redirect_uri.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app/o_auth_redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/outputs.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/saml.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app/saml.py`

 * *Files 1% similar despite different names*

```diff
@@ -1923,16 +1923,14 @@
 
         A SAML App can be imported via the Okta ID.
 
         ```sh
          $ pulumi import okta:app/saml:Saml example &#60;app id&#62;
         ```
 
-         It's also possible to import app without groups or/and users. In this case ID may look like this
-
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] accessibility_error_redirect_url: Custom error page URL.
         :param pulumi.Input[str] accessibility_login_redirect_url: Custom login page for this application.
         :param pulumi.Input[bool] accessibility_self_service: Enable self-service. Default is: `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] acs_endpoints: An array of ACS endpoints. You can configure a maximum of 100 endpoints.
         :param pulumi.Input[str] admin_note: Application notes for admins.
@@ -2131,16 +2129,14 @@
 
         A SAML App can be imported via the Okta ID.
 
         ```sh
          $ pulumi import okta:app/saml:Saml example &#60;app id&#62;
         ```
 
-         It's also possible to import app without groups or/and users. In this case ID may look like this
-
         :param str resource_name: The name of the resource.
         :param SamlArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(SamlArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/secure_password_store.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app/secure_password_store.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/swa.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app/swa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/three_field.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app/three_field.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app/user.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app_group_assignments.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app_group_assignments.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app_oauth_api_scope.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app_oauth_api_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app_saml_app_settings.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app_saml_app_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app_shared_credentials.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app_shared_credentials.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app_signon_policy.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app_signon_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app_signon_policy_rule.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app_signon_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app_user_base_schema_property.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app_user_base_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/app_user_schema_property.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/app_user_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/__init__.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/get_server.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/get_server.py`

 * *Files 5% similar despite different names*

```diff
@@ -183,25 +183,25 @@
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:auth/getServer:getServer', __args__, opts=opts, typ=GetServerResult).value
 
     return AwaitableGetServerResult(
-        audiences=__ret__.audiences,
-        credentials_last_rotated=__ret__.credentials_last_rotated,
-        credentials_next_rotation=__ret__.credentials_next_rotation,
-        credentials_rotation_mode=__ret__.credentials_rotation_mode,
-        description=__ret__.description,
-        id=__ret__.id,
-        issuer=__ret__.issuer,
-        issuer_mode=__ret__.issuer_mode,
-        kid=__ret__.kid,
-        name=__ret__.name,
-        status=__ret__.status)
+        audiences=pulumi.get(__ret__, 'audiences'),
+        credentials_last_rotated=pulumi.get(__ret__, 'credentials_last_rotated'),
+        credentials_next_rotation=pulumi.get(__ret__, 'credentials_next_rotation'),
+        credentials_rotation_mode=pulumi.get(__ret__, 'credentials_rotation_mode'),
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        issuer=pulumi.get(__ret__, 'issuer'),
+        issuer_mode=pulumi.get(__ret__, 'issuer_mode'),
+        kid=pulumi.get(__ret__, 'kid'),
+        name=pulumi.get(__ret__, 'name'),
+        status=pulumi.get(__ret__, 'status'))
 
 
 @_utilities.lift_output_func(get_server)
 def get_server_output(name: Optional[pulumi.Input[str]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServerResult]:
     """
     Use this data source to retrieve an auth server from Okta.
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/get_server_policy.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/get_server_policy.py`

 * *Files 7% similar despite different names*

```diff
@@ -121,20 +121,20 @@
     __args__ = dict()
     __args__['authServerId'] = auth_server_id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:auth/getServerPolicy:getServerPolicy', __args__, opts=opts, typ=GetServerPolicyResult).value
 
     return AwaitableGetServerPolicyResult(
-        assigned_clients=__ret__.assigned_clients,
-        auth_server_id=__ret__.auth_server_id,
-        description=__ret__.description,
-        id=__ret__.id,
-        name=__ret__.name,
-        priority=__ret__.priority)
+        assigned_clients=pulumi.get(__ret__, 'assigned_clients'),
+        auth_server_id=pulumi.get(__ret__, 'auth_server_id'),
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        priority=pulumi.get(__ret__, 'priority'))
 
 
 @_utilities.lift_output_func(get_server_policy)
 def get_server_policy_output(auth_server_id: Optional[pulumi.Input[str]] = None,
                              name: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServerPolicyResult]:
     """
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/get_server_scopes.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/get_server_scopes.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,17 +85,17 @@
     """
     __args__ = dict()
     __args__['authServerId'] = auth_server_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:auth/getServerScopes:getServerScopes', __args__, opts=opts, typ=GetServerScopesResult).value
 
     return AwaitableGetServerScopesResult(
-        auth_server_id=__ret__.auth_server_id,
-        id=__ret__.id,
-        scopes=__ret__.scopes)
+        auth_server_id=pulumi.get(__ret__, 'auth_server_id'),
+        id=pulumi.get(__ret__, 'id'),
+        scopes=pulumi.get(__ret__, 'scopes'))
 
 
 @_utilities.lift_output_func(get_server_scopes)
 def get_server_scopes_output(auth_server_id: Optional[pulumi.Input[str]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetServerScopesResult]:
     """
     Use this data source to retrieve a list of authorization server scopes from Okta.
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/outputs.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/server.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server_claim.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/server_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server_policy.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/server_policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server_policy_claim.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/server_policy_claim.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server_policy_rule.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/server_policy_rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth/server_scope.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/auth/server_scope.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth_server_claim_default.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/auth_server_claim_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/auth_server_default.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/auth_server_default.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                  status: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a AuthServerDefault resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: The recipients that the tokens are intended for. This becomes the `aud` claim in an access token.
         :param pulumi.Input[str] credentials_rotation_mode: The key rotation mode for the authorization server. Can be `"AUTO"` or `"MANUAL"`.
         :param pulumi.Input[str] description: The description of the authorization server.
         :param pulumi.Input[str] issuer_mode: Allows you to use a custom issuer URL. It can be set to `"CUSTOM_URL"`, `"ORG_URL"`, or `"DYNAMIC"`.
-        :param pulumi.Input[str] name: The name of the authorization server.
+        :param pulumi.Input[str] name: The name of the authorization server. Not necessary but left for backwards capacity with legacy implementation.
         :param pulumi.Input[str] status: The status of the auth server.
         """
         if audiences is not None:
             pulumi.set(__self__, "audiences", audiences)
         if credentials_rotation_mode is not None:
             pulumi.set(__self__, "credentials_rotation_mode", credentials_rotation_mode)
         if description is not None:
@@ -90,15 +90,15 @@
     def issuer_mode(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "issuer_mode", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the authorization server.
+        The name of the authorization server. Not necessary but left for backwards capacity with legacy implementation.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -134,15 +134,15 @@
         :param pulumi.Input[str] credentials_last_rotated: The timestamp when the authorization server started to use the `kid` for signing tokens.
         :param pulumi.Input[str] credentials_next_rotation: The timestamp when the authorization server changes the key for signing tokens. Only returned when `credentials_rotation_mode` is `"AUTO"`.
         :param pulumi.Input[str] credentials_rotation_mode: The key rotation mode for the authorization server. Can be `"AUTO"` or `"MANUAL"`.
         :param pulumi.Input[str] description: The description of the authorization server.
         :param pulumi.Input[str] issuer: The complete URL for a Custom Authorization Server. This becomes the `iss` claim in an access token.
         :param pulumi.Input[str] issuer_mode: Allows you to use a custom issuer URL. It can be set to `"CUSTOM_URL"`, `"ORG_URL"`, or `"DYNAMIC"`.
         :param pulumi.Input[str] kid: The ID of the JSON Web Key used for signing tokens issued by the authorization server.
-        :param pulumi.Input[str] name: The name of the authorization server.
+        :param pulumi.Input[str] name: The name of the authorization server. Not necessary but left for backwards capacity with legacy implementation.
         :param pulumi.Input[str] status: The status of the auth server.
         """
         if audiences is not None:
             pulumi.set(__self__, "audiences", audiences)
         if credentials_last_rotated is not None:
             pulumi.set(__self__, "credentials_last_rotated", credentials_last_rotated)
         if credentials_next_rotation is not None:
@@ -258,15 +258,15 @@
     def kid(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "kid", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the authorization server.
+        The name of the authorization server. Not necessary but left for backwards capacity with legacy implementation.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -302,32 +302,34 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_okta as okta
 
-        example = okta.AuthServerDefault("example")
+        example = okta.AuthServerDefault("example",
+            audiences=["api://default"],
+            description="Default Authorization Server for your Applications")
         ```
 
         ## Import
 
         Authorization Server can be imported via the Okta ID.
 
         ```sh
-         $ pulumi import okta:index/authServerDefault:AuthServerDefault example &#60;auth server name&#62;
+         $ pulumi import okta:index/authServerDefault:AuthServerDefault example &#60;default&#62;
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] audiences: The recipients that the tokens are intended for. This becomes the `aud` claim in an access token.
         :param pulumi.Input[str] credentials_rotation_mode: The key rotation mode for the authorization server. Can be `"AUTO"` or `"MANUAL"`.
         :param pulumi.Input[str] description: The description of the authorization server.
         :param pulumi.Input[str] issuer_mode: Allows you to use a custom issuer URL. It can be set to `"CUSTOM_URL"`, `"ORG_URL"`, or `"DYNAMIC"`.
-        :param pulumi.Input[str] name: The name of the authorization server.
+        :param pulumi.Input[str] name: The name of the authorization server. Not necessary but left for backwards capacity with legacy implementation.
         :param pulumi.Input[str] status: The status of the auth server.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[AuthServerDefaultArgs] = None,
@@ -339,23 +341,25 @@
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_okta as okta
 
-        example = okta.AuthServerDefault("example")
+        example = okta.AuthServerDefault("example",
+            audiences=["api://default"],
+            description="Default Authorization Server for your Applications")
         ```
 
         ## Import
 
         Authorization Server can be imported via the Okta ID.
 
         ```sh
-         $ pulumi import okta:index/authServerDefault:AuthServerDefault example &#60;auth server name&#62;
+         $ pulumi import okta:index/authServerDefault:AuthServerDefault example &#60;default&#62;
         ```
 
         :param str resource_name: The name of the resource.
         :param AuthServerDefaultArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
@@ -425,15 +429,15 @@
         :param pulumi.Input[str] credentials_last_rotated: The timestamp when the authorization server started to use the `kid` for signing tokens.
         :param pulumi.Input[str] credentials_next_rotation: The timestamp when the authorization server changes the key for signing tokens. Only returned when `credentials_rotation_mode` is `"AUTO"`.
         :param pulumi.Input[str] credentials_rotation_mode: The key rotation mode for the authorization server. Can be `"AUTO"` or `"MANUAL"`.
         :param pulumi.Input[str] description: The description of the authorization server.
         :param pulumi.Input[str] issuer: The complete URL for a Custom Authorization Server. This becomes the `iss` claim in an access token.
         :param pulumi.Input[str] issuer_mode: Allows you to use a custom issuer URL. It can be set to `"CUSTOM_URL"`, `"ORG_URL"`, or `"DYNAMIC"`.
         :param pulumi.Input[str] kid: The ID of the JSON Web Key used for signing tokens issued by the authorization server.
-        :param pulumi.Input[str] name: The name of the authorization server.
+        :param pulumi.Input[str] name: The name of the authorization server. Not necessary but left for backwards capacity with legacy implementation.
         :param pulumi.Input[str] status: The status of the auth server.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _AuthServerDefaultState.__new__(_AuthServerDefaultState)
 
         __props__.__dict__["audiences"] = audiences
@@ -512,15 +516,15 @@
         """
         return pulumi.get(self, "kid")
 
     @property
     @pulumi.getter
     def name(self) -> pulumi.Output[str]:
         """
-        The name of the authorization server.
+        The name of the authorization server. Not necessary but left for backwards capacity with legacy implementation.
         """
         return pulumi.get(self, "name")
 
     @property
     @pulumi.getter
     def status(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/authenticator.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/authenticator.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/behaviour.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/behaviour.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/brand.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/brand.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
                  agree_to_custom_privacy_policy: Optional[pulumi.Input[bool]] = None,
                  brand_id: Optional[pulumi.Input[str]] = None,
                  custom_privacy_policy_url: Optional[pulumi.Input[str]] = None,
                  remove_powered_by_okta: Optional[pulumi.Input[bool]] = None):
         """
         The set of arguments for constructing a Brand resource.
         :param pulumi.Input[bool] agree_to_custom_privacy_policy: Is a required input flag with when changing custom_privacy_url, shouldn't be considered as a readable property
-        :param pulumi.Input[str] brand_id: Brand ID, used for read (faux-create)
+        :param pulumi.Input[str] brand_id: Brand ID, used for read (faux-create). Setting `brand_id` to `default` is equivalent to importing the default brand by its ID.
         :param pulumi.Input[str] custom_privacy_policy_url: (Optional) Custom privacy policy URL
         :param pulumi.Input[bool] remove_powered_by_okta: (Optional) Removes "Powered by Okta" from the Okta-hosted sign-in page, and "© 2021 Okta, Inc." from the Okta End-User Dashboard
         """
         if agree_to_custom_privacy_policy is not None:
             pulumi.set(__self__, "agree_to_custom_privacy_policy", agree_to_custom_privacy_policy)
         if brand_id is not None:
             pulumi.set(__self__, "brand_id", brand_id)
@@ -46,15 +46,15 @@
     def agree_to_custom_privacy_policy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "agree_to_custom_privacy_policy", value)
 
     @property
     @pulumi.getter(name="brandId")
     def brand_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Brand ID, used for read (faux-create)
+        Brand ID, used for read (faux-create). Setting `brand_id` to `default` is equivalent to importing the default brand by its ID.
         """
         return pulumi.get(self, "brand_id")
 
     @brand_id.setter
     def brand_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "brand_id", value)
 
@@ -91,15 +91,15 @@
                  custom_privacy_policy_url: Optional[pulumi.Input[str]] = None,
                  links: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  remove_powered_by_okta: Optional[pulumi.Input[bool]] = None):
         """
         Input properties used for looking up and filtering Brand resources.
         :param pulumi.Input[bool] agree_to_custom_privacy_policy: Is a required input flag with when changing custom_privacy_url, shouldn't be considered as a readable property
-        :param pulumi.Input[str] brand_id: Brand ID, used for read (faux-create)
+        :param pulumi.Input[str] brand_id: Brand ID, used for read (faux-create). Setting `brand_id` to `default` is equivalent to importing the default brand by its ID.
         :param pulumi.Input[str] custom_privacy_policy_url: (Optional) Custom privacy policy URL
         :param pulumi.Input[str] links: (Read-only) Link relations for this object - JSON HAL - Discoverable resources related to the brand
         :param pulumi.Input[str] name: Brand name
         :param pulumi.Input[bool] remove_powered_by_okta: (Optional) Removes "Powered by Okta" from the Okta-hosted sign-in page, and "© 2021 Okta, Inc." from the Okta End-User Dashboard
         """
         if agree_to_custom_privacy_policy is not None:
             pulumi.set(__self__, "agree_to_custom_privacy_policy", agree_to_custom_privacy_policy)
@@ -126,15 +126,15 @@
     def agree_to_custom_privacy_policy(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "agree_to_custom_privacy_policy", value)
 
     @property
     @pulumi.getter(name="brandId")
     def brand_id(self) -> Optional[pulumi.Input[str]]:
         """
-        Brand ID, used for read (faux-create)
+        Brand ID, used for read (faux-create). Setting `brand_id` to `default` is equivalent to importing the default brand by its ID.
         """
         return pulumi.get(self, "brand_id")
 
     @brand_id.setter
     def brand_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "brand_id", value)
 
@@ -206,28 +206,34 @@
 
         # resource has been imported into current state
         # $ terraform import okta_brand.example <brand id>
         example = okta.Brand("example",
             agree_to_custom_privacy_policy=True,
             custom_privacy_policy_url="https://example.com/privacy-policy",
             remove_powered_by_okta=True)
+        # setting brand_id to default is equivalent to importing the default brand by its ID
+        default = okta.Brand("default",
+            agree_to_custom_privacy_policy=True,
+            brand_id="default",
+            custom_privacy_policy_url="https://example.com/privacy-policy",
+            remove_powered_by_okta=True)
         ```
 
         ## Import
 
         An Okta Brand can be imported via the ID.
 
         ```sh
          $ pulumi import okta:index/brand:Brand example &#60;brand id&#62;
         ```
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] agree_to_custom_privacy_policy: Is a required input flag with when changing custom_privacy_url, shouldn't be considered as a readable property
-        :param pulumi.Input[str] brand_id: Brand ID, used for read (faux-create)
+        :param pulumi.Input[str] brand_id: Brand ID, used for read (faux-create). Setting `brand_id` to `default` is equivalent to importing the default brand by its ID.
         :param pulumi.Input[str] custom_privacy_policy_url: (Optional) Custom privacy policy URL
         :param pulumi.Input[bool] remove_powered_by_okta: (Optional) Removes "Powered by Okta" from the Okta-hosted sign-in page, and "© 2021 Okta, Inc." from the Okta End-User Dashboard
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
@@ -242,14 +248,20 @@
 
         # resource has been imported into current state
         # $ terraform import okta_brand.example <brand id>
         example = okta.Brand("example",
             agree_to_custom_privacy_policy=True,
             custom_privacy_policy_url="https://example.com/privacy-policy",
             remove_powered_by_okta=True)
+        # setting brand_id to default is equivalent to importing the default brand by its ID
+        default = okta.Brand("default",
+            agree_to_custom_privacy_policy=True,
+            brand_id="default",
+            custom_privacy_policy_url="https://example.com/privacy-policy",
+            remove_powered_by_okta=True)
         ```
 
         ## Import
 
         An Okta Brand can be imported via the ID.
 
         ```sh
@@ -310,15 +322,15 @@
         Get an existing Brand resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
         :param str resource_name: The unique name of the resulting resource.
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[bool] agree_to_custom_privacy_policy: Is a required input flag with when changing custom_privacy_url, shouldn't be considered as a readable property
-        :param pulumi.Input[str] brand_id: Brand ID, used for read (faux-create)
+        :param pulumi.Input[str] brand_id: Brand ID, used for read (faux-create). Setting `brand_id` to `default` is equivalent to importing the default brand by its ID.
         :param pulumi.Input[str] custom_privacy_policy_url: (Optional) Custom privacy policy URL
         :param pulumi.Input[str] links: (Read-only) Link relations for this object - JSON HAL - Discoverable resources related to the brand
         :param pulumi.Input[str] name: Brand name
         :param pulumi.Input[bool] remove_powered_by_okta: (Optional) Removes "Powered by Okta" from the Okta-hosted sign-in page, and "© 2021 Okta, Inc." from the Okta End-User Dashboard
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
@@ -340,15 +352,15 @@
         """
         return pulumi.get(self, "agree_to_custom_privacy_policy")
 
     @property
     @pulumi.getter(name="brandId")
     def brand_id(self) -> pulumi.Output[Optional[str]]:
         """
-        Brand ID, used for read (faux-create)
+        Brand ID, used for read (faux-create). Setting `brand_id` to `default` is equivalent to importing the default brand by its ID.
         """
         return pulumi.get(self, "brand_id")
 
     @property
     @pulumi.getter(name="customPrivacyPolicyUrl")
     def custom_privacy_policy_url(self) -> pulumi.Output[Optional[str]]:
         """
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/captcha.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/captcha.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/captcha_org_wide_settings.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/captcha_org_wide_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/config/vars.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/domain.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/domain_certificate.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/domain_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/domain_verification.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/domain_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/email_sender.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/email_sender.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,14 +160,16 @@
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  from_address: Optional[pulumi.Input[str]] = None,
                  from_name: Optional[pulumi.Input[str]] = None,
                  subdomain: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
+        > **DEPRECATED** use `Index.EmailDomain` instead.
+
         This resource allows you to create and configure a custom email sender.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_okta as okta
@@ -195,14 +197,16 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: EmailSenderArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        > **DEPRECATED** use `Index.EmailDomain` instead.
+
         This resource allows you to create and configure a custom email sender.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_okta as okta
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/email_sender_verification.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/email_sender_verification.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,16 @@
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  sender_id: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
+        > **DEPRECATED** use `Index.EmailDomainVerification` instead.
+
         Verifies the email sender. The resource won't be created if the email sender could not be verified.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_okta as okta
@@ -92,14 +94,16 @@
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: EmailSenderVerificationArgs,
                  opts: Optional[pulumi.ResourceOptions] = None):
         """
+        > **DEPRECATED** use `Index.EmailDomainVerification` instead.
+
         Verifies the email sender. The resource won't be created if the email sender could not be verified.
 
         ## Example Usage
 
         ```python
         import pulumi
         import pulumi_okta as okta
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/event_hook.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/event_hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/event_hook_verification.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/event_hook_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/factor/factor.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/factor/factor.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/factor_totp.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/factor_totp.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_app_group_assignments.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_app_group_assignments.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,16 +75,16 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getAppGroupAssignments:getAppGroupAssignments', __args__, opts=opts, typ=GetAppGroupAssignmentsResult).value
 
     return AwaitableGetAppGroupAssignmentsResult(
-        groups=__ret__.groups,
-        id=__ret__.id)
+        groups=pulumi.get(__ret__, 'groups'),
+        id=pulumi.get(__ret__, 'id'))
 
 
 @_utilities.lift_output_func(get_app_group_assignments)
 def get_app_group_assignments_output(id: Optional[pulumi.Input[str]] = None,
                                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppGroupAssignmentsResult]:
     """
     Use this data source to retrieve the list of groups assigned to the given Okta application (by ID).
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_app_signon_policy.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_app_signon_policy.py`

 * *Files 6% similar despite different names*

```diff
@@ -83,17 +83,17 @@
     """
     __args__ = dict()
     __args__['appId'] = app_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getAppSignonPolicy:getAppSignonPolicy', __args__, opts=opts, typ=GetAppSignonPolicyResult).value
 
     return AwaitableGetAppSignonPolicyResult(
-        app_id=__ret__.app_id,
-        id=__ret__.id,
-        name=__ret__.name)
+        app_id=pulumi.get(__ret__, 'app_id'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'))
 
 
 @_utilities.lift_output_func(get_app_signon_policy)
 def get_app_signon_policy_output(app_id: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppSignonPolicyResult]:
     """
     > **WARNING:** This feature is only available as a part of the Identity Engine. Contact support for further information.
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_app_user_assignments.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_app_user_assignments.py`

 * *Files 10% similar despite different names*

```diff
@@ -75,16 +75,16 @@
     """
     __args__ = dict()
     __args__['id'] = id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getAppUserAssignments:getAppUserAssignments', __args__, opts=opts, typ=GetAppUserAssignmentsResult).value
 
     return AwaitableGetAppUserAssignmentsResult(
-        id=__ret__.id,
-        users=__ret__.users)
+        id=pulumi.get(__ret__, 'id'),
+        users=pulumi.get(__ret__, 'users'))
 
 
 @_utilities.lift_output_func(get_app_user_assignments)
 def get_app_user_assignments_output(id: Optional[pulumi.Input[str]] = None,
                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAppUserAssignmentsResult]:
     """
     Use this data source to retrieve the list of users assigned to the given Okta application (by ID).
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_auth_server_claim.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_auth_server_claim.py`

 * *Files 5% similar despite different names*

```diff
@@ -163,23 +163,23 @@
     __args__['authServerId'] = auth_server_id
     __args__['id'] = id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getAuthServerClaim:getAuthServerClaim', __args__, opts=opts, typ=GetAuthServerClaimResult).value
 
     return AwaitableGetAuthServerClaimResult(
-        always_include_in_token=__ret__.always_include_in_token,
-        auth_server_id=__ret__.auth_server_id,
-        claim_type=__ret__.claim_type,
-        id=__ret__.id,
-        name=__ret__.name,
-        scopes=__ret__.scopes,
-        status=__ret__.status,
-        value=__ret__.value,
-        value_type=__ret__.value_type)
+        always_include_in_token=pulumi.get(__ret__, 'always_include_in_token'),
+        auth_server_id=pulumi.get(__ret__, 'auth_server_id'),
+        claim_type=pulumi.get(__ret__, 'claim_type'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        scopes=pulumi.get(__ret__, 'scopes'),
+        status=pulumi.get(__ret__, 'status'),
+        value=pulumi.get(__ret__, 'value'),
+        value_type=pulumi.get(__ret__, 'value_type'))
 
 
 @_utilities.lift_output_func(get_auth_server_claim)
 def get_auth_server_claim_output(auth_server_id: Optional[pulumi.Input[str]] = None,
                                  id: Optional[pulumi.Input[Optional[str]]] = None,
                                  name: Optional[pulumi.Input[Optional[str]]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAuthServerClaimResult]:
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_auth_server_claims.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_auth_server_claims.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,17 +85,17 @@
     """
     __args__ = dict()
     __args__['authServerId'] = auth_server_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getAuthServerClaims:getAuthServerClaims', __args__, opts=opts, typ=GetAuthServerClaimsResult).value
 
     return AwaitableGetAuthServerClaimsResult(
-        auth_server_id=__ret__.auth_server_id,
-        claims=__ret__.claims,
-        id=__ret__.id)
+        auth_server_id=pulumi.get(__ret__, 'auth_server_id'),
+        claims=pulumi.get(__ret__, 'claims'),
+        id=pulumi.get(__ret__, 'id'))
 
 
 @_utilities.lift_output_func(get_auth_server_claims)
 def get_auth_server_claims_output(auth_server_id: Optional[pulumi.Input[str]] = None,
                                   opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAuthServerClaimsResult]:
     """
     Use this data source to retrieve a list of authorization server claims from Okta.
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_authenticator.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_authenticator.py`

 * *Files 10% similar despite different names*

```diff
@@ -204,26 +204,26 @@
     __args__['id'] = id
     __args__['key'] = key
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getAuthenticator:getAuthenticator', __args__, opts=opts, typ=GetAuthenticatorResult).value
 
     return AwaitableGetAuthenticatorResult(
-        id=__ret__.id,
-        key=__ret__.key,
-        name=__ret__.name,
-        provider_auth_port=__ret__.provider_auth_port,
-        provider_hostname=__ret__.provider_hostname,
-        provider_instance_id=__ret__.provider_instance_id,
-        provider_json=__ret__.provider_json,
-        provider_type=__ret__.provider_type,
-        provider_user_name_template=__ret__.provider_user_name_template,
-        settings=__ret__.settings,
-        status=__ret__.status,
-        type=__ret__.type)
+        id=pulumi.get(__ret__, 'id'),
+        key=pulumi.get(__ret__, 'key'),
+        name=pulumi.get(__ret__, 'name'),
+        provider_auth_port=pulumi.get(__ret__, 'provider_auth_port'),
+        provider_hostname=pulumi.get(__ret__, 'provider_hostname'),
+        provider_instance_id=pulumi.get(__ret__, 'provider_instance_id'),
+        provider_json=pulumi.get(__ret__, 'provider_json'),
+        provider_type=pulumi.get(__ret__, 'provider_type'),
+        provider_user_name_template=pulumi.get(__ret__, 'provider_user_name_template'),
+        settings=pulumi.get(__ret__, 'settings'),
+        status=pulumi.get(__ret__, 'status'),
+        type=pulumi.get(__ret__, 'type'))
 
 
 @_utilities.lift_output_func(get_authenticator)
 def get_authenticator_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                              key: Optional[pulumi.Input[Optional[str]]] = None,
                              name: Optional[pulumi.Input[Optional[str]]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetAuthenticatorResult]:
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_behaviour.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_behaviour.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,19 +106,19 @@
     __args__ = dict()
     __args__['id'] = id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getBehaviour:getBehaviour', __args__, opts=opts, typ=GetBehaviourResult).value
 
     return AwaitableGetBehaviourResult(
-        id=__ret__.id,
-        name=__ret__.name,
-        settings=__ret__.settings,
-        status=__ret__.status,
-        type=__ret__.type)
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        settings=pulumi.get(__ret__, 'settings'),
+        status=pulumi.get(__ret__, 'status'),
+        type=pulumi.get(__ret__, 'type'))
 
 
 @_utilities.lift_output_func(get_behaviour)
 def get_behaviour_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                          name: Optional[pulumi.Input[Optional[str]]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetBehaviourResult]:
     """
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_behaviours.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_behaviours.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,17 +85,17 @@
     """
     __args__ = dict()
     __args__['q'] = q
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getBehaviours:getBehaviours', __args__, opts=opts, typ=GetBehavioursResult).value
 
     return AwaitableGetBehavioursResult(
-        behaviors=__ret__.behaviors,
-        id=__ret__.id,
-        q=__ret__.q)
+        behaviors=pulumi.get(__ret__, 'behaviors'),
+        id=pulumi.get(__ret__, 'id'),
+        q=pulumi.get(__ret__, 'q'))
 
 
 @_utilities.lift_output_func(get_behaviours)
 def get_behaviours_output(q: Optional[pulumi.Input[Optional[str]]] = None,
                           opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetBehavioursResult]:
     """
     Use this data source to retrieve a behaviors from Okta.
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_brand.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_brand.py`

 * *Files 8% similar despite different names*

```diff
@@ -100,33 +100,33 @@
 
 def get_brand(brand_id: Optional[str] = None,
               opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetBrandResult:
     """
     Use this data source to retrieve a [Brand](https://developer.okta.com/docs/reference/api/brands/#brand-object) from Okta.
 
 
-    :param str brand_id: Brand ID
+    :param str brand_id: Brand ID. Setting `brand_id` to `default` is equivalent to importing the default brand by its ID.
     """
     __args__ = dict()
     __args__['brandId'] = brand_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getBrand:getBrand', __args__, opts=opts, typ=GetBrandResult).value
 
     return AwaitableGetBrandResult(
-        brand_id=__ret__.brand_id,
-        custom_privacy_policy_url=__ret__.custom_privacy_policy_url,
-        id=__ret__.id,
-        links=__ret__.links,
-        name=__ret__.name,
-        remove_powered_by_okta=__ret__.remove_powered_by_okta)
+        brand_id=pulumi.get(__ret__, 'brand_id'),
+        custom_privacy_policy_url=pulumi.get(__ret__, 'custom_privacy_policy_url'),
+        id=pulumi.get(__ret__, 'id'),
+        links=pulumi.get(__ret__, 'links'),
+        name=pulumi.get(__ret__, 'name'),
+        remove_powered_by_okta=pulumi.get(__ret__, 'remove_powered_by_okta'))
 
 
 @_utilities.lift_output_func(get_brand)
 def get_brand_output(brand_id: Optional[pulumi.Input[str]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetBrandResult]:
     """
     Use this data source to retrieve a [Brand](https://developer.okta.com/docs/reference/api/brands/#brand-object) from Okta.
 
 
-    :param str brand_id: Brand ID
+    :param str brand_id: Brand ID. Setting `brand_id` to `default` is equivalent to importing the default brand by its ID.
     """
     ...
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_brands.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_brands.py`

 * *Files 12% similar despite different names*

```diff
@@ -70,9 +70,9 @@
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getBrands:getBrands', __args__, opts=opts, typ=GetBrandsResult).value
 
     return AwaitableGetBrandsResult(
-        brands=__ret__.brands,
-        id=__ret__.id)
+        brands=pulumi.get(__ret__, 'brands'),
+        id=pulumi.get(__ret__, 'id'))
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_email_customization.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_email_customization.py`

 * *Files 5% similar despite different names*

```diff
@@ -149,23 +149,23 @@
     __args__['brandId'] = brand_id
     __args__['customizationId'] = customization_id
     __args__['templateName'] = template_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getEmailCustomization:getEmailCustomization', __args__, opts=opts, typ=GetEmailCustomizationResult).value
 
     return AwaitableGetEmailCustomizationResult(
-        body=__ret__.body,
-        brand_id=__ret__.brand_id,
-        customization_id=__ret__.customization_id,
-        id=__ret__.id,
-        is_default=__ret__.is_default,
-        language=__ret__.language,
-        links=__ret__.links,
-        subject=__ret__.subject,
-        template_name=__ret__.template_name)
+        body=pulumi.get(__ret__, 'body'),
+        brand_id=pulumi.get(__ret__, 'brand_id'),
+        customization_id=pulumi.get(__ret__, 'customization_id'),
+        id=pulumi.get(__ret__, 'id'),
+        is_default=pulumi.get(__ret__, 'is_default'),
+        language=pulumi.get(__ret__, 'language'),
+        links=pulumi.get(__ret__, 'links'),
+        subject=pulumi.get(__ret__, 'subject'),
+        template_name=pulumi.get(__ret__, 'template_name'))
 
 
 @_utilities.lift_output_func(get_email_customization)
 def get_email_customization_output(brand_id: Optional[pulumi.Input[str]] = None,
                                    customization_id: Optional[pulumi.Input[str]] = None,
                                    template_name: Optional[pulumi.Input[str]] = None,
                                    opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetEmailCustomizationResult]:
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_email_customizations.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_email_customizations.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,18 +90,18 @@
     __args__ = dict()
     __args__['brandId'] = brand_id
     __args__['templateName'] = template_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getEmailCustomizations:getEmailCustomizations', __args__, opts=opts, typ=GetEmailCustomizationsResult).value
 
     return AwaitableGetEmailCustomizationsResult(
-        brand_id=__ret__.brand_id,
-        email_customizations=__ret__.email_customizations,
-        id=__ret__.id,
-        template_name=__ret__.template_name)
+        brand_id=pulumi.get(__ret__, 'brand_id'),
+        email_customizations=pulumi.get(__ret__, 'email_customizations'),
+        id=pulumi.get(__ret__, 'id'),
+        template_name=pulumi.get(__ret__, 'template_name'))
 
 
 @_utilities.lift_output_func(get_email_customizations)
 def get_email_customizations_output(brand_id: Optional[pulumi.Input[str]] = None,
                                     template_name: Optional[pulumi.Input[str]] = None,
                                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetEmailCustomizationsResult]:
     """
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_groups.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_groups.py`

 * *Files 2% similar despite different names*

```diff
@@ -116,19 +116,19 @@
     __args__['q'] = q
     __args__['search'] = search
     __args__['type'] = type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getGroups:getGroups', __args__, opts=opts, typ=GetGroupsResult).value
 
     return AwaitableGetGroupsResult(
-        groups=__ret__.groups,
-        id=__ret__.id,
-        q=__ret__.q,
-        search=__ret__.search,
-        type=__ret__.type)
+        groups=pulumi.get(__ret__, 'groups'),
+        id=pulumi.get(__ret__, 'id'),
+        q=pulumi.get(__ret__, 'q'),
+        search=pulumi.get(__ret__, 'search'),
+        type=pulumi.get(__ret__, 'type'))
 
 
 @_utilities.lift_output_func(get_groups)
 def get_groups_output(q: Optional[pulumi.Input[Optional[str]]] = None,
                       search: Optional[pulumi.Input[Optional[str]]] = None,
                       type: Optional[pulumi.Input[Optional[str]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetGroupsResult]:
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_network_zone.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_network_zone.py`

 * *Files 5% similar despite different names*

```diff
@@ -174,24 +174,24 @@
     __args__ = dict()
     __args__['id'] = id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getNetworkZone:getNetworkZone', __args__, opts=opts, typ=GetNetworkZoneResult).value
 
     return AwaitableGetNetworkZoneResult(
-        asns=__ret__.asns,
-        dynamic_locations=__ret__.dynamic_locations,
-        dynamic_proxy_type=__ret__.dynamic_proxy_type,
-        gateways=__ret__.gateways,
-        id=__ret__.id,
-        name=__ret__.name,
-        proxies=__ret__.proxies,
-        status=__ret__.status,
-        type=__ret__.type,
-        usage=__ret__.usage)
+        asns=pulumi.get(__ret__, 'asns'),
+        dynamic_locations=pulumi.get(__ret__, 'dynamic_locations'),
+        dynamic_proxy_type=pulumi.get(__ret__, 'dynamic_proxy_type'),
+        gateways=pulumi.get(__ret__, 'gateways'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        proxies=pulumi.get(__ret__, 'proxies'),
+        status=pulumi.get(__ret__, 'status'),
+        type=pulumi.get(__ret__, 'type'),
+        usage=pulumi.get(__ret__, 'usage'))
 
 
 @_utilities.lift_output_func(get_network_zone)
 def get_network_zone_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                             name: Optional[pulumi.Input[Optional[str]]] = None,
                             opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetNetworkZoneResult]:
     """
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_role_subscription.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_role_subscription.py`

 * *Files 9% similar despite different names*

```diff
@@ -111,18 +111,18 @@
     __args__ = dict()
     __args__['notificationType'] = notification_type
     __args__['roleType'] = role_type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getRoleSubscription:getRoleSubscription', __args__, opts=opts, typ=GetRoleSubscriptionResult).value
 
     return AwaitableGetRoleSubscriptionResult(
-        id=__ret__.id,
-        notification_type=__ret__.notification_type,
-        role_type=__ret__.role_type,
-        status=__ret__.status)
+        id=pulumi.get(__ret__, 'id'),
+        notification_type=pulumi.get(__ret__, 'notification_type'),
+        role_type=pulumi.get(__ret__, 'role_type'),
+        status=pulumi.get(__ret__, 'status'))
 
 
 @_utilities.lift_output_func(get_role_subscription)
 def get_role_subscription_output(notification_type: Optional[pulumi.Input[str]] = None,
                                  role_type: Optional[pulumi.Input[str]] = None,
                                  opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetRoleSubscriptionResult]:
     """
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_template.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,18 +89,18 @@
     __args__ = dict()
     __args__['brandId'] = brand_id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getTemplate:getTemplate', __args__, opts=opts, typ=GetTemplateResult).value
 
     return AwaitableGetTemplateResult(
-        brand_id=__ret__.brand_id,
-        id=__ret__.id,
-        links=__ret__.links,
-        name=__ret__.name)
+        brand_id=pulumi.get(__ret__, 'brand_id'),
+        id=pulumi.get(__ret__, 'id'),
+        links=pulumi.get(__ret__, 'links'),
+        name=pulumi.get(__ret__, 'name'))
 
 
 @_utilities.lift_output_func(get_template)
 def get_template_output(brand_id: Optional[pulumi.Input[str]] = None,
                         name: Optional[pulumi.Input[str]] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTemplateResult]:
     """
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_templates.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_templates.py`

 * *Files 7% similar despite different names*

```diff
@@ -78,17 +78,17 @@
     """
     __args__ = dict()
     __args__['brandId'] = brand_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getTemplates:getTemplates', __args__, opts=opts, typ=GetTemplatesResult).value
 
     return AwaitableGetTemplatesResult(
-        brand_id=__ret__.brand_id,
-        email_templates=__ret__.email_templates,
-        id=__ret__.id)
+        brand_id=pulumi.get(__ret__, 'brand_id'),
+        email_templates=pulumi.get(__ret__, 'email_templates'),
+        id=pulumi.get(__ret__, 'id'))
 
 
 @_utilities.lift_output_func(get_templates)
 def get_templates_output(brand_id: Optional[pulumi.Input[str]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTemplatesResult]:
     """
     Use this data source to retrieve the [email
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_theme.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_theme.py`

 * *Files 14% similar despite different names*

```diff
@@ -221,29 +221,29 @@
     __args__ = dict()
     __args__['brandId'] = brand_id
     __args__['themeId'] = theme_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getTheme:getTheme', __args__, opts=opts, typ=GetThemeResult).value
 
     return AwaitableGetThemeResult(
-        background_image_url=__ret__.background_image_url,
-        brand_id=__ret__.brand_id,
-        email_template_touch_point_variant=__ret__.email_template_touch_point_variant,
-        end_user_dashboard_touch_point_variant=__ret__.end_user_dashboard_touch_point_variant,
-        error_page_touch_point_variant=__ret__.error_page_touch_point_variant,
-        favicon_url=__ret__.favicon_url,
-        id=__ret__.id,
-        links=__ret__.links,
-        logo_url=__ret__.logo_url,
-        primary_color_contrast_hex=__ret__.primary_color_contrast_hex,
-        primary_color_hex=__ret__.primary_color_hex,
-        secondary_color_contrast_hex=__ret__.secondary_color_contrast_hex,
-        secondary_color_hex=__ret__.secondary_color_hex,
-        sign_in_page_touch_point_variant=__ret__.sign_in_page_touch_point_variant,
-        theme_id=__ret__.theme_id)
+        background_image_url=pulumi.get(__ret__, 'background_image_url'),
+        brand_id=pulumi.get(__ret__, 'brand_id'),
+        email_template_touch_point_variant=pulumi.get(__ret__, 'email_template_touch_point_variant'),
+        end_user_dashboard_touch_point_variant=pulumi.get(__ret__, 'end_user_dashboard_touch_point_variant'),
+        error_page_touch_point_variant=pulumi.get(__ret__, 'error_page_touch_point_variant'),
+        favicon_url=pulumi.get(__ret__, 'favicon_url'),
+        id=pulumi.get(__ret__, 'id'),
+        links=pulumi.get(__ret__, 'links'),
+        logo_url=pulumi.get(__ret__, 'logo_url'),
+        primary_color_contrast_hex=pulumi.get(__ret__, 'primary_color_contrast_hex'),
+        primary_color_hex=pulumi.get(__ret__, 'primary_color_hex'),
+        secondary_color_contrast_hex=pulumi.get(__ret__, 'secondary_color_contrast_hex'),
+        secondary_color_hex=pulumi.get(__ret__, 'secondary_color_hex'),
+        sign_in_page_touch_point_variant=pulumi.get(__ret__, 'sign_in_page_touch_point_variant'),
+        theme_id=pulumi.get(__ret__, 'theme_id'))
 
 
 @_utilities.lift_output_func(get_theme)
 def get_theme_output(brand_id: Optional[pulumi.Input[str]] = None,
                      theme_id: Optional[pulumi.Input[str]] = None,
                      opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetThemeResult]:
     """
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_themes.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_themes.py`

 * *Files 12% similar despite different names*

```diff
@@ -78,17 +78,17 @@
     """
     __args__ = dict()
     __args__['brandId'] = brand_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getThemes:getThemes', __args__, opts=opts, typ=GetThemesResult).value
 
     return AwaitableGetThemesResult(
-        brand_id=__ret__.brand_id,
-        id=__ret__.id,
-        themes=__ret__.themes)
+        brand_id=pulumi.get(__ret__, 'brand_id'),
+        id=pulumi.get(__ret__, 'id'),
+        themes=pulumi.get(__ret__, 'themes'))
 
 
 @_utilities.lift_output_func(get_themes)
 def get_themes_output(brand_id: Optional[pulumi.Input[str]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetThemesResult]:
     """
     Use this data source to retrieve
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_trusted_origins.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_trusted_origins.py`

 * *Files 7% similar despite different names*

```diff
@@ -82,17 +82,17 @@
     """
     __args__ = dict()
     __args__['filter'] = filter
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getTrustedOrigins:getTrustedOrigins', __args__, opts=opts, typ=GetTrustedOriginsResult).value
 
     return AwaitableGetTrustedOriginsResult(
-        filter=__ret__.filter,
-        id=__ret__.id,
-        trusted_origins=__ret__.trusted_origins)
+        filter=pulumi.get(__ret__, 'filter'),
+        id=pulumi.get(__ret__, 'id'),
+        trusted_origins=pulumi.get(__ret__, 'trusted_origins'))
 
 
 @_utilities.lift_output_func(get_trusted_origins)
 def get_trusted_origins_output(filter: Optional[pulumi.Input[Optional[str]]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetTrustedOriginsResult]:
     """
     This resource allows you to retrieve a list of trusted origins from Okta.
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/get_user_security_questions.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/get_user_security_questions.py`

 * *Files 8% similar despite different names*

```diff
@@ -90,17 +90,17 @@
     """
     __args__ = dict()
     __args__['userId'] = user_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:index/getUserSecurityQuestions:getUserSecurityQuestions', __args__, opts=opts, typ=GetUserSecurityQuestionsResult).value
 
     return AwaitableGetUserSecurityQuestionsResult(
-        id=__ret__.id,
-        questions=__ret__.questions,
-        user_id=__ret__.user_id)
+        id=pulumi.get(__ret__, 'id'),
+        questions=pulumi.get(__ret__, 'questions'),
+        user_id=pulumi.get(__ret__, 'user_id'))
 
 
 @_utilities.lift_output_func(get_user_security_questions)
 def get_user_security_questions_output(user_id: Optional[pulumi.Input[str]] = None,
                                        opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserSecurityQuestionsResult]:
     """
     Use this data source to retrieve a list of user's security questions.
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/group/get_everyone_group.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/group/get_everyone_group.py`

 * *Files 8% similar despite different names*

```diff
@@ -85,17 +85,17 @@
     """
     __args__ = dict()
     __args__['includeUsers'] = include_users
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:group/getEveryoneGroup:getEveryoneGroup', __args__, opts=opts, typ=GetEveryoneGroupResult).value
 
     return AwaitableGetEveryoneGroupResult(
-        description=__ret__.description,
-        id=__ret__.id,
-        include_users=__ret__.include_users)
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        include_users=pulumi.get(__ret__, 'include_users'))
 
 
 @_utilities.lift_output_func(get_everyone_group)
 def get_everyone_group_output(include_users: Optional[pulumi.Input[Optional[bool]]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetEveryoneGroupResult]:
     """
     Use this data source to retrieve the `Everyone` group from Okta. The same can be achieved with the `group.Group` data
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/group/get_group.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/group/get_group.py`

 * *Files 6% similar despite different names*

```diff
@@ -142,21 +142,21 @@
     __args__['includeUsers'] = include_users
     __args__['name'] = name
     __args__['type'] = type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:group/getGroup:getGroup', __args__, opts=opts, typ=GetGroupResult).value
 
     return AwaitableGetGroupResult(
-        delay_read_seconds=__ret__.delay_read_seconds,
-        description=__ret__.description,
-        id=__ret__.id,
-        include_users=__ret__.include_users,
-        name=__ret__.name,
-        type=__ret__.type,
-        users=__ret__.users)
+        delay_read_seconds=pulumi.get(__ret__, 'delay_read_seconds'),
+        description=pulumi.get(__ret__, 'description'),
+        id=pulumi.get(__ret__, 'id'),
+        include_users=pulumi.get(__ret__, 'include_users'),
+        name=pulumi.get(__ret__, 'name'),
+        type=pulumi.get(__ret__, 'type'),
+        users=pulumi.get(__ret__, 'users'))
 
 
 @_utilities.lift_output_func(get_group)
 def get_group_output(delay_read_seconds: Optional[pulumi.Input[Optional[str]]] = None,
                      id: Optional[pulumi.Input[Optional[str]]] = None,
                      include_users: Optional[pulumi.Input[Optional[bool]]] = None,
                      name: Optional[pulumi.Input[Optional[str]]] = None,
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/group/group.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/group/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,14 +75,17 @@
 
     @property
     @pulumi.getter(name="skipUsers")
     def skip_users(self) -> Optional[pulumi.Input[bool]]:
         """
         Ignore users sync. This is a temporary solution until 'users' field is supported in all the app-like resources
         """
+        warnings.warn("""Because users has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+        pulumi.log.warn("""skip_users is deprecated: Because users has been removed, this attribute is a no op and will be removed""")
+
         return pulumi.get(self, "skip_users")
 
     @skip_users.setter
     def skip_users(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "skip_users", value)
 
 
@@ -150,14 +153,17 @@
 
     @property
     @pulumi.getter(name="skipUsers")
     def skip_users(self) -> Optional[pulumi.Input[bool]]:
         """
         Ignore users sync. This is a temporary solution until 'users' field is supported in all the app-like resources
         """
+        warnings.warn("""Because users has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+        pulumi.log.warn("""skip_users is deprecated: Because users has been removed, this attribute is a no op and will be removed""")
+
         return pulumi.get(self, "skip_users")
 
     @skip_users.setter
     def skip_users(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "skip_users", value)
 
 
@@ -355,9 +361,12 @@
 
     @property
     @pulumi.getter(name="skipUsers")
     def skip_users(self) -> pulumi.Output[Optional[bool]]:
         """
         Ignore users sync. This is a temporary solution until 'users' field is supported in all the app-like resources
         """
+        warnings.warn("""Because users has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+        pulumi.log.warn("""skip_users is deprecated: Because users has been removed, this attribute is a no op and will be removed""")
+
         return pulumi.get(self, "skip_users")
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/group/role.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/group/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/group/rule.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/group/rule.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/group_memberships.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/group_schema_property.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/group_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/get_metadata_saml.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/idp/get_metadata_saml.py`

 * *Files 11% similar despite different names*

```diff
@@ -168,24 +168,24 @@
     """
     __args__ = dict()
     __args__['idpId'] = idp_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:idp/getMetadataSaml:getMetadataSaml', __args__, opts=opts, typ=GetMetadataSamlResult).value
 
     return AwaitableGetMetadataSamlResult(
-        assertions_signed=__ret__.assertions_signed,
-        authn_request_signed=__ret__.authn_request_signed,
-        encryption_certificate=__ret__.encryption_certificate,
-        entity_id=__ret__.entity_id,
-        http_post_binding=__ret__.http_post_binding,
-        http_redirect_binding=__ret__.http_redirect_binding,
-        id=__ret__.id,
-        idp_id=__ret__.idp_id,
-        metadata=__ret__.metadata,
-        signing_certificate=__ret__.signing_certificate)
+        assertions_signed=pulumi.get(__ret__, 'assertions_signed'),
+        authn_request_signed=pulumi.get(__ret__, 'authn_request_signed'),
+        encryption_certificate=pulumi.get(__ret__, 'encryption_certificate'),
+        entity_id=pulumi.get(__ret__, 'entity_id'),
+        http_post_binding=pulumi.get(__ret__, 'http_post_binding'),
+        http_redirect_binding=pulumi.get(__ret__, 'http_redirect_binding'),
+        id=pulumi.get(__ret__, 'id'),
+        idp_id=pulumi.get(__ret__, 'idp_id'),
+        metadata=pulumi.get(__ret__, 'metadata'),
+        signing_certificate=pulumi.get(__ret__, 'signing_certificate'))
 
 
 @_utilities.lift_output_func(get_metadata_saml)
 def get_metadata_saml_output(idp_id: Optional[pulumi.Input[Optional[str]]] = None,
                              opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetMetadataSamlResult]:
     """
     Use this data source to retrieve SAML IdP metadata from Okta.
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/get_oidc.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/idp/get_oidc.py`

 * *Files 14% similar despite different names*

```diff
@@ -270,32 +270,32 @@
     __args__ = dict()
     __args__['id'] = id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:idp/getOidc:getOidc', __args__, opts=opts, typ=GetOidcResult).value
 
     return AwaitableGetOidcResult(
-        authorization_binding=__ret__.authorization_binding,
-        authorization_url=__ret__.authorization_url,
-        client_id=__ret__.client_id,
-        client_secret=__ret__.client_secret,
-        id=__ret__.id,
-        issuer_mode=__ret__.issuer_mode,
-        issuer_url=__ret__.issuer_url,
-        jwks_binding=__ret__.jwks_binding,
-        jwks_url=__ret__.jwks_url,
-        max_clock_skew=__ret__.max_clock_skew,
-        name=__ret__.name,
-        protocol_type=__ret__.protocol_type,
-        scopes=__ret__.scopes,
-        token_binding=__ret__.token_binding,
-        token_url=__ret__.token_url,
-        type=__ret__.type,
-        user_info_binding=__ret__.user_info_binding,
-        user_info_url=__ret__.user_info_url)
+        authorization_binding=pulumi.get(__ret__, 'authorization_binding'),
+        authorization_url=pulumi.get(__ret__, 'authorization_url'),
+        client_id=pulumi.get(__ret__, 'client_id'),
+        client_secret=pulumi.get(__ret__, 'client_secret'),
+        id=pulumi.get(__ret__, 'id'),
+        issuer_mode=pulumi.get(__ret__, 'issuer_mode'),
+        issuer_url=pulumi.get(__ret__, 'issuer_url'),
+        jwks_binding=pulumi.get(__ret__, 'jwks_binding'),
+        jwks_url=pulumi.get(__ret__, 'jwks_url'),
+        max_clock_skew=pulumi.get(__ret__, 'max_clock_skew'),
+        name=pulumi.get(__ret__, 'name'),
+        protocol_type=pulumi.get(__ret__, 'protocol_type'),
+        scopes=pulumi.get(__ret__, 'scopes'),
+        token_binding=pulumi.get(__ret__, 'token_binding'),
+        token_url=pulumi.get(__ret__, 'token_url'),
+        type=pulumi.get(__ret__, 'type'),
+        user_info_binding=pulumi.get(__ret__, 'user_info_binding'),
+        user_info_url=pulumi.get(__ret__, 'user_info_url'))
 
 
 @_utilities.lift_output_func(get_oidc)
 def get_oidc_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                     name: Optional[pulumi.Input[Optional[str]]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetOidcResult]:
     """
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/get_saml.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/idp/get_saml.py`

 * *Files 5% similar despite different names*

```diff
@@ -219,28 +219,28 @@
     __args__ = dict()
     __args__['id'] = id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:idp/getSaml:getSaml', __args__, opts=opts, typ=GetSamlResult).value
 
     return AwaitableGetSamlResult(
-        acs_binding=__ret__.acs_binding,
-        acs_type=__ret__.acs_type,
-        audience=__ret__.audience,
-        id=__ret__.id,
-        issuer=__ret__.issuer,
-        issuer_mode=__ret__.issuer_mode,
-        kid=__ret__.kid,
-        name=__ret__.name,
-        sso_binding=__ret__.sso_binding,
-        sso_destination=__ret__.sso_destination,
-        sso_url=__ret__.sso_url,
-        subject_filter=__ret__.subject_filter,
-        subject_formats=__ret__.subject_formats,
-        type=__ret__.type)
+        acs_binding=pulumi.get(__ret__, 'acs_binding'),
+        acs_type=pulumi.get(__ret__, 'acs_type'),
+        audience=pulumi.get(__ret__, 'audience'),
+        id=pulumi.get(__ret__, 'id'),
+        issuer=pulumi.get(__ret__, 'issuer'),
+        issuer_mode=pulumi.get(__ret__, 'issuer_mode'),
+        kid=pulumi.get(__ret__, 'kid'),
+        name=pulumi.get(__ret__, 'name'),
+        sso_binding=pulumi.get(__ret__, 'sso_binding'),
+        sso_destination=pulumi.get(__ret__, 'sso_destination'),
+        sso_url=pulumi.get(__ret__, 'sso_url'),
+        subject_filter=pulumi.get(__ret__, 'subject_filter'),
+        subject_formats=pulumi.get(__ret__, 'subject_formats'),
+        type=pulumi.get(__ret__, 'type'))
 
 
 @_utilities.lift_output_func(get_saml)
 def get_saml_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                     name: Optional[pulumi.Input[Optional[str]]] = None,
                     opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSamlResult]:
     """
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/get_social.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/idp/get_social.py`

 * *Files 8% similar despite different names*

```diff
@@ -372,41 +372,41 @@
     __args__ = dict()
     __args__['id'] = id
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:idp/getSocial:getSocial', __args__, opts=opts, typ=GetSocialResult).value
 
     return AwaitableGetSocialResult(
-        account_link_action=__ret__.account_link_action,
-        account_link_group_includes=__ret__.account_link_group_includes,
-        authorization_binding=__ret__.authorization_binding,
-        authorization_url=__ret__.authorization_url,
-        client_id=__ret__.client_id,
-        client_secret=__ret__.client_secret,
-        deprovisioned_action=__ret__.deprovisioned_action,
-        groups_action=__ret__.groups_action,
-        groups_assignments=__ret__.groups_assignments,
-        groups_attribute=__ret__.groups_attribute,
-        groups_filters=__ret__.groups_filters,
-        id=__ret__.id,
-        issuer_mode=__ret__.issuer_mode,
-        max_clock_skew=__ret__.max_clock_skew,
-        name=__ret__.name,
-        profile_master=__ret__.profile_master,
-        protocol_type=__ret__.protocol_type,
-        provisioning_action=__ret__.provisioning_action,
-        scopes=__ret__.scopes,
-        status=__ret__.status,
-        subject_match_attribute=__ret__.subject_match_attribute,
-        subject_match_type=__ret__.subject_match_type,
-        suspended_action=__ret__.suspended_action,
-        token_binding=__ret__.token_binding,
-        token_url=__ret__.token_url,
-        type=__ret__.type,
-        username_template=__ret__.username_template)
+        account_link_action=pulumi.get(__ret__, 'account_link_action'),
+        account_link_group_includes=pulumi.get(__ret__, 'account_link_group_includes'),
+        authorization_binding=pulumi.get(__ret__, 'authorization_binding'),
+        authorization_url=pulumi.get(__ret__, 'authorization_url'),
+        client_id=pulumi.get(__ret__, 'client_id'),
+        client_secret=pulumi.get(__ret__, 'client_secret'),
+        deprovisioned_action=pulumi.get(__ret__, 'deprovisioned_action'),
+        groups_action=pulumi.get(__ret__, 'groups_action'),
+        groups_assignments=pulumi.get(__ret__, 'groups_assignments'),
+        groups_attribute=pulumi.get(__ret__, 'groups_attribute'),
+        groups_filters=pulumi.get(__ret__, 'groups_filters'),
+        id=pulumi.get(__ret__, 'id'),
+        issuer_mode=pulumi.get(__ret__, 'issuer_mode'),
+        max_clock_skew=pulumi.get(__ret__, 'max_clock_skew'),
+        name=pulumi.get(__ret__, 'name'),
+        profile_master=pulumi.get(__ret__, 'profile_master'),
+        protocol_type=pulumi.get(__ret__, 'protocol_type'),
+        provisioning_action=pulumi.get(__ret__, 'provisioning_action'),
+        scopes=pulumi.get(__ret__, 'scopes'),
+        status=pulumi.get(__ret__, 'status'),
+        subject_match_attribute=pulumi.get(__ret__, 'subject_match_attribute'),
+        subject_match_type=pulumi.get(__ret__, 'subject_match_type'),
+        suspended_action=pulumi.get(__ret__, 'suspended_action'),
+        token_binding=pulumi.get(__ret__, 'token_binding'),
+        token_url=pulumi.get(__ret__, 'token_url'),
+        type=pulumi.get(__ret__, 'type'),
+        username_template=pulumi.get(__ret__, 'username_template'))
 
 
 @_utilities.lift_output_func(get_social)
 def get_social_output(id: Optional[pulumi.Input[Optional[str]]] = None,
                       name: Optional[pulumi.Input[Optional[str]]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetSocialResult]:
     """
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/oidc.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/idp/oidc.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/saml.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/idp/saml.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/saml_key.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/idp/saml_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/idp/social.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/idp/social.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/index/_inputs.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/index/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/index/email_domain.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/index/email_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/index/email_domain_verification.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/index/email_domain_verification.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/index/get_domain.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/index/get_domain.py`

 * *Files 4% similar despite different names*

```diff
@@ -138,21 +138,21 @@
     """
     __args__ = dict()
     __args__['domainIdOrName'] = domain_id_or_name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:Index/getDomain:getDomain', __args__, opts=opts, typ=GetDomainResult).value
 
     return AwaitableGetDomainResult(
-        certificate_source_type=__ret__.certificate_source_type,
-        dns_records=__ret__.dns_records,
-        domain=__ret__.domain,
-        domain_id_or_name=__ret__.domain_id_or_name,
-        id=__ret__.id,
-        public_certificate=__ret__.public_certificate,
-        validation_status=__ret__.validation_status)
+        certificate_source_type=pulumi.get(__ret__, 'certificate_source_type'),
+        dns_records=pulumi.get(__ret__, 'dns_records'),
+        domain=pulumi.get(__ret__, 'domain'),
+        domain_id_or_name=pulumi.get(__ret__, 'domain_id_or_name'),
+        id=pulumi.get(__ret__, 'id'),
+        public_certificate=pulumi.get(__ret__, 'public_certificate'),
+        validation_status=pulumi.get(__ret__, 'validation_status'))
 
 
 @_utilities.lift_output_func(get_domain)
 def get_domain_output(domain_id_or_name: Optional[pulumi.Input[str]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDomainResult]:
     """
     Use this data source to retrieve a domain from Okta.
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/index/outputs.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/index/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/inline/_inputs.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/inline/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/inline/hook.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/inline/hook.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/inline/outputs.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/inline/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/link_definition.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/link_definition.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/link_value.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/link_value.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/network/zone.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/network/zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/org_configuration.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/org_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/org_support.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/org_support.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/outputs.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,30 +99,30 @@
         return super().get(key, default)
 
     def __init__(__self__, *,
                  os_expression: Optional[str] = None,
                  os_type: Optional[str] = None,
                  type: Optional[str] = None):
         """
-        :param str os_expression: Only available when using `os_type = "OTHER"`
+        :param str os_expression: Only available and required when using `os_type = "OTHER"`
         :param str os_type: One of: `"ANY"`, `"IOS"`, `"WINDOWS"`, `"ANDROID"`, `"OTHER"`, `"OSX"`, `"MACOS"`
         :param str type: The Verification Method type. It can be set to `"ASSURANCE"`. Default is `"ASSURANCE"`.
         """
         if os_expression is not None:
             pulumi.set(__self__, "os_expression", os_expression)
         if os_type is not None:
             pulumi.set(__self__, "os_type", os_type)
         if type is not None:
             pulumi.set(__self__, "type", type)
 
     @property
     @pulumi.getter(name="osExpression")
     def os_expression(self) -> Optional[str]:
         """
-        Only available when using `os_type = "OTHER"`
+        Only available and required when using `os_type = "OTHER"`
         """
         return pulumi.get(self, "os_expression")
 
     @property
     @pulumi.getter(name="osType")
     def os_type(self) -> Optional[str]:
         """
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/__init__.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/_inputs.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/get_default_policy.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/get_default_policy.py`

 * *Files 12% similar despite different names*

```diff
@@ -76,16 +76,16 @@
     """
     __args__ = dict()
     __args__['type'] = type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:policy/getDefaultPolicy:getDefaultPolicy', __args__, opts=opts, typ=GetDefaultPolicyResult).value
 
     return AwaitableGetDefaultPolicyResult(
-        id=__ret__.id,
-        type=__ret__.type)
+        id=pulumi.get(__ret__, 'id'),
+        type=pulumi.get(__ret__, 'type'))
 
 
 @_utilities.lift_output_func(get_default_policy)
 def get_default_policy_output(type: Optional[pulumi.Input[str]] = None,
                               opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetDefaultPolicyResult]:
     """
     Use this data source to retrieve a default policy from Okta. This same thing can be achieved using the `policy_get_policy` with default names, this is simply a shortcut.
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/get_policy.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/get_policy.py`

 * *Files 6% similar despite different names*

```diff
@@ -101,18 +101,18 @@
     __args__ = dict()
     __args__['name'] = name
     __args__['type'] = type
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:policy/getPolicy:getPolicy', __args__, opts=opts, typ=GetPolicyResult).value
 
     return AwaitableGetPolicyResult(
-        id=__ret__.id,
-        name=__ret__.name,
-        status=__ret__.status,
-        type=__ret__.type)
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        status=pulumi.get(__ret__, 'status'),
+        type=pulumi.get(__ret__, 'type'))
 
 
 @_utilities.lift_output_func(get_policy)
 def get_policy_output(name: Optional[pulumi.Input[str]] = None,
                       type: Optional[pulumi.Input[str]] = None,
                       opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetPolicyResult]:
     """
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/mfa.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/mfa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/outputs.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/password.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/password.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/rule_idp_discovery.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/rule_idp_discovery.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/rule_mfa.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/rule_mfa.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/rule_password.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/rule_password.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/rule_signon.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/rule_signon.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy/signon.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/policy/signon.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy_mfa_default.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/policy_mfa_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy_password_default.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/policy_password_default.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy_profile_enrollment.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/policy_profile_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy_profile_enrollment_apps.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/policy_profile_enrollment_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/policy_rule_profile_enrollment.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/policy_rule_profile_enrollment.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/profile/_inputs.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/profile/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/profile/mapping.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/profile/mapping.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/profile/outputs.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/profile/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/provider.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/rate_limiting.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/resource_set.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/resource_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/role_subscription.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/role_subscription.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/security_notification_emails.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/security_notification_emails.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/template_sms.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/template_sms.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/theme.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/theme.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/threat_insight_settings.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/threat_insight_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/trustedorigin/origin.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/trustedorigin/origin.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/user/_inputs.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/user/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/user/get_user.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/user/get_user.py`

 * *Files 7% similar despite different names*

```diff
@@ -560,57 +560,57 @@
     __args__['skipGroups'] = skip_groups
     __args__['skipRoles'] = skip_roles
     __args__['userId'] = user_id
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:user/getUser:getUser', __args__, opts=opts, typ=GetUserResult).value
 
     return AwaitableGetUserResult(
-        admin_roles=__ret__.admin_roles,
-        city=__ret__.city,
-        compound_search_operator=__ret__.compound_search_operator,
-        cost_center=__ret__.cost_center,
-        country_code=__ret__.country_code,
-        custom_profile_attributes=__ret__.custom_profile_attributes,
-        delay_read_seconds=__ret__.delay_read_seconds,
-        department=__ret__.department,
-        display_name=__ret__.display_name,
-        division=__ret__.division,
-        email=__ret__.email,
-        employee_number=__ret__.employee_number,
-        first_name=__ret__.first_name,
-        group_memberships=__ret__.group_memberships,
-        honorific_prefix=__ret__.honorific_prefix,
-        honorific_suffix=__ret__.honorific_suffix,
-        id=__ret__.id,
-        last_name=__ret__.last_name,
-        locale=__ret__.locale,
-        login=__ret__.login,
-        manager=__ret__.manager,
-        manager_id=__ret__.manager_id,
-        middle_name=__ret__.middle_name,
-        mobile_phone=__ret__.mobile_phone,
-        nick_name=__ret__.nick_name,
-        organization=__ret__.organization,
-        postal_address=__ret__.postal_address,
-        preferred_language=__ret__.preferred_language,
-        primary_phone=__ret__.primary_phone,
-        profile_url=__ret__.profile_url,
-        roles=__ret__.roles,
-        searches=__ret__.searches,
-        second_email=__ret__.second_email,
-        skip_groups=__ret__.skip_groups,
-        skip_roles=__ret__.skip_roles,
-        state=__ret__.state,
-        status=__ret__.status,
-        street_address=__ret__.street_address,
-        timezone=__ret__.timezone,
-        title=__ret__.title,
-        user_id=__ret__.user_id,
-        user_type=__ret__.user_type,
-        zip_code=__ret__.zip_code)
+        admin_roles=pulumi.get(__ret__, 'admin_roles'),
+        city=pulumi.get(__ret__, 'city'),
+        compound_search_operator=pulumi.get(__ret__, 'compound_search_operator'),
+        cost_center=pulumi.get(__ret__, 'cost_center'),
+        country_code=pulumi.get(__ret__, 'country_code'),
+        custom_profile_attributes=pulumi.get(__ret__, 'custom_profile_attributes'),
+        delay_read_seconds=pulumi.get(__ret__, 'delay_read_seconds'),
+        department=pulumi.get(__ret__, 'department'),
+        display_name=pulumi.get(__ret__, 'display_name'),
+        division=pulumi.get(__ret__, 'division'),
+        email=pulumi.get(__ret__, 'email'),
+        employee_number=pulumi.get(__ret__, 'employee_number'),
+        first_name=pulumi.get(__ret__, 'first_name'),
+        group_memberships=pulumi.get(__ret__, 'group_memberships'),
+        honorific_prefix=pulumi.get(__ret__, 'honorific_prefix'),
+        honorific_suffix=pulumi.get(__ret__, 'honorific_suffix'),
+        id=pulumi.get(__ret__, 'id'),
+        last_name=pulumi.get(__ret__, 'last_name'),
+        locale=pulumi.get(__ret__, 'locale'),
+        login=pulumi.get(__ret__, 'login'),
+        manager=pulumi.get(__ret__, 'manager'),
+        manager_id=pulumi.get(__ret__, 'manager_id'),
+        middle_name=pulumi.get(__ret__, 'middle_name'),
+        mobile_phone=pulumi.get(__ret__, 'mobile_phone'),
+        nick_name=pulumi.get(__ret__, 'nick_name'),
+        organization=pulumi.get(__ret__, 'organization'),
+        postal_address=pulumi.get(__ret__, 'postal_address'),
+        preferred_language=pulumi.get(__ret__, 'preferred_language'),
+        primary_phone=pulumi.get(__ret__, 'primary_phone'),
+        profile_url=pulumi.get(__ret__, 'profile_url'),
+        roles=pulumi.get(__ret__, 'roles'),
+        searches=pulumi.get(__ret__, 'searches'),
+        second_email=pulumi.get(__ret__, 'second_email'),
+        skip_groups=pulumi.get(__ret__, 'skip_groups'),
+        skip_roles=pulumi.get(__ret__, 'skip_roles'),
+        state=pulumi.get(__ret__, 'state'),
+        status=pulumi.get(__ret__, 'status'),
+        street_address=pulumi.get(__ret__, 'street_address'),
+        timezone=pulumi.get(__ret__, 'timezone'),
+        title=pulumi.get(__ret__, 'title'),
+        user_id=pulumi.get(__ret__, 'user_id'),
+        user_type=pulumi.get(__ret__, 'user_type'),
+        zip_code=pulumi.get(__ret__, 'zip_code'))
 
 
 @_utilities.lift_output_func(get_user)
 def get_user_output(compound_search_operator: Optional[pulumi.Input[Optional[str]]] = None,
                     delay_read_seconds: Optional[pulumi.Input[Optional[str]]] = None,
                     searches: Optional[pulumi.Input[Optional[Sequence[pulumi.InputType['GetUserSearchArgs']]]]] = None,
                     skip_groups: Optional[pulumi.Input[Optional[bool]]] = None,
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/user/get_user_profile_mapping_source.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/user/get_user_profile_mapping_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,10 +83,10 @@
     ```
     """
     __args__ = dict()
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:user/getUserProfileMappingSource:getUserProfileMappingSource', __args__, opts=opts, typ=GetUserProfileMappingSourceResult).value
 
     return AwaitableGetUserProfileMappingSourceResult(
-        id=__ret__.id,
-        name=__ret__.name,
-        type=__ret__.type)
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'),
+        type=pulumi.get(__ret__, 'type'))
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/user/get_user_type.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/user/get_user_type.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,18 +99,18 @@
     """
     __args__ = dict()
     __args__['name'] = name
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:user/getUserType:getUserType', __args__, opts=opts, typ=GetUserTypeResult).value
 
     return AwaitableGetUserTypeResult(
-        description=__ret__.description,
-        display_name=__ret__.display_name,
-        id=__ret__.id,
-        name=__ret__.name)
+        description=pulumi.get(__ret__, 'description'),
+        display_name=pulumi.get(__ret__, 'display_name'),
+        id=pulumi.get(__ret__, 'id'),
+        name=pulumi.get(__ret__, 'name'))
 
 
 @_utilities.lift_output_func(get_user_type)
 def get_user_type_output(name: Optional[pulumi.Input[str]] = None,
                          opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetUserTypeResult]:
     """
     Use this data source to retrieve a user type from Okta.
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/user/get_users.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/user/get_users.py`

 * *Files 9% similar despite different names*

```diff
@@ -159,22 +159,22 @@
     __args__['includeGroups'] = include_groups
     __args__['includeRoles'] = include_roles
     __args__['searches'] = searches
     opts = pulumi.InvokeOptions.merge(_utilities.get_invoke_opts_defaults(), opts)
     __ret__ = pulumi.runtime.invoke('okta:user/getUsers:getUsers', __args__, opts=opts, typ=GetUsersResult).value
 
     return AwaitableGetUsersResult(
-        compound_search_operator=__ret__.compound_search_operator,
-        delay_read_seconds=__ret__.delay_read_seconds,
-        group_id=__ret__.group_id,
-        id=__ret__.id,
-        include_groups=__ret__.include_groups,
-        include_roles=__ret__.include_roles,
-        searches=__ret__.searches,
-        users=__ret__.users)
+        compound_search_operator=pulumi.get(__ret__, 'compound_search_operator'),
+        delay_read_seconds=pulumi.get(__ret__, 'delay_read_seconds'),
+        group_id=pulumi.get(__ret__, 'group_id'),
+        id=pulumi.get(__ret__, 'id'),
+        include_groups=pulumi.get(__ret__, 'include_groups'),
+        include_roles=pulumi.get(__ret__, 'include_roles'),
+        searches=pulumi.get(__ret__, 'searches'),
+        users=pulumi.get(__ret__, 'users'))
 
 
 @_utilities.lift_output_func(get_users)
 def get_users_output(compound_search_operator: Optional[pulumi.Input[Optional[str]]] = None,
                      delay_read_seconds: Optional[pulumi.Input[Optional[str]]] = None,
                      group_id: Optional[pulumi.Input[Optional[str]]] = None,
                      include_groups: Optional[pulumi.Input[Optional[bool]]] = None,
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/user/outputs.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/user/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/user/user.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/user/user.py`

 * *Files 2% similar despite different names*

```diff
@@ -615,14 +615,17 @@
 
     @property
     @pulumi.getter(name="skipRoles")
     def skip_roles(self) -> Optional[pulumi.Input[bool]]:
         """
         Do not populate user roles information (prevents additional API call)
         """
+        warnings.warn("""Because admin_roles has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+        pulumi.log.warn("""skip_roles is deprecated: Because admin_roles has been removed, this attribute is a no op and will be removed""")
+
         return pulumi.get(self, "skip_roles")
 
     @skip_roles.setter
     def skip_roles(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "skip_roles", value)
 
     @property
@@ -1332,14 +1335,17 @@
 
     @property
     @pulumi.getter(name="skipRoles")
     def skip_roles(self) -> Optional[pulumi.Input[bool]]:
         """
         Do not populate user roles information (prevents additional API call)
         """
+        warnings.warn("""Because admin_roles has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+        pulumi.log.warn("""skip_roles is deprecated: Because admin_roles has been removed, this attribute is a no op and will be removed""")
+
         return pulumi.get(self, "skip_roles")
 
     @skip_roles.setter
     def skip_roles(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "skip_roles", value)
 
     @property
@@ -2248,14 +2254,17 @@
 
     @property
     @pulumi.getter(name="skipRoles")
     def skip_roles(self) -> pulumi.Output[Optional[bool]]:
         """
         Do not populate user roles information (prevents additional API call)
         """
+        warnings.warn("""Because admin_roles has been removed, this attribute is a no op and will be removed""", DeprecationWarning)
+        pulumi.log.warn("""skip_roles is deprecated: Because admin_roles has been removed, this attribute is a no op and will be removed""")
+
         return pulumi.get(self, "skip_roles")
 
     @property
     @pulumi.getter
     def state(self) -> pulumi.Output[Optional[str]]:
         """
         User profile property.
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/user/user_type.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/user/user_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/user_admin_roles.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/user_admin_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/user_base_schema_property.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/user_base_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/user_factor_question.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/user_factor_question.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/user_group_memberships.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/user_group_memberships.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta/user_schema_property.py` & `pulumi_okta-4.1.0a1689006772/pulumi_okta/user_schema_property.py`

 * *Files identical despite different names*

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta.egg-info/PKG-INFO` & `pulumi_okta-4.1.0a1689006772/pulumi_okta.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-okta
-Version: 4.1.0a1687800548
+Version: 4.1.0a1689006772
 Summary: A Pulumi package for creating and managing okta resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-okta
 Keywords: pulumi okta
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_okta-4.1.0a1687800548/pulumi_okta.egg-info/SOURCES.txt` & `pulumi_okta-4.1.0a1689006772/pulumi_okta.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -117,14 +117,15 @@
 pulumi_okta/config/__init__.py
 pulumi_okta/config/vars.py
 pulumi_okta/factor/__init__.py
 pulumi_okta/factor/factor.py
 pulumi_okta/group/__init__.py
 pulumi_okta/group/get_everyone_group.py
 pulumi_okta/group/get_group.py
+pulumi_okta/group/get_rule.py
 pulumi_okta/group/group.py
 pulumi_okta/group/role.py
 pulumi_okta/group/rule.py
 pulumi_okta/idp/__init__.py
 pulumi_okta/idp/get_metadata_saml.py
 pulumi_okta/idp/get_oidc.py
 pulumi_okta/idp/get_saml.py
```

### Comparing `pulumi_okta-4.1.0a1687800548/setup.py` & `pulumi_okta-4.1.0a1689006772/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.1.0a1687800548"
-PLUGIN_VERSION = "4.1.0-alpha.1687800548+cc3da24f"
+VERSION = "4.1.0a1689006772"
+PLUGIN_VERSION = "4.1.0-alpha.1689006772+cddfceea"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'okta', PLUGIN_VERSION])
         except OSError as error:
```

