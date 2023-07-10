# Comparing `tmp/awsibox-0.8.7.tar.gz` & `tmp/awsibox-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awsibox-0.8.7.tar", last modified: Fri Jun 16 09:29:31 2023, max compression
+gzip compressed data, was "awsibox-0.8.8.tar", last modified: Mon Jul 10 13:54:48 2023, max compression
```

## Comparing `awsibox-0.8.7.tar` & `awsibox-0.8.8.tar`

### file list

```diff
@@ -1,276 +1,286 @@
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.393291 awsibox-0.8.7/
--rw-r--r--   0 mello     (1000) mello     (1000)      771 2020-01-23 17:57:57.000000 awsibox-0.8.7/.gitignore
--rw-r--r--   0 mello     (1000) mello     (1000)      257 2023-06-16 08:09:06.000000 awsibox-0.8.7/MANIFEST.in
--rw-r--r--   0 mello     (1000) mello     (1000)     1014 2023-06-16 09:29:31.393291 awsibox-0.8.7/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)      373 2022-03-14 08:29:15.000000 awsibox-0.8.7/README.md
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.277289 awsibox-0.8.7/awsibox/
--rw-r--r--   0 mello     (1000) mello     (1000)    19452 2023-06-15 12:57:11.000000 awsibox-0.8.7/awsibox/RP.py
--rw-r--r--   0 mello     (1000) mello     (1000)       39 2023-06-16 09:28:20.000000 awsibox-0.8.7/awsibox/__init__.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2251 2022-07-01 08:39:37.000000 awsibox-0.8.7/awsibox/args.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.281289 awsibox-0.8.7/awsibox/aws/
--rw-r--r--   0 mello     (1000) mello     (1000)  7094944 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/aws/CloudFormationResourceSpecification.json
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.265289 awsibox-0.8.7/awsibox/cfg/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.273289 awsibox-0.8.7/awsibox/cfg/ibox/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.313290 awsibox-0.8.7/awsibox/cfg/ibox/com/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.317290 awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/
--rw-r--r--   0 mello     (1000) mello     (1000)      534 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/capacity.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      459 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/cloudwatch-agent.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1252 2023-06-16 09:13:11.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1357 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1303 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2303 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2934 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2206 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.321290 awsibox-0.8.7/awsibox/cfg/ibox/com/certificatemanager/
--rw-r--r--   0 mello     (1000) mello     (1000)     1222 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.321290 awsibox-0.8.7/awsibox/cfg/ibox/com/cloudformation/
--rw-r--r--   0 mello     (1000) mello     (1000)      658 2023-06-06 14:25:53.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/cloudformation/custom-resource_light-house.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.321290 awsibox-0.8.7/awsibox/cfg/ibox/com/cloudfront/
--rw-r--r--   0 mello     (1000) mello     (1000)     1521 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1656 2023-06-14 15:23:58.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/cloudfront/for-services.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      121 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/cloudfront/i_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      495 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/cloudfront/origin-adhoc.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.321290 awsibox-0.8.7/awsibox/cfg/ibox/com/codedeploy/
--rw-r--r--   0 mello     (1000) mello     (1000)      190 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/codedeploy/deployment-group.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1810 2023-06-16 09:12:56.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/common.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.321290 awsibox-0.8.7/awsibox/cfg/ibox/com/dynamodb/
--rw-r--r--   0 mello     (1000) mello     (1000)      579 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.325290 awsibox-0.8.7/awsibox/cfg/ibox/com/ec2/
--rw-r--r--   0 mello     (1000) mello     (1000)     1975 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ec2/bottlerocket.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      265 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ec2/securitygroup.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      672 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.329290 awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/
--rw-r--r--   0 mello     (1000) mello     (1000)     2452 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/capacityprovider.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1414 2023-06-14 16:05:45.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1518 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/fargate-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3140 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      703 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     6894 2023-06-14 16:14:09.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      899 2023-06-14 16:05:02.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/task.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      399 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/taskdefinition-volume.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.329290 awsibox-0.8.7/awsibox/cfg/ibox/com/efs/
--rw-r--r--   0 mello     (1000) mello     (1000)      378 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/efs/accesspoint-app.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.329290 awsibox-0.8.7/awsibox/cfg/ibox/com/elasticloadbalancing/
--rw-r--r--   0 mello     (1000) mello     (1000)     1287 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2246 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1945 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      242 2023-06-14 15:18:04.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/elasticloadbalancing/i_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      201 2023-06-14 16:13:04.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/elasticloadbalancing/loadbalancer.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      194 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/elasticloadbalancing/v2-listener.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.333290 awsibox-0.8.7/awsibox/cfg/ibox/com/events/
--rw-r--r--   0 mello     (1000) mello     (1000)     2892 2023-05-01 13:36:02.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1340 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/events/cluster-autoscale.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     6914 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/events/ec2.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1581 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2584 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/events/ecs-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1570 2023-05-01 13:33:03.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/events/ecs.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1203 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/events/spot_advisor.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.333290 awsibox-0.8.7/awsibox/cfg/ibox/com/iam/
--rw-r--r--   0 mello     (1000) mello     (1000)     5020 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/iam/managed-policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      435 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/iam/policy-ecs-exec.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      939 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2115 2023-05-18 13:24:47.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/iam/policy-update_stack.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1591 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1939 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/iam/roles.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.337290 awsibox-0.8.7/awsibox/cfg/ibox/com/kms/
--rw-r--r--   0 mello     (1000) mello     (1000)      684 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.337290 awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/
--rw-r--r--   0 mello     (1000) mello     (1000)      607 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3732 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1393 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       46 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/layers.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      935 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/py-packager.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1204 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/service-unavailable.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.341291 awsibox-0.8.7/awsibox/cfg/ibox/com/route53/
--rw-r--r--   0 mello     (1000) mello     (1000)      428 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/route53/resolverendpoint-outbound.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.341291 awsibox-0.8.7/awsibox/cfg/ibox/com/s3/
--rw-r--r--   0 mello     (1000) mello     (1000)      513 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/s3/bucket-log.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.341291 awsibox-0.8.7/awsibox/cfg/ibox/com/servicediscovery/
--rw-r--r--   0 mello     (1000) mello     (1000)      374 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/servicediscovery/publicdnsnamespace-find.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.341291 awsibox-0.8.7/awsibox/cfg/ibox/com/sns/
--rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      225 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/sns/cloudwatch-alarm.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.341291 awsibox-0.8.7/awsibox/cfg/ibox/com/ssm/
--rw-r--r--   0 mello     (1000) mello     (1000)      312 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/com/ssm/parameter-user-password.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.273289 awsibox-0.8.7/awsibox/cfg/ibox/res/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.341291 awsibox-0.8.7/awsibox/cfg/ibox/res/apigateway/
--rw-r--r--   0 mello     (1000) mello     (1000)      147 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/apigateway/accounts.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      250 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/apigateway/deployments.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      491 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/apigateway/domain-names.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1821 2023-06-14 15:29:04.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/apigateway/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.345291 awsibox-0.8.7/awsibox/cfg/ibox/res/application-autoscaling/
--rw-r--r--   0 mello     (1000) mello     (1000)      832 2023-06-14 15:40:34.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2965 2023-06-14 15:41:11.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2143 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.345291 awsibox-0.8.7/awsibox/cfg/ibox/res/autoscaling/
--rw-r--r--   0 mello     (1000) mello     (1000)     2402 2023-06-14 15:45:22.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3163 2023-06-14 15:45:28.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     5137 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1889 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.345291 awsibox-0.8.7/awsibox/cfg/ibox/res/certificatemanager/
--rw-r--r--   0 mello     (1000) mello     (1000)      222 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/certificatemanager/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.349291 awsibox-0.8.7/awsibox/cfg/ibox/res/cloudfront/
--rw-r--r--   0 mello     (1000) mello     (1000)     4829 2023-06-14 15:51:31.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      243 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/cloudfront/origin-access-identities.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     5958 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/cloudfront/policies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.349291 awsibox-0.8.7/awsibox/cfg/ibox/res/cloudwatch/
--rw-r--r--   0 mello     (1000) mello     (1000)     7727 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/cloudwatch/alarms.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1041 2023-06-14 15:57:15.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      966 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.349291 awsibox-0.8.7/awsibox/cfg/ibox/res/codedeploy/
--rw-r--r--   0 mello     (1000) mello     (1000)      364 2023-06-14 16:02:37.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/codedeploy/deployment-groups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1081 2023-06-14 16:01:55.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.349291 awsibox-0.8.7/awsibox/cfg/ibox/res/ec2/
--rw-r--r--   0 mello     (1000) mello     (1000)      160 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/ec2/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      118 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/ec2/vpc-endpoints.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.349291 awsibox-0.8.7/awsibox/cfg/ibox/res/ecr/
--rw-r--r--   0 mello     (1000) mello     (1000)      136 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/ecr/accounts.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1405 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/ecr/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.353291 awsibox-0.8.7/awsibox/cfg/ibox/res/ecs/
--rw-r--r--   0 mello     (1000) mello     (1000)     9924 2023-06-14 16:06:44.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/ecs/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1964 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/ecs/services.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1021 2023-06-06 14:25:53.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.353291 awsibox-0.8.7/awsibox/cfg/ibox/res/efs/
--rw-r--r--   0 mello     (1000) mello     (1000)       68 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/efs/filesystems.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      561 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/efs/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.353291 awsibox-0.8.7/awsibox/cfg/ibox/res/elasticache/
--rw-r--r--   0 mello     (1000) mello     (1000)     5327 2023-05-31 09:04:53.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/elasticache/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       69 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/elasticache/subnet-groups.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.357291 awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/
--rw-r--r--   0 mello     (1000) mello     (1000)     4187 2023-06-14 16:14:27.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     4552 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/listeners.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1002 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2831 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2962 2023-06-06 14:25:53.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.357291 awsibox-0.8.7/awsibox/cfg/ibox/res/events/
--rw-r--r--   0 mello     (1000) mello     (1000)     1765 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/events/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.357291 awsibox-0.8.7/awsibox/cfg/ibox/res/iam/
--rw-r--r--   0 mello     (1000) mello     (1000)     2364 2023-06-14 16:17:13.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/iam/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      143 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/iam/instance-profiles.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3687 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/iam/managed-policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1716 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/iam/policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      918 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/iam/roles.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.357291 awsibox-0.8.7/awsibox/cfg/ibox/res/lambda/
--rw-r--r--   0 mello     (1000) mello     (1000)     1286 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/lambda/functions.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2591 2023-06-14 16:23:01.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/lambda/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      213 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/lambda/layer_permissions.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      938 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/lambda/permissions.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      586 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/lambda/versions.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.361291 awsibox-0.8.7/awsibox/cfg/ibox/res/rds/
--rw-r--r--   0 mello     (1000) mello     (1000)      393 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/rds/db-subnet-groups.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     8105 2023-05-10 15:52:15.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/rds/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.361291 awsibox-0.8.7/awsibox/cfg/ibox/res/route53/
--rw-r--r--   0 mello     (1000) mello     (1000)     1427 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/route53/hostedzones.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      410 2023-06-14 15:15:46.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/route53/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     7638 2023-06-14 15:16:13.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/route53/recordsets.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.361291 awsibox-0.8.7/awsibox/cfg/ibox/res/s3/
--rw-r--r--   0 mello     (1000) mello     (1000)     2808 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/s3/bucket-policies.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     8088 2023-06-15 07:52:15.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/s3/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.361291 awsibox-0.8.7/awsibox/cfg/ibox/res/scheduler/
--rw-r--r--   0 mello     (1000) mello     (1000)     1487 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/scheduler/ibox_base.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.361291 awsibox-0.8.7/awsibox/cfg/ibox/res/sns/
--rw-r--r--   0 mello     (1000) mello     (1000)      449 2023-06-14 16:29:21.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/sns/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      719 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/sns/subscriptions.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.365291 awsibox-0.8.7/awsibox/cfg/ibox/res/sqs/
--rw-r--r--   0 mello     (1000) mello     (1000)      467 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/sqs/ibox_base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      978 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/res/sqs/queue-policies.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.273289 awsibox-0.8.7/awsibox/cfg/ibox/stacks/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.365291 awsibox-0.8.7/awsibox/cfg/ibox/stacks/agw/
--rw-r--r--   0 mello     (1000) mello     (1000)     1690 2023-06-14 15:29:08.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/agw/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2612 2023-04-27 10:02:55.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/agw/infra-info.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.365291 awsibox-0.8.7/awsibox/cfg/ibox/stacks/cch/
--rw-r--r--   0 mello     (1000) mello     (1000)      280 2023-06-14 15:24:02.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/cch/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.365291 awsibox-0.8.7/awsibox/cfg/ibox/stacks/clf/
--rw-r--r--   0 mello     (1000) mello     (1000)       89 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/clf/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.365291 awsibox-0.8.7/awsibox/cfg/ibox/stacks/ec2/
--rw-r--r--   0 mello     (1000) mello     (1000)     4594 2023-05-11 09:07:31.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3294 2023-06-15 07:55:39.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/ec2/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.369291 awsibox-0.8.7/awsibox/cfg/ibox/stacks/ecs/
--rw-r--r--   0 mello     (1000) mello     (1000)      839 2023-06-15 07:56:29.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/ecs/buildkite.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2378 2023-06-14 16:05:52.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/ecs/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      690 2023-06-15 07:55:51.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.369291 awsibox-0.8.7/awsibox/cfg/ibox/stacks/lbd/
--rw-r--r--   0 mello     (1000) mello     (1000)     1291 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.369291 awsibox-0.8.7/awsibox/cfg/ibox/stacks/rds/
--rw-r--r--   0 mello     (1000) mello     (1000)      209 2023-06-14 15:24:08.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/rds/i_type.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.373291 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/
--rw-r--r--   0 mello     (1000) mello     (1000)      633 2023-06-15 07:57:04.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-base.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     1543 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      794 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     3497 2023-06-14 15:55:04.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      139 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-event-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      559 2023-06-16 09:17:19.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-extra-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      910 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     4645 2023-06-14 16:16:30.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      108 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-iam-user-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)      655 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)       29 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-s3-01.yml
--rw-r--r--   0 mello     (1000) mello     (1000)     2152 2023-06-16 09:17:10.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/vpc.yml
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.373291 awsibox-0.8.7/awsibox/cfg/ibox/stacks/tsk/
--rw-r--r--   0 mello     (1000) mello     (1000)     2459 2023-06-14 16:36:55.000000 awsibox-0.8.7/awsibox/cfg/ibox/stacks/tsk/i_type.yml
--rw-r--r--   0 mello     (1000) mello     (1000)    16806 2023-06-16 09:12:22.000000 awsibox-0.8.7/awsibox/cfg.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1685 2023-04-17 10:03:18.000000 awsibox-0.8.7/awsibox/common.py
--rw-r--r--   0 mello     (1000) mello     (1000)     1867 2023-04-27 09:19:18.000000 awsibox-0.8.7/awsibox/discover.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2407 2023-06-16 09:27:54.000000 awsibox-0.8.7/awsibox/generate.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.385291 awsibox-0.8.7/awsibox/lambdas/
--rw-r--r--   0 mello     (1000) mello     (1000)     1687 2022-03-14 08:29:15.000000 awsibox-0.8.7/awsibox/lambdas/ASGSpot.code
--rw-r--r--   0 mello     (1000) mello     (1000)      812 2022-03-14 08:29:15.000000 awsibox-0.8.7/awsibox/lambdas/AtEdgeAddHeaders.code
--rw-r--r--   0 mello     (1000) mello     (1000)     4293 2023-04-11 07:34:58.000000 awsibox-0.8.7/awsibox/lambdas/CCRFargateSpot.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2759 2022-11-22 10:02:17.000000 awsibox-0.8.7/awsibox/lambdas/CCRLightHouse.code
--rw-r--r--   0 mello     (1000) mello     (1000)     3916 2023-04-11 07:35:07.000000 awsibox-0.8.7/awsibox/lambdas/CCRStackReplicator.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2115 2022-11-22 13:27:14.000000 awsibox-0.8.7/awsibox/lambdas/CloudWatchAlarmStateChange.code
--rw-r--r--   0 mello     (1000) mello     (1000)     1675 2022-11-22 13:26:46.000000 awsibox-0.8.7/awsibox/lambdas/CloudWatchRepeatedNotify.code
--rw-r--r--   0 mello     (1000) mello     (1000)      739 2022-03-14 08:29:15.000000 awsibox-0.8.7/awsibox/lambdas/EC2StartStopTagged.code
--rwxr-xr-x   0 mello     (1000) mello     (1000)     6507 2022-11-30 10:37:32.000000 awsibox-0.8.7/awsibox/lambdas/ECSClusterAutoscale.code
--rw-r--r--   0 mello     (1000) mello     (1000)     6697 2022-11-29 16:18:45.000000 awsibox-0.8.7/awsibox/lambdas/ECSDrainInstance.code
--rw-r--r--   0 mello     (1000) mello     (1000)     7111 2023-04-17 15:59:09.000000 awsibox-0.8.7/awsibox/lambdas/ECSDrainTasks.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2899 2022-11-22 15:41:37.000000 awsibox-0.8.7/awsibox/lambdas/ECSEventTaskStateChange.code
--rw-r--r--   0 mello     (1000) mello     (1000)     4193 2023-04-12 09:41:12.000000 awsibox-0.8.7/awsibox/lambdas/ECSEventsSpot.code
--rw-r--r--   0 mello     (1000) mello     (1000)     6177 2023-04-12 10:46:40.000000 awsibox-0.8.7/awsibox/lambdas/ECSRaiseASGAlarm.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2792 2022-11-30 13:18:45.000000 awsibox-0.8.7/awsibox/lambdas/ECSRunTask.code
--rw-r--r--   0 mello     (1000) mello     (1000)      987 2022-03-14 08:29:15.000000 awsibox-0.8.7/awsibox/lambdas/ECSUpdateDesiredCount.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2167 2022-03-14 08:29:15.000000 awsibox-0.8.7/awsibox/lambdas/ElasticSearchSnapShot.code
--rwxr-xr-x   0 mello     (1000) mello     (1000)     5370 2023-06-07 12:49:30.000000 awsibox-0.8.7/awsibox/lambdas/InfraInfo.code
--rw-r--r--   0 mello     (1000) mello     (1000)     1267 2022-04-23 16:11:28.000000 awsibox-0.8.7/awsibox/lambdas/ManageService.code
--rw-r--r--   0 mello     (1000) mello     (1000)      547 2022-03-14 08:29:15.000000 awsibox-0.8.7/awsibox/lambdas/PaidApi.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2724 2023-04-07 09:45:45.000000 awsibox-0.8.7/awsibox/lambdas/PyPackager.code
--rw-r--r--   0 mello     (1000) mello     (1000)      844 2022-03-14 08:29:15.000000 awsibox-0.8.7/awsibox/lambdas/Python37SSM.layer
--rw-r--r--   0 mello     (1000) mello     (1000)     3826 2022-11-30 13:32:53.000000 awsibox-0.8.7/awsibox/lambdas/R53RecordInstanceId.code
--rw-r--r--   0 mello     (1000) mello     (1000)     4360 2022-11-30 14:07:17.000000 awsibox-0.8.7/awsibox/lambdas/ServiceDiscovery.code
--rw-r--r--   0 mello     (1000) mello     (1000)      890 2022-11-30 13:39:06.000000 awsibox-0.8.7/awsibox/lambdas/ServiceUnavailable.code
--rw-r--r--   0 mello     (1000) mello     (1000)     2589 2023-05-18 20:19:14.000000 awsibox-0.8.7/awsibox/lambdas/StacksOps.code
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.389291 awsibox-0.8.7/awsibox/mod/
--rw-r--r--   0 mello     (1000) mello     (1000)     3962 2023-06-16 08:24:34.000000 awsibox-0.8.7/awsibox/mod/autoscaling.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3746 2023-06-16 09:25:14.000000 awsibox-0.8.7/awsibox/mod/cloudformation.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2169 2023-06-16 08:27:11.000000 awsibox-0.8.7/awsibox/mod/cloudfront.py
--rw-r--r--   0 mello     (1000) mello     (1000)    13198 2023-06-16 08:28:25.000000 awsibox-0.8.7/awsibox/mod/ec2.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2353 2023-06-16 08:28:54.000000 awsibox-0.8.7/awsibox/mod/ecr.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2829 2023-06-16 08:29:28.000000 awsibox-0.8.7/awsibox/mod/efs.py
--rw-r--r--   0 mello     (1000) mello     (1000)     5205 2023-06-16 08:30:20.000000 awsibox-0.8.7/awsibox/mod/elasticloadbalancing.py
--rw-r--r--   0 mello     (1000) mello     (1000)     3320 2023-06-16 08:30:51.000000 awsibox-0.8.7/awsibox/mod/iam.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2945 2023-06-16 08:14:41.000000 awsibox-0.8.7/awsibox/mod/joker.py
--rw-r--r--   0 mello     (1000) mello     (1000)     5849 2023-06-16 08:32:12.000000 awsibox-0.8.7/awsibox/mod/rds.py
--rw-r--r--   0 mello     (1000) mello     (1000)     2674 2023-06-16 08:32:47.000000 awsibox-0.8.7/awsibox/mod/s3.py
--rw-r--r--   0 mello     (1000) mello     (1000)     7926 2023-06-16 08:33:12.000000 awsibox-0.8.7/awsibox/mod/waf.py
--rw-r--r--   0 mello     (1000) mello     (1000)    46030 2023-06-09 13:02:41.000000 awsibox-0.8.7/awsibox/shared.py
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.389291 awsibox-0.8.7/awsibox/user-data/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.393291 awsibox-0.8.7/awsibox/user-data/SCRIPTS/
--rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-02 14:06:20.000000 awsibox-0.8.7/awsibox/user-data/SCRIPTS/ELBCHECK.sh
--rw-r--r--   0 mello     (1000) mello     (1000)      685 2023-02-28 14:52:11.000000 awsibox-0.8.7/awsibox/user-data/SCRIPTS/END.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1467 2023-01-03 11:25:14.000000 awsibox-0.8.7/awsibox/user-data/SCRIPTS/INIT.sh
--rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-05 16:57:15.000000 awsibox-0.8.7/awsibox/user-data/SCRIPTS/PACKAGE.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1184 2023-01-02 14:06:20.000000 awsibox-0.8.7/awsibox/user-data/SCRIPTS/SERVICE.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     1771 2023-01-03 16:26:40.000000 awsibox-0.8.7/awsibox/user-data/SCRIPTS/SETUP.sh
--rw-r--r--   0 mello     (1000) mello     (1000)     2521 2023-01-03 11:24:26.000000 awsibox-0.8.7/awsibox/user-data/ecs-cluster.sh
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.265289 awsibox-0.8.7/build/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.265289 awsibox-0.8.7/build/lib/
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.277289 awsibox-0.8.7/build/lib/awsibox.egg-info/
--rw-r--r--   0 mello     (1000) mello     (1000)     1014 2023-06-16 09:29:30.000000 awsibox-0.8.7/build/lib/awsibox.egg-info/PKG-INFO
--rw-r--r--   0 mello     (1000) mello     (1000)     8805 2023-06-16 09:29:30.000000 awsibox-0.8.7/build/lib/awsibox.egg-info/SOURCES.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-06-16 09:29:30.000000 awsibox-0.8.7/build/lib/awsibox.egg-info/dependency_links.txt
--rw-r--r--   0 mello     (1000) mello     (1000)       44 2023-06-16 09:29:30.000000 awsibox-0.8.7/build/lib/awsibox.egg-info/requires.txt
--rw-r--r--   0 mello     (1000) mello     (1000)        8 2023-06-16 09:29:30.000000 awsibox-0.8.7/build/lib/awsibox.egg-info/top_level.txt
-drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-06-16 09:29:31.393291 awsibox-0.8.7/scripts/
--rwxr-xr-x   0 mello     (1000) mello     (1000)     3350 2023-06-15 12:57:11.000000 awsibox-0.8.7/scripts/ibox_generate_templates.py
--rw-r--r--   0 mello     (1000) mello     (1000)      556 2023-06-16 09:29:31.393291 awsibox-0.8.7/setup.cfg
--rw-r--r--   0 mello     (1000) mello     (1000)      536 2023-06-16 08:09:19.000000 awsibox-0.8.7/setup.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.686881 awsibox-0.8.8/
+-rw-r--r--   0 mello     (1000) mello     (1000)      771 2020-01-23 17:57:57.000000 awsibox-0.8.8/.gitignore
+-rw-r--r--   0 mello     (1000) mello     (1000)    10297 2022-03-14 08:29:15.000000 awsibox-0.8.8/LICENSE
+-rw-r--r--   0 mello     (1000) mello     (1000)      257 2023-06-16 08:09:06.000000 awsibox-0.8.8/MANIFEST.in
+-rw-r--r--   0 mello     (1000) mello     (1000)      877 2023-07-10 13:54:48.686881 awsibox-0.8.8/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)      373 2022-03-14 08:29:15.000000 awsibox-0.8.8/README.md
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.510878 awsibox-0.8.8/awsibox/
+-rw-r--r--   0 mello     (1000) mello     (1000)    19454 2023-07-08 15:37:21.000000 awsibox-0.8.8/awsibox/RP.py
+-rw-r--r--   0 mello     (1000) mello     (1000)       39 2023-07-10 13:54:21.000000 awsibox-0.8.8/awsibox/__init__.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2251 2022-07-01 08:39:37.000000 awsibox-0.8.8/awsibox/args.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.510878 awsibox-0.8.8/awsibox/aws/
+-rw-r--r--   0 mello     (1000) mello     (1000)  7094944 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/aws/CloudFormationResourceSpecification.json
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.478878 awsibox-0.8.8/awsibox/cfg/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.490878 awsibox-0.8.8/awsibox/cfg/ibox/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.546879 awsibox-0.8.8/awsibox/cfg/ibox/com/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.550879 awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5582 2023-07-04 07:34:22.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/autoscalinggroup-elasticloadbalancing.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      534 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/capacity.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      459 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/cloudwatch-agent.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1252 2023-06-16 09:13:11.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1357 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1303 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2303 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2934 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2206 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.550879 awsibox-0.8.8/awsibox/cfg/ibox/com/certificatemanager/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1222 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.554879 awsibox-0.8.8/awsibox/cfg/ibox/com/cloudformation/
+-rw-r--r--   0 mello     (1000) mello     (1000)      658 2023-06-06 14:25:53.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/cloudformation/custom-resource_light-house.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.554879 awsibox-0.8.8/awsibox/cfg/ibox/com/cloudfront/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1481 2023-07-06 14:25:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1656 2023-07-03 12:08:45.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/cloudfront/for-services.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      197 2023-07-06 10:29:30.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/cloudfront/i_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      495 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/cloudfront/origin-adhoc.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.558879 awsibox-0.8.8/awsibox/cfg/ibox/com/codedeploy/
+-rw-r--r--   0 mello     (1000) mello     (1000)      190 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/codedeploy/deployment-group.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1935 2023-07-06 08:02:40.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/common.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.558879 awsibox-0.8.8/awsibox/cfg/ibox/com/dynamodb/
+-rw-r--r--   0 mello     (1000) mello     (1000)      579 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.558879 awsibox-0.8.8/awsibox/cfg/ibox/com/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1975 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ec2/bottlerocket.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      265 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ec2/securitygroup.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      672 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.566879 awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2452 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/capacityprovider.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1414 2023-06-14 16:05:45.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1518 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/fargate-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3156 2023-07-03 10:17:08.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      703 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     5739 2023-07-03 14:54:45.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      899 2023-06-14 16:05:02.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/task.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      399 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/taskdefinition-volume.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.566879 awsibox-0.8.8/awsibox/cfg/ibox/com/efs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      378 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/efs/accesspoint-app.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.570879 awsibox-0.8.8/awsibox/cfg/ibox/com/elasticloadbalancing/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1287 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2246 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1945 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      242 2023-06-14 15:18:04.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/elasticloadbalancing/i_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      201 2023-06-14 16:13:04.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/elasticloadbalancing/loadbalancer.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      194 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/elasticloadbalancing/v2-listener.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.574879 awsibox-0.8.8/awsibox/cfg/ibox/com/events/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2892 2023-05-01 13:36:02.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1340 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/events/cluster-autoscale.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     6914 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/events/ec2.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1581 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2584 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/events/ecs-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1570 2023-05-01 13:33:03.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/events/ecs.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1203 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/events/spot_advisor.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.582879 awsibox-0.8.8/awsibox/cfg/ibox/com/iam/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5020 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/iam/managed-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      435 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/iam/policy-ecs-exec.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      939 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2115 2023-05-18 13:24:47.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/iam/policy-update_stack.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1591 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1939 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/iam/roles.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.582879 awsibox-0.8.8/awsibox/cfg/ibox/com/kms/
+-rw-r--r--   0 mello     (1000) mello     (1000)      684 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.586879 awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/
+-rw-r--r--   0 mello     (1000) mello     (1000)      607 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3732 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1393 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       46 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/layers.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      935 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/py-packager.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1204 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/service-unavailable.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.586879 awsibox-0.8.8/awsibox/cfg/ibox/com/route53/
+-rw-r--r--   0 mello     (1000) mello     (1000)      428 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/route53/resolverendpoint-outbound.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.586879 awsibox-0.8.8/awsibox/cfg/ibox/com/s3/
+-rw-r--r--   0 mello     (1000) mello     (1000)      566 2023-07-07 19:35:03.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/s3/bucket-log.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.590880 awsibox-0.8.8/awsibox/cfg/ibox/com/servicediscovery/
+-rw-r--r--   0 mello     (1000) mello     (1000)      374 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/servicediscovery/publicdnsnamespace-find.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.590880 awsibox-0.8.8/awsibox/cfg/ibox/com/sns/
+-rw-r--r--   0 mello     (1000) mello     (1000)      951 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      225 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/sns/cloudwatch-alarm.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.590880 awsibox-0.8.8/awsibox/cfg/ibox/com/ssm/
+-rw-r--r--   0 mello     (1000) mello     (1000)      312 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/com/ssm/parameter-user-password.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.490878 awsibox-0.8.8/awsibox/cfg/ibox/res/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.594879 awsibox-0.8.8/awsibox/cfg/ibox/res/apigateway/
+-rw-r--r--   0 mello     (1000) mello     (1000)      147 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/apigateway/accounts.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      250 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/apigateway/deployments.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      491 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/apigateway/domain-names.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1821 2023-06-14 15:29:04.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/apigateway/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.594879 awsibox-0.8.8/awsibox/cfg/ibox/res/application-autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)      832 2023-06-14 15:40:34.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2965 2023-06-14 15:41:11.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2143 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.598879 awsibox-0.8.8/awsibox/cfg/ibox/res/autoscaling/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2402 2023-06-14 15:45:22.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3163 2023-06-14 15:45:28.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     5218 2023-07-10 08:40:23.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1889 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.598879 awsibox-0.8.8/awsibox/cfg/ibox/res/certificatemanager/
+-rw-r--r--   0 mello     (1000) mello     (1000)      222 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/certificatemanager/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.602880 awsibox-0.8.8/awsibox/cfg/ibox/res/cloudfront/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5910 2023-07-07 08:35:38.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      504 2023-07-06 09:46:36.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/cloudfront/origin-access-controls.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     5958 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/cloudfront/policies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.602880 awsibox-0.8.8/awsibox/cfg/ibox/res/cloudwatch/
+-rw-r--r--   0 mello     (1000) mello     (1000)     7805 2023-07-03 12:27:14.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/cloudwatch/alarms.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1041 2023-06-14 15:57:15.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      966 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.602880 awsibox-0.8.8/awsibox/cfg/ibox/res/codedeploy/
+-rw-r--r--   0 mello     (1000) mello     (1000)      364 2023-06-14 16:02:37.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/codedeploy/deployment-groups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1081 2023-06-14 16:01:55.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.606880 awsibox-0.8.8/awsibox/cfg/ibox/res/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)      604 2023-07-10 12:57:50.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/ec2/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1794 2023-07-04 07:39:01.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/ec2/securitygroupingresses.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      346 2023-06-29 13:36:52.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/ec2/securitygroups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      438 2023-07-10 13:10:42.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/ec2/subnet-routetable-associations.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1245 2023-07-10 13:15:14.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/ec2/subnets.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      118 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/ec2/vpc-endpoints.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.610880 awsibox-0.8.8/awsibox/cfg/ibox/res/ecr/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1405 2023-06-29 14:55:24.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/ecr/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.610880 awsibox-0.8.8/awsibox/cfg/ibox/res/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)     9924 2023-06-14 16:06:44.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/ecs/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1964 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/ecs/services.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1021 2023-06-06 14:25:53.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.610880 awsibox-0.8.8/awsibox/cfg/ibox/res/efs/
+-rw-r--r--   0 mello     (1000) mello     (1000)       68 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/efs/filesystems.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1961 2023-07-03 12:08:45.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/efs/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.614880 awsibox-0.8.8/awsibox/cfg/ibox/res/elasticache/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5327 2023-05-31 09:04:53.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/elasticache/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       69 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/elasticache/subnet-groups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.618880 awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/
+-rw-r--r--   0 mello     (1000) mello     (1000)     3978 2023-07-03 13:48:39.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1002 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     5049 2023-07-04 07:33:41.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listeners.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2831 2023-07-03 12:17:05.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3618 2023-07-04 07:33:55.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.618880 awsibox-0.8.8/awsibox/cfg/ibox/res/events/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1765 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/events/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.622880 awsibox-0.8.8/awsibox/cfg/ibox/res/iam/
+-rw-r--r--   0 mello     (1000) mello     (1000)     3064 2023-07-04 13:41:29.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/iam/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      143 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/iam/instance-profiles.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3687 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/iam/managed-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1716 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/iam/policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      918 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/iam/roles.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.626880 awsibox-0.8.8/awsibox/cfg/ibox/res/lambda/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1286 2023-07-03 12:08:45.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/lambda/functions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2591 2023-06-14 16:23:01.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/lambda/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      213 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/lambda/layer_permissions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      938 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/lambda/permissions.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      586 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/lambda/versions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.630880 awsibox-0.8.8/awsibox/cfg/ibox/res/rds/
+-rw-r--r--   0 mello     (1000) mello     (1000)      576 2023-07-04 15:47:10.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/rds/db-parameter_groups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      393 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/rds/db-subnet-groups.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     9062 2023-07-04 16:14:49.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/rds/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.630880 awsibox-0.8.8/awsibox/cfg/ibox/res/route53/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1427 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/route53/hostedzones.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      410 2023-06-14 15:15:46.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/route53/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     7296 2023-07-03 09:40:54.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/route53/recordsets.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.634880 awsibox-0.8.8/awsibox/cfg/ibox/res/s3/
+-rw-r--r--   0 mello     (1000) mello     (1000)       41 2023-07-05 12:35:38.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/s3/bucket-policies.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)    12432 2023-07-07 20:33:32.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/s3/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.634880 awsibox-0.8.8/awsibox/cfg/ibox/res/scheduler/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1487 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/scheduler/ibox_base.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.634880 awsibox-0.8.8/awsibox/cfg/ibox/res/sns/
+-rw-r--r--   0 mello     (1000) mello     (1000)      449 2023-06-14 16:29:21.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/sns/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      719 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/sns/subscriptions.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.638880 awsibox-0.8.8/awsibox/cfg/ibox/res/sqs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      467 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/sqs/ibox_base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      978 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/res/sqs/queue-policies.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.494878 awsibox-0.8.8/awsibox/cfg/ibox/stacks/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.638880 awsibox-0.8.8/awsibox/cfg/ibox/stacks/agw/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1690 2023-06-14 15:29:08.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/agw/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2612 2023-04-27 10:02:55.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/agw/infra-info.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.638880 awsibox-0.8.8/awsibox/cfg/ibox/stacks/cch/
+-rw-r--r--   0 mello     (1000) mello     (1000)      280 2023-06-14 15:24:02.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/cch/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.638880 awsibox-0.8.8/awsibox/cfg/ibox/stacks/clf/
+-rw-r--r--   0 mello     (1000) mello     (1000)       89 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/clf/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.642880 awsibox-0.8.8/awsibox/cfg/ibox/stacks/ec2/
+-rw-r--r--   0 mello     (1000) mello     (1000)     4610 2023-07-03 10:16:46.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3411 2023-07-03 13:32:23.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/ec2/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.642880 awsibox-0.8.8/awsibox/cfg/ibox/stacks/ecs/
+-rw-r--r--   0 mello     (1000) mello     (1000)      839 2023-06-15 07:56:29.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/ecs/buildkite.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     2401 2023-07-03 15:45:53.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/ecs/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      690 2023-06-15 07:55:51.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.642880 awsibox-0.8.8/awsibox/cfg/ibox/stacks/lbd/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1291 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.642880 awsibox-0.8.8/awsibox/cfg/ibox/stacks/rds/
+-rw-r--r--   0 mello     (1000) mello     (1000)      241 2023-07-04 15:47:16.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/rds/i_type.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.654880 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/
+-rw-r--r--   0 mello     (1000) mello     (1000)      633 2023-06-15 07:57:04.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-base.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     1543 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      794 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     3497 2023-06-14 15:55:04.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      139 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-event-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      559 2023-06-16 09:17:19.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-extra-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      749 2023-07-04 10:04:47.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     4645 2023-06-14 16:16:30.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      108 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-iam-user-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)      655 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)       29 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-s3-01.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)     4070 2023-07-10 13:18:33.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/vpc.yml
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.654880 awsibox-0.8.8/awsibox/cfg/ibox/stacks/tsk/
+-rw-r--r--   0 mello     (1000) mello     (1000)     2459 2023-06-14 16:36:55.000000 awsibox-0.8.8/awsibox/cfg/ibox/stacks/tsk/i_type.yml
+-rw-r--r--   0 mello     (1000) mello     (1000)    17352 2023-07-10 10:25:27.000000 awsibox-0.8.8/awsibox/cfg.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     6346 2023-07-10 13:32:50.000000 awsibox-0.8.8/awsibox/common.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1867 2023-04-27 09:19:18.000000 awsibox-0.8.8/awsibox/discover.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2315 2023-07-05 16:08:18.000000 awsibox-0.8.8/awsibox/generate.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.670881 awsibox-0.8.8/awsibox/lambdas/
+-rw-r--r--   0 mello     (1000) mello     (1000)     1687 2022-03-14 08:29:15.000000 awsibox-0.8.8/awsibox/lambdas/ASGSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      812 2022-03-14 08:29:15.000000 awsibox-0.8.8/awsibox/lambdas/AtEdgeAddHeaders.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4293 2023-04-11 07:34:58.000000 awsibox-0.8.8/awsibox/lambdas/CCRFargateSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2759 2022-11-22 10:02:17.000000 awsibox-0.8.8/awsibox/lambdas/CCRLightHouse.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     3916 2023-04-11 07:35:07.000000 awsibox-0.8.8/awsibox/lambdas/CCRStackReplicator.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2115 2022-11-22 13:27:14.000000 awsibox-0.8.8/awsibox/lambdas/CloudWatchAlarmStateChange.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     1675 2022-11-22 13:26:46.000000 awsibox-0.8.8/awsibox/lambdas/CloudWatchRepeatedNotify.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      739 2022-03-14 08:29:15.000000 awsibox-0.8.8/awsibox/lambdas/EC2StartStopTagged.code
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     6507 2022-11-30 10:37:32.000000 awsibox-0.8.8/awsibox/lambdas/ECSClusterAutoscale.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     6697 2022-11-29 16:18:45.000000 awsibox-0.8.8/awsibox/lambdas/ECSDrainInstance.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     7111 2023-04-17 15:59:09.000000 awsibox-0.8.8/awsibox/lambdas/ECSDrainTasks.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2899 2022-11-22 15:41:37.000000 awsibox-0.8.8/awsibox/lambdas/ECSEventTaskStateChange.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4193 2023-04-12 09:41:12.000000 awsibox-0.8.8/awsibox/lambdas/ECSEventsSpot.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     6177 2023-04-12 10:46:40.000000 awsibox-0.8.8/awsibox/lambdas/ECSRaiseASGAlarm.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2792 2022-11-30 13:18:45.000000 awsibox-0.8.8/awsibox/lambdas/ECSRunTask.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      987 2022-03-14 08:29:15.000000 awsibox-0.8.8/awsibox/lambdas/ECSUpdateDesiredCount.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2167 2022-03-14 08:29:15.000000 awsibox-0.8.8/awsibox/lambdas/ElasticSearchSnapShot.code
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     5370 2023-06-07 12:49:30.000000 awsibox-0.8.8/awsibox/lambdas/InfraInfo.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     1267 2022-04-23 16:11:28.000000 awsibox-0.8.8/awsibox/lambdas/ManageService.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      547 2022-03-14 08:29:15.000000 awsibox-0.8.8/awsibox/lambdas/PaidApi.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2724 2023-04-07 09:45:45.000000 awsibox-0.8.8/awsibox/lambdas/PyPackager.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      844 2022-03-14 08:29:15.000000 awsibox-0.8.8/awsibox/lambdas/Python37SSM.layer
+-rw-r--r--   0 mello     (1000) mello     (1000)     3826 2022-11-30 13:32:53.000000 awsibox-0.8.8/awsibox/lambdas/R53RecordInstanceId.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     4360 2022-11-30 14:07:17.000000 awsibox-0.8.8/awsibox/lambdas/ServiceDiscovery.code
+-rw-r--r--   0 mello     (1000) mello     (1000)      890 2022-11-30 13:39:06.000000 awsibox-0.8.8/awsibox/lambdas/ServiceUnavailable.code
+-rw-r--r--   0 mello     (1000) mello     (1000)     2589 2023-05-18 20:19:14.000000 awsibox-0.8.8/awsibox/lambdas/StacksOps.code
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.674881 awsibox-0.8.8/awsibox/mod/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.682881 awsibox-0.8.8/awsibox/mod/__pycache__/
+-rw-r--r--   0 mello     (1000) mello     (1000)     5503 2023-07-10 12:23:40.000000 awsibox-0.8.8/awsibox/mod/__pycache__/autoscaling.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     6051 2023-07-03 12:05:44.000000 awsibox-0.8.8/awsibox/mod/__pycache__/cloudformation.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     3330 2023-07-10 12:23:40.000000 awsibox-0.8.8/awsibox/mod/__pycache__/cloudfront.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)    17996 2023-07-10 12:23:40.000000 awsibox-0.8.8/awsibox/mod/__pycache__/ec2.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     6211 2023-07-03 12:05:44.000000 awsibox-0.8.8/awsibox/mod/__pycache__/elasticloadbalancing.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     4581 2023-07-03 12:05:44.000000 awsibox-0.8.8/awsibox/mod/__pycache__/iam.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     3491 2023-07-10 12:23:40.000000 awsibox-0.8.8/awsibox/mod/__pycache__/joker.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     6017 2023-07-03 12:05:44.000000 awsibox-0.8.8/awsibox/mod/__pycache__/rds.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     3068 2023-07-03 12:05:44.000000 awsibox-0.8.8/awsibox/mod/__pycache__/s3.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)    14961 2023-07-03 12:05:44.000000 awsibox-0.8.8/awsibox/mod/__pycache__/waf.cpython-311.pyc
+-rw-r--r--   0 mello     (1000) mello     (1000)     3950 2023-07-03 14:09:13.000000 awsibox-0.8.8/awsibox/mod/autoscaling.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     3746 2023-06-16 09:25:14.000000 awsibox-0.8.8/awsibox/mod/cloudformation.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     1941 2023-07-08 12:36:18.000000 awsibox-0.8.8/awsibox/mod/cloudfront.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     9175 2023-07-10 13:33:26.000000 awsibox-0.8.8/awsibox/mod/ec2.py
+-rw-r--r--   0 mello     (1000) mello     (1000)     2946 2023-07-07 20:01:28.000000 awsibox-0.8.8/awsibox/mod/joker.py
+-rw-r--r--   0 mello     (1000) mello     (1000)    46519 2023-07-10 12:54:00.000000 awsibox-0.8.8/awsibox/shared.py
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.682881 awsibox-0.8.8/awsibox/user-data/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.686881 awsibox-0.8.8/awsibox/user-data/SCRIPTS/
+-rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-02 14:06:20.000000 awsibox-0.8.8/awsibox/user-data/SCRIPTS/ELBCHECK.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)      685 2023-02-28 14:52:11.000000 awsibox-0.8.8/awsibox/user-data/SCRIPTS/END.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1467 2023-01-03 11:25:14.000000 awsibox-0.8.8/awsibox/user-data/SCRIPTS/INIT.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)      907 2023-01-05 16:57:15.000000 awsibox-0.8.8/awsibox/user-data/SCRIPTS/PACKAGE.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1184 2023-01-02 14:06:20.000000 awsibox-0.8.8/awsibox/user-data/SCRIPTS/SERVICE.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     1771 2023-01-03 16:26:40.000000 awsibox-0.8.8/awsibox/user-data/SCRIPTS/SETUP.sh
+-rw-r--r--   0 mello     (1000) mello     (1000)     2521 2023-01-03 11:24:26.000000 awsibox-0.8.8/awsibox/user-data/ecs-cluster.sh
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.478878 awsibox-0.8.8/build/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.478878 awsibox-0.8.8/build/lib/
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.502878 awsibox-0.8.8/build/lib/awsibox.egg-info/
+-rw-r--r--   0 mello     (1000) mello     (1000)      877 2023-07-10 13:54:47.000000 awsibox-0.8.8/build/lib/awsibox.egg-info/PKG-INFO
+-rw-r--r--   0 mello     (1000) mello     (1000)     9428 2023-07-10 13:54:47.000000 awsibox-0.8.8/build/lib/awsibox.egg-info/SOURCES.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        1 2023-07-10 13:54:47.000000 awsibox-0.8.8/build/lib/awsibox.egg-info/dependency_links.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)       44 2023-07-10 13:54:47.000000 awsibox-0.8.8/build/lib/awsibox.egg-info/requires.txt
+-rw-r--r--   0 mello     (1000) mello     (1000)        8 2023-07-10 13:54:47.000000 awsibox-0.8.8/build/lib/awsibox.egg-info/top_level.txt
+drwxr-xr-x   0 mello     (1000) mello     (1000)        0 2023-07-10 13:54:48.686881 awsibox-0.8.8/scripts/
+-rwxr-xr-x   0 mello     (1000) mello     (1000)     3350 2023-06-15 12:57:11.000000 awsibox-0.8.8/scripts/ibox_generate_templates.py
+-rw-r--r--   0 mello     (1000) mello     (1000)      556 2023-07-10 13:54:48.690881 awsibox-0.8.8/setup.cfg
+-rw-r--r--   0 mello     (1000) mello     (1000)      536 2023-06-16 08:09:19.000000 awsibox-0.8.8/setup.py
```

### Comparing `awsibox-0.8.7/.gitignore` & `awsibox-0.8.8/.gitignore`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/PKG-INFO` & `awsibox-0.8.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: awsibox
-Version: 0.8.7
+Version: 0.8.8
 Summary: AWS Infrastructure in a Box
 Home-page: https://github.com/mello7tre/AwsIBox
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
-Description: # AwsIBox
-        AwsIBox - **AWS** **I**nfrastructure in a **Box**
-        
-        Work in progres...
-        
-        Guidelines:
-        - Infrastructure as code.
-        - Same cloudformation template for all environments and regions (Ex. development and production).
-        - Scalable as needed.
-        
-        ## Installation ##
-        `pip install awsibox`
-        
-        ## License ##
-        
-        This software is distributed under the terms of the MIT [license](LICENSE).
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# AwsIBox
+AwsIBox - **AWS** **I**nfrastructure in a **Box**
+
+Work in progres...
+
+Guidelines:
+- Infrastructure as code.
+- Same cloudformation template for all environments and regions (Ex. development and production).
+- Scalable as needed.
+
+## Installation ##
+`pip install awsibox`
+
+## License ##
+
+This software is distributed under the terms of the MIT [license](LICENSE).
```

### Comparing `awsibox-0.8.7/awsibox/RP.py` & `awsibox-0.8.8/awsibox/RP.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 import yaml
 import yaml.constructor
 import sys
 import os
 import copy
 import json
 import logging
+from yaml.resolver import Resolver
 from pprint import pprint, pformat
 
 from . import cfg
 
+# Un comment to stop PyYAML from automatically converting certain keys to boolean values
+# remove resolver entries for On/Off/Yes/No
+# for ch in "OoYyNn":
+#    if len(Resolver.yaml_implicit_resolvers[ch]) == 1:
+#        del Resolver.yaml_implicit_resolvers[ch]
+#    else:
+#        Resolver.yaml_implicit_resolvers[ch] = [
+#            x
+#            for x in Resolver.yaml_implicit_resolvers[ch]
+#            if x[0] != "tag:yaml.org,2002:bool"
+#        ]
+
 
 def inject_in_RP_map(key_name, value):
     for n, v in cfg.Mappings.items():
         for m, w in v.items():
             if key_name not in w:
                 w[key_name] = value
 
@@ -300,35 +313,20 @@
 
                 for resource_key, resource_key_value in main_key_value.items():
                     if (
                         resource_key == base_key
                         or "IBOX_BASE_SKIP" in resource_key_value
                     ):
                         continue
-                    # inject in cfg key/value
-                    RP_to_cfg(
-                        base_key_value,
-                        prefix=f"{main_key_full}{resource_key}",
-                        overwrite=False,
-                    )
-
                     # inject in existing structure
-                    merged = merge_dict(
+                    RP[main_key][resource_key] = merge_dict(
                         copy.deepcopy(base_key_value), resource_key_value
                     )
-                    # need to do it this way to keep the "link" between existing dict keys and values
-                    for n, v in merged.items():
-                        RP[main_key][resource_key][n] = v
-                # delete IBOX_BASE in RP structure..
+                # delete IBOX_BASE in RP structure
                 del RP[main_key][base_key]
-                # ..and in cfg one
-                try:
-                    del getattr(cfg, f"{root}{main_key}")[base_key]
-                except Exception:
-                    pass
 
             if isinstance(main_key_value, dict):
                 inject_ibox_base(main_key_value, root=main_key_full)
 
     def get_RP(yaml_cfg):
         cfg_keys = ["IBoxLoader", "IBoxLoaderAfter"]
 
@@ -405,21 +403,21 @@
 
             cfg.mappedvalues = mapped_keys
             return RP
 
         # RP_tree represent the resources structure and it's configuration.
         RP_tree = get_RP_tree()
 
+        # Inject IBOX_BASE configurations in RP_tree structure
+        inject_ibox_base(RP_tree)
+
         # Read RP_tree and put a flat key/value configuration in cfg.
         cfg.fixedvalues = {}
         RP_to_cfg(RP_tree)
 
-        # Inject IBOX_BASE configurations
-        inject_ibox_base(RP_tree)
-
         # Create the mapping for env/region.
         RP_map = get_RP_map()
 
         return RP_tree, RP_map
 
     # End inner methods and begin of main code.
 
@@ -461,29 +459,29 @@
         "role": yaml_role,
     }
 
     cfg.RP_tree, cfg.RP_map = get_RP(yaml_cfg)
 
     if cfg.debug:
         print("########## RP ######### START #####")
-        pprint(cfg.RP_tree)
+        pprint(cfg.RP_tree, sort_dicts=False)
         print("########## RP ######### END #######")
 
         print("########## EXCLUDED ####### START #####")
-        pprint(LD_EXCLUDED)
+        pprint(LD_EXCLUDED, sort_dicts=False)
         print("########## EXCLUDED ####### END #######")
 
         print("########## INCLUDED ####### START #####")
-        pprint(LD_INCLUDED)
+        pprint(LD_INCLUDED, sort_dicts=False)
         print("########## INCLUDED ####### END #######")
 
         print("########## FIXED_VALUES ######### START #####")
-        pprint(cfg.fixedvalues)
+        pprint(cfg.fixedvalues, sort_dicts=False)
         print("########## FIXED_VALUES ######### END #######")
 
         print("########## MAPPED_VALUES ######### START #####")
-        pprint(cfg.mappedvalues)
+        pprint(cfg.mappedvalues, sort_dicts=False)
         print("########## MAPPED_VALUES ######### END #######")
 
         print("########## RP_MAP ######### START #####")
-        pprint(cfg.RP_map)
+        pprint(cfg.RP_map, sort_dicts=False)
         print("########## RP_MAP ######### END #######")
```

### Comparing `awsibox-0.8.7/awsibox/args.py` & `awsibox-0.8.8/awsibox/args.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/aws/CloudFormationResourceSpecification.json` & `awsibox-0.8.8/awsibox/aws/CloudFormationResourceSpecification.json`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/capacity.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/capacity.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/ephemeral.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/spot-asg.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/autoscaling/spot-auto.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/certificatemanager/certificate-regional.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/cloudformation/custom-resource_light-house.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/cloudformation/custom-resource_light-house.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/cloudfront/custom-errors.yml`

 * *Files 11% similar despite different names*

```diff
@@ -35,9 +35,8 @@
                 ResponsePagePath: '/error-pages/504.html'
                 ResponseCode: 504
           Origins:
             - PortalStaticErrorPages:
                 DomainName: Sub(f'{cfg.BucketNamePortalStatic}.s3.amazonaws.com')
                 Id: portal-static-error-pages
                 OriginCustomHeaders: []
-                S3OriginConfig:
-                  OriginAccessIdentity: ''
+                S3OriginConfig: {}
```

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/cloudfront/for-services.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/cloudfront/for-services.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/common.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/common.yml`

 * *Files 8% similar despite different names*

```diff
@@ -50,16 +50,21 @@
         Value: Ref('Env')
     - EnvRole:
         Value: Ref('EnvRole')
     - EnvStackVersion:
         Value: Ref('EnvStackVersion')
     - StackType:
         Value: cfg.stacktype
+  AWSAccount:
+    - Own: Ref("AWS::AccountId")
+    - Dev: '000000000000'
+    - Stg: '000000000000'
+    - Prd: '000000000000'
   BaseRegion: eu-west-1
   Mapping:
     - IBoxEnvRegion:
   AllowedIp: [{}]
   CloudWatchAlarmEndpoint: 'mello+aws@ankot.org'
   HostedZoneIdCF: Z2FDTNDATAQYW2
-  LoadBalancer: []
+  LoadBalancer: ''
   RecordSet: ['Internal', 'External']
   SecurityGroupsImport: []
```

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/dynamodb/table-credstash.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/ec2/bottlerocket.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/ec2/bottlerocket.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/ec2/securitygroups-base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/capacityprovider.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/capacityprovider.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/daemon-reserver-cpu.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/fargate-spot.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/fargate-spot.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/service-and-cluster.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 IBoxLoader:
   - !exclude
       - com/ecs/daemon-reserver-cpu.yml
-      - com/elasticloadbalancing/loadbalancer.yml
+      - com/autoscaling/autoscalinggroup-elasticloadbalancing.yml
   - !include
       - stacks/ec2/i_type.yml
       - stacks/ec2/ecs-cluster.yml
 
 global:
   IBOX_LAUNCH_TEMPLATE_NO_SG_EXTRA: True
   IBOX_ROLE_EX: ecs-cluster
```

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/service-and-eventer-scheduled-task.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/service-elasticloadbalancing.yml`

 * *Files 12% similar despite different names*

```diff
@@ -99,33 +99,14 @@
                 - LoadBalancerApplicationInternal
                 - IBOX_IFVALUE
                 - Ref("AWS::NoValue")
               FromPort: get_endvalue("ECSTaskDefinitionBaseContainerDefinitions1ContainerPort")
               IpProtocol: tcp
               SourceSecurityGroupId: ImportValue("SecurityGroupLoadBalancerApplicationInternal")
               ToPort: get_endvalue("ECSTaskDefinitionBaseContainerDefinitions1ContainerPort")
-  EC2SecurityGroupIngress:
-    - LoadBalancerApplicationHttpExternal:
-        IBOX_ENABLED: False
-        CidrIp: '0.0.0.0/0'
-        GroupId: get_expvalue('SecurityGroupLoadBalancerApplicationExternal', 'LoadBalancerApplicationStack')
-        FromPort: get_endvalue('ElasticLoadBalancingV2ListenerECSHttpExternalPort')
-        ToPort: get_endvalue('ElasticLoadBalancingV2ListenerECSHttpExternalPort')
-    - LoadBalancerApplicationHttpInternal:
-        IBOX_ENABLED: False
-        CidrIp: '0.0.0.0/0'
-        GroupId: get_expvalue('SecurityGroupLoadBalancerApplicationInternal', 'LoadBalancerApplicationStack')
-        FromPort: get_endvalue('ElasticLoadBalancingV2ListenerECSHttpInternalPort')
-        ToPort: get_endvalue('ElasticLoadBalancingV2ListenerECSHttpInternalPort')
-    - LoadBalancerApplicationHttpsExternal:
-        IBOX_ENABLED: False
-        CidrIp: '0.0.0.0/0'
-        GroupId: get_expvalue('SecurityGroupLoadBalancerApplicationExternal', 'LoadBalancerApplicationStack')
-        FromPort: get_endvalue('ElasticLoadBalancingV2ListenerECSHttpsExternalPort')
-        ToPort: get_endvalue('ElasticLoadBalancingV2ListenerECSHttpsExternalPort')
   ElasticLoadBalancingV2ListenerRule:
     - HttpsExternalRules1:
         IBOX_ENABLED: True
         Condition: LoadBalancerApplicationExternal
     - HttpInternalRules1:
         IBOX_ENABLED: True
         Condition: LoadBalancerApplicationInternal
```

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/ecs/task.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/ecs/task.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/elasticloadbalancing/accountid.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/elasticloadbalancing/certificate-adhoc.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/elasticloadbalancing/hostedzoneid.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/events/cloudwatch-alarm.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/events/cluster-autoscale.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/events/cluster-autoscale.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/events/ec2.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/events/ec2.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/events/ecs-raise-asg-alarm.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/events/ecs-spot.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/events/ecs-spot.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/events/ecs.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/events/ecs.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/events/spot_advisor.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/events/spot_advisor.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/iam/managed-policies.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/iam/managed-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/iam/policy-parameterstore.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/iam/policy-update_stack.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/iam/policy-update_stack.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/iam/roles-cloudformation-stackset.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/iam/roles.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/iam/roles.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/kms/key-and-alias-parameter-store.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/ccr-fargate-spot.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/ecs-draininstance.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/ecs-runtask.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/py-packager.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/py-packager.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/lambda/service-unavailable.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/lambda/service-unavailable.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/com/sns/asgnotificationr53.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/apigateway/ibox_base.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/apigateway/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/application-autoscaling/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/application-autoscaling/scalabletargets.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/autoscaling/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml`

 * *Files 4% similar despite different names*

```diff
@@ -54,15 +54,17 @@
                 VolumeSize: 0
                 VolumeType: gp3
               Mount: 'yes'
         IamInstanceProfile:
           Arn: GetAtt('InstanceProfile', 'Arn')
         ImageId.IBOX_CODE: If(
           'LaunchTemplateDataImageIdLatest', Ref('LaunchTemplateDataImageIdLatest'), get_endvalue('LaunchTemplateDataImageId'))
-        ImageId.IBOX_AUTO_PO: {}
+        ImageId.IBOX_AUTO_PO:
+          Value: >-
+            ${ImageId} = get_endvalue(f"{IBOX_MAPNAME}ImageId")
         ImageId: latest
         ImageIdLatest.IBOX_AUTO_PO:
           Description: 'Latest Amazon Linux2 ami available from SSM'
           Default: '/aws/service/ami-amazon-linux-latest/amzn2-ami-hvm-x86_64-gp2'
           AllowedValues:
             - '/aws/service/ami-amazon-linux-latest/amzn2-ami-hvm-x86_64-gp2'
             - '/aws/service/ami-amazon-linux-latest/amzn2-ami-kernel-5.10-hvm-x86_64-gp2'
```

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/cloudfront/ibox_base.yml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-IBoxLoader: !include
-  - res/cloudfront/origin-access-identities.yml
-
 global:
   CloudFrontDistribution:
     - IBOX_BASE:
         IBOX_TITLE: CloudFrontDistribution
         Condition: IBOX_RESNAME.Create
         AcmCertificate.IBOX_PCO:
           IBOX_CONDITION:
@@ -51,19 +48,35 @@
                   - IBOX_REFNAME.DomainName:
                       Description: 'empty for mapped value'
                 CustomOriginConfig:
                   IBOX_PARAMETER:
                     - IBOX_REFNAME.CustomOriginConfigHTTPSPort:
                         Description: 'empty for mapped value'
                   OriginProtocolPolicy: https-only
+                OriginAccessControlId.IBOX_AUTO_P:
+                  AllowedValues: ["", "Always", "Conditional", "Never"]
+                OriginAccessControlId.IBOX_PCO:
+                  IBOX_CONDITION:
+                    - IBOX_CURNAME.Always:
+                        get_condition("", "equals", "Always", IBOX_CURNAME)
+                    - IBOX_CURNAME.Conditional:
+                        get_condition("", "equals", "Conditional", IBOX_CURNAME)
+                  IBOX_OUTPUT:
+                    - IBOX_CURNAME:
+                        Value: >-
+                          ${OriginAccessControlId} = get_endvalue(f"{IBOX_MAPNAME}OriginAccessControlId")
+                OriginAccessControlId.IBOX_CODE_KEY: >-
+                  If(
+                    f"{IBOX_CURNAME}Always",
+                    get_endvalue("CloudFrontOriginOriginAccessControlS3Always"),
+                    If(
+                      f"{IBOX_CURNAME}Conditional",
+                      get_endvalue("CloudFrontOriginOriginAccessControlS3Conditional"),
+                      Ref("AWS::NoValue")))
                 OriginPath: ''
-                S3OriginConfig:
-                  IBOX_PARAMETER:
-                    - IBOX_REFNAME.S3OriginConfigOriginAccessIdentity:
-                        Description: 'empty for mapped value'
           PriceClass: PriceClass_100
           ViewerCertificate:
             AcmCertificateArn: If(f'{IBOX_RESNAME}AcmCertificate', get_endvalue('GlobalCertificateArn'), Ref('AWS::NoValue'))
             CloudFrontDefaultCertificate: If(f'{IBOX_RESNAME}AcmCertificate', Ref('AWS::NoValue'), True)
             SslSupportMethod: If(f'{IBOX_RESNAME}AcmCertificate', 'sni-only', Ref('AWS::NoValue'))
             MinimumProtocolVersion.IBOX_CODE: If(f'{IBOX_RESNAME}AcmCertificate', get_endvalue(IBOX_CURNAME), Ref('AWS::NoValue'))
             MinimumProtocolVersion.IBOX_AUTO_PO:
@@ -104,7 +117,17 @@
               get_condition('', 'not_equals', 'none', f'{IBOX_RESNAME}LambdaFunctionARN')
         IBOX_OUTPUT:
           - _LambdaFunctionARN:
               Value: ${LambdaFunctionARN}
         Condition: IBOX_RESNAME.LambdaFunctionARN
         EventType: viewer-request
         LambdaFunctionARN: none
+
+  CloudFrontOriginOriginAccessControl:
+    - IBOX_BASE:
+        IBOX_OUTPUT:
+          _:
+            Value: GetAtt(IBOX_RESNAME, "Id")
+        OriginAccessControlConfig:
+          Name: IBOX_RESNAME
+          OriginAccessControlOriginType: s3
+          SigningProtocol: sigv4
```

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/cloudfront/policies.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/cloudfront/policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/cloudwatch/alarms.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/cloudwatch/alarms.yml`

 * *Files 4% similar despite different names*

```diff
@@ -154,33 +154,33 @@
         Dimensions:
           - LoadBalancer:
               Name: LoadBalancer
               Value: get_expvalue('LoadBalancerApplicationInternalFullName', 'LoadBalancerApplicationStack')
           - TargetGroup:
               Name: TargetGroup
               Value: Sub('${TargetGroupInternal.TargetGroupFullName}')
-    - TargetEC2External5XX:
+    - LoadBalancerApplicationExternalTarget5XX:
         <<: *target5xx
         Dimensions:
           - LoadBalancer:
               Name: LoadBalancer
               Value: Sub('${LoadBalancerApplicationExternal.LoadBalancerFullName}')
-    - TargetEC2Internal5XX:
+    - LoadBalancerApplicationInternalTarget5XX:
         <<: *target5xx
         Dimensions:
           - LoadBalancer:
               Name: LoadBalancer
               Value: Sub('${LoadBalancerApplicationInternal.LoadBalancerFullName}')
-    - BackendExternal5XX:
+    - LoadBalancerClassicExternalBackend5XX:
         <<: *backend5xx
         Dimensions:
           - LoadBalancer:
               Name: LoadBalancerName
               Value: Ref('LoadBalancerClassicExternal')
-    - BackendInternal5XX:
+    - LoadBalancerClassicInternalBackend5XX:
         <<: *backend5xx
         Dimensions:
           - LoadBalancer:
               Name: LoadBalancerName
               Value: Ref('LoadBalancerClassicInternal')
     - LoadBalancerApplicationExternal5XX:
         <<: *alb5xx
```

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/cloudwatch/log_groups.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/codedeploy/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/ecr/ibox_base.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/ecr/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/ecs/ibox_base.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/ecs/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/ecs/services.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/ecs/services.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/ecs/taskdefinitions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/elasticache/ibox_base.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/elasticache/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 IBoxLoader: !include
-  - res/elasticloadbalancing/listeners.yml
+  - res/elasticloadbalancing/v2-listeners.yml
   - res/elasticloadbalancing/v2-targetgroups.yml
   - res/elasticloadbalancing/v2-listener-rules.yml
   - res/elasticloadbalancing/v2-loadbalancers.yml
 
 global:
   ElasticLoadBalancingLoadBalancer:
     - IBOX_BASE:
@@ -58,20 +58,14 @@
                     Value: >-
                       LoadBalancerPort= ${LoadBalancerPort} ,InstancePort= ${InstancePort} ,Protocol= ${Protocol} ,Access= get_endvalue(f"{IBOX_MAPNAME}Access")
               PolicyNames:
                 - If(f'{IBOX_MAPNAME}LBCookieStickinessPolicyBaseCookieExpirationPeriod', 'LBCookieStickinessPolicyBase', Ref('AWS::NoValue'))
               SSLCertificateId: get_endvalue('RegionalCertificateArn')
         SecurityGroups:
           - GetAtt('SecurityGroupLoadBalancer', 'GroupId')
-    - External:
-        Scheme: 'internet-facing'
-        Subnets: Split(',', get_expvalue('SubnetsPublic'))
-    - Internal:
-        Scheme: 'internal'
-        Subnets: Split(',', get_expvalue('SubnetsPrivate'))
 
   ElasticLoadBalancingV2Listener:
     - IBOX_BASE:
         Access: Public
         Port.IBOX_AUTO_PO: {}
 
   ElasticLoadBalancingV2ListenerRule:
```

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/listeners.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listeners.yml`

 * *Files 7% similar despite different names*

```diff
@@ -21,117 +21,126 @@
 Internal: &internal
   DefaultActions:
     - TG:
         Type: forward
         TargetGroupArn: Ref(f'TargetGroupInternal')
   LoadBalancerArn: Ref(f'LoadBalancerApplicationInternal')
 
-HttpExternal: &httpexternal
+HttpExternal: &http_external
   <<: [*external, *http]
 
-HttpInternal: &httpinternal
+HttpInternal: &http_internal
   <<: [*internal, *http]
 
-HttpsExternal: &httpsexternal
+HttpsExternal: &https_external
   <<: [*external, *https]
 
 ALB: &alb
   DefaultActions:
     - 404:
         FixedResponseConfig:
           ContentType: 'text/plain'
           MessageBody: "404 Not Found\n"
           StatusCode: '404'
         Type: 'fixed-response' 
 
 
 global:
   ElasticLoadBalancingV2Listener:
-    - EC2HttpInternal:
+    - EC2LoadBalancerApplicationInternalHttp:
         IBOX_ENABLED: False
         <<: *http
         DefaultActions:
           - TG:
               Type: forward
               TargetGroupArn: Ref('ElasticLoadBalancingV2TargetGroupEC2LoadBalancerApplicationInternal')
         LoadBalancerArn: Ref('LoadBalancerApplicationInternal')
-    - EC2HttpsExternal:
+    - EC2LoadBalancerApplicationExternalHttps:
         IBOX_ENABLED: False
         <<: *https
         DefaultActions:
           - TG:
               Type: forward
               TargetGroupArn: Ref('ElasticLoadBalancingV2TargetGroupEC2LoadBalancerApplicationExternal')
         LoadBalancerArn: Ref('LoadBalancerApplicationExternal')
-    - EC2TCPExternal:
+    - EC2LoadBalancerNetworkExternal:
         IBOX_ENABLED: False
         DefaultActions:
           - TG:
               Type: forward
               TargetGroupArn: Ref('ElasticLoadBalancingV2TargetGroupEC2LoadBalancerNetworkExternal')
         LoadBalancerArn: Ref('LoadBalancerNetworkExternal')
         Protocol: TCP
         Port: 80
-    - EC2TCPInternal:
+    - EC2LoadBalancerNetworkInternal:
         IBOX_ENABLED: False
         DefaultActions:
           - TG:
               Type: forward
               TargetGroupArn: Ref('ElasticLoadBalancingV2TargetGroupEC2LoadBalancerNetworkInternal')
         LoadBalancerArn: Ref('LoadBalancerNetworkInternal')
         Protocol: TCP
         Port: 80
     - ECSHttpDefaultExternal:
         IBOX_ENABLED: False
         IBOX_TITLE: ListenerHttpDefaultExternal
-        <<: [*alb, *httpexternal]
+        <<: [*alb, *http_external]
         IBOX_OUTPUT:
           - _:
               Condition: LoadBalancerApplicationExternal
               Value: Ref(IBOX_TITLE)
               Export: Export(Sub('%s-${AWS::StackName}' % IBOX_TITLE))
         Condition: LoadBalancerApplicationExternal
     - ECSHttpDefaultInternal:
         IBOX_ENABLED: False
         IBOX_TITLE: ListenerHttpDefaultInternal
-        <<: [*alb, *httpinternal]
+        <<: [*alb, *http_internal]
         IBOX_OUTPUT:
           - _:
               Condition: LoadBalancerApplicationInternal
               Value: Ref(IBOX_TITLE)
               Export: Export(Sub('%s-${AWS::StackName}' % IBOX_TITLE))
         Condition: LoadBalancerApplicationInternal
     - ECSHttpsDefaultExternal:
         IBOX_ENABLED: False
         IBOX_TITLE: ListenerHttpsDefaultExternal
-        <<: [*alb, *httpsexternal]
+        <<: [*alb, *https_external]
         IBOX_OUTPUT:
           - _:
               Condition: LoadBalancerApplicationExternal
               Value: Ref(IBOX_TITLE)
               Export: Export(Sub('%s-${AWS::StackName}' % IBOX_TITLE))
         Condition: LoadBalancerApplicationExternal
-    - ECSHttpExternal:
+    - ECSLoadBalancerApplicationExternalHttp:
         IBOX_ENABLED: False
         IBOX_LINKED_OBJ:
           Name: LoadBalancerApplicationHttpExternal
           Key: EC2SecurityGroupIngress
-          Type: LoadBalancerApplicationHttpExternal
-        <<: *httpexternal
+          Type: ECSLoadBalancerApplicationLoadBalancerRule
+          Conf:
+            IBOX_LINKED_OBJ_NAME: IBOX_RESNAME
+            IBOX_LINKED_OBJ_INDEX: External
+        <<: *http_external
         LoadBalancerArn: get_expvalue('LoadBalancerApplicationExternal', 'LoadBalancerApplicationStack')
-    - ECSHttpInternal:
+    - ECSLoadBalancerApplicationInternalHttp:
         IBOX_ENABLED: False
         IBOX_LINKED_OBJ:
           Name: LoadBalancerApplicationHttpInternal
           Key: EC2SecurityGroupIngress
-          Type: LoadBalancerApplicationHttpInternal
-        <<: *httpinternal
+          Type: ECSLoadBalancerApplicationLoadBalancerRule
+          Conf:
+            IBOX_LINKED_OBJ_NAME: IBOX_RESNAME
+            IBOX_LINKED_OBJ_INDEX: Internal
+        <<: *http_internal
         LoadBalancerArn: get_expvalue('LoadBalancerApplicationInternal', 'LoadBalancerApplicationStack')
-    - ECSHttpsExternal:
+    - ECSLoadBalancerApplicationExternalHttps:
         IBOX_ENABLED: False
         IBOX_RESNAME: ListenerHttpsExternal
         IBOX_LINKED_OBJ:
           Name: LoadBalancerApplicationHttpsExternal
           Key: EC2SecurityGroupIngress
-          Type: LoadBalancerApplicationHttpsExternal
-        <<: *httpsexternal
+          Type: ECSLoadBalancerApplicationLoadBalancerRule
+          Conf:
+            IBOX_LINKED_OBJ_NAME: IBOX_REFNAME
+            IBOX_LINKED_OBJ_INDEX: External
+        <<: *https_external
         LoadBalancerArn: get_expvalue('LoadBalancerApplicationExternal', 'LoadBalancerApplicationStack')
```

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml`

 * *Files 26% similar despite different names*

```diff
@@ -24,27 +24,43 @@
   Protocol: HTTP
   VpcId: get_expvalue('VpcId')
 
 global:
   ElasticLoadBalancingV2TargetGroup:
     - EC2LoadBalancerApplicationExternal:
         IBOX_ENABLED: False
+        IBOX_LINKED_OBJ:
+          Key: EC2SecurityGroupIngress
+          Name: LoadBalancerApplicationExternal
+          Type: EC2LoadBalancerApplicationInstancesRule
         <<: *base
         Port: 80
     - EC2LoadBalancerApplicationInternal:
         IBOX_ENABLED: False
+        IBOX_LINKED_OBJ:
+          Key: EC2SecurityGroupIngress
+          Name: LoadBalancerApplicationInternal
+          Type: EC2LoadBalancerApplicationInstancesRule
         <<: *base
         Port: 80
     - EC2LoadBalancerNetworkExternal:
         IBOX_ENABLED: False
+        IBOX_LINKED_OBJ:
+          Key: EC2SecurityGroupIngress
+          Name: LoadBalancerNetworkExternal
+          Type: EC2LoadBalancerNetworkInstancesRule
         Port: 80
         Protocol: TCP
         VpcId: get_expvalue('VpcId')
     - EC2LoadBalancerNetworkInternal:
         IBOX_ENABLED: False
+        IBOX_LINKED_OBJ:
+          Key: EC2SecurityGroupIngress
+          Name: LoadBalancerNetworkInternal
+          Type: EC2LoadBalancerNetworkInstancesRule
         Port: 80
         Protocol: TCP
         VpcId: get_expvalue('VpcId')
     - ECSLoadBalancerApplicationDefaultExternal:
         IBOX_ENABLED: False
         IBOX_TITLE: TargetGroupServiceUnavailableExternal
         IBOX_OUTPUT:
```

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/events/ibox_base.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/events/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/iam/ibox_base.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/iam/ibox_base.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 IBoxLoader: !include
   - res/iam/managed-policies.yml
   - res/iam/roles.yml
 
 global:
+  IAMGroup:
+    - IBOX_BASE:
+        Create: 'yes'
+        GroupName: IBOX_INDEXNAME
+        ManagedPolicyArns.IBOX_CUSTOM_OBJ:
+          Value: ImportValue(f"IAMPolicy{IBOX_RESNAME}") if not IBOX_RESNAME.startswith(("arn", "Ref(")) else get_dictvalue(IBOX_RESNAME)
   IAMManagedPolicy:
     - IBOX_BASE:
         IBOX_RESNAME: IAMPolicy.IBOX_INDEXNAME
         IBOX_OUTPUT:
           - _:
               IBOX_ENABLED_IF: get_endvalue(f"{IBOX_MAPNAME}Export") == True
               Value: Ref(IBOX_RESNAME)
@@ -57,17 +63,25 @@
             IBOX_RESNAME: SSMParameterPassword.IBOX_INDEXNAME
             IBOX_LINKED_OBJ_NAME: IBOX_RESNAME
             IBOX_LINKED_OBJ_INDEX: IBOX_INDEXNAME
         IBOX_PARAMETER:
           - PasswordBase.IBOX_INDEXNAME:
               Description: "Base Password, must be changed at first login"
               NoEcho: True
-        IBOX_CONDITION:
-          - _:
-              get_condition("", "equals", "yes", f"{IBOX_RESNAME}Enabled")
-          - _RoleAccount:
-              get_condition("", "not_equals", "none", f"{IBOX_RESNAME}RoleAccount")
-        Condition: IBOX_RESNAME
-        UserName: str(IBOX_REMAPNAME)
+        Create: 'yes'
+        Groups.IBOX_CUSTOM_OBJ:
+          IBOX_CONDITION:
+            - IBOX_REFNAME.Group.IBOX_RESNAME:
+                get_condition("", "equals", "yes", f"{IBOX_MAPNAME}{IBOX_RESNAME}")
+          Value: If(f"{IBOX_REFNAME}Group{IBOX_RESNAME}", IBOX_RESNAME, Ref("AWS::NoValue"))
         LoginProfile:
           Password: GetAtt(f"SSMParameterPassword{IBOX_INDEXNAME}", "Value")
           PasswordResetRequired: True
+        UserName: str(IBOX_REMAPNAME)
+  IAMUserToGroupAddition:
+    - IBOX_BASE:
+        GroupName: IBOX_INDEXNAME
+        Users.IBOX_CUSTOM_OBJ:
+          IBOX_CONDITION:
+            - IBOX_MAPNAME.IBOX_RESNAME:
+                get_condition("", "not_equals", "none", f"{IBOX_MAPNAME}{IBOX_RESNAME}")
+          Value: If(f"{IBOX_MAPNAME}{IBOX_RESNAME}",  get_endvalue(f"{IBOX_MAPNAME}{IBOX_RESNAME}"), Ref("AWS::NoValue"))
```

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/iam/managed-policies.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/iam/managed-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/iam/policies.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/iam/policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/iam/roles.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/iam/roles.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/lambda/functions.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/lambda/functions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/lambda/ibox_base.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/lambda/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/lambda/permissions.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/lambda/permissions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/lambda/versions.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/lambda/versions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/rds/ibox_base.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/rds/ibox_base.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+IBoxLoader: !include
+  - res/rds/db-parameter_groups.yml
+
 Mysql: &mysql
   Engine: mysql
   EngineVersion: '5.7'
 
 MysqlInternal:
   <<: *mysql
   PubliclyAccessible: false
@@ -14,20 +17,27 @@
 global:
   RDSDBInstance:
     # Here i use IBOX_MAPNAME in place of IBOX_RESNAME because current resource name IBOX_RESNAME is simply DBInstance.
     # Instead i want to have a code that permit to create multiple rds resources in the same stack.
     - IBOX_BASE:
         IBOX_ENABLED: False
         IBOX_LINKED_OBJ:
-          Key: Route53RecordSet
-          Conf:
-            IBOX_RESNAME: RecordSet
-            IBOX_LINKED_OBJ_NAME: IBOX_RESNAME
-          Type: RDS
-          For: ["External", "Internal"]
+          ParameterGroup:
+            Key: RDSDBParameterGroup
+            Type: Base
+            Conf:
+              IBOX_TITLE: DBParameterGroup1
+              IBOX_LINKED_OBJ_NAME: IBOX_REFNAME
+          RecordSet:
+            Key: Route53RecordSet
+            Conf:
+              IBOX_RESNAME: RecordSet
+              IBOX_LINKED_OBJ_NAME: IBOX_RESNAME
+            Type: RDS
+            For: ["External", "Internal"]
         IBOX_PARAMETER:
           - IBOX_MAPNAME.AllocatedStorage:
               Description: 'Storage Size in GB - empty for mapped value'
           - IBOX_MAPNAME.MaxAllocatedStorage:
               Description: 'Max Storage Size in GB (Enable Storage Autoscaling)- empty for mapped value - 0 to disable'
           - IBOX_MAPNAME.DBInstanceClass:
               Description: 'Instance Type - empty for mapped value'
@@ -127,35 +137,43 @@
           - IBOX_MAPNAME.StorageThroughput:
               Value: ${StorageThroughput}
           - IBOX_MAPNAME.Iops:
               Value: ${Iops}
         AllocatedStorage: 50
         AllowMajorVersionUpgrade: true
         DBInstanceClass: db.t3.micro
+        DBName.IBOX_CODE: If(f"{IBOX_REFNAME}DBInstanceSkipProperties", Ref("AWS::NoValue"), get_endvalue(IBOX_CURNAME))
         DBName: dbname
         DBParameterGroupName: Ref('DBParameterGroup1')
+        DBSnapshotIdentifier.IBOX_CODE: If(IBOX_CURNAME, get_endvalue(IBOX_CURNAME), Ref("AWS::NoValue"))
         DBSnapshotIdentifier: none
         DeletionProtection: false
         EnablePerformanceInsights:
           If(f'{IBOX_MAPNAME}PerformanceInsights', True, False)
         Iops.IBOX_CODE:
           If(f'{IBOX_MAPNAME}Iops', get_endvalue(f'{IBOX_MAPNAME}Iops'), Ref('AWS::NoValue'))
         Iops: 0
+        MasterUsername.IBOX_CODE: If(f"{IBOX_REFNAME}DBInstanceSkipProperties", Ref("AWS::NoValue"), get_endvalue(IBOX_CURNAME))
         MasterUsername: masterusername
+        MasterUserPassword.IBOX_CODE: If(f"{IBOX_REFNAME}DBInstanceSkipProperties", Ref("AWS::NoValue"), get_endvalue(IBOX_CURNAME))
         MasterUserPassword: masteruserpassword
         MaxAllocatedStorage: 0
         MaxAllocatedStorage.IBOX_CODE:
           If(f'{IBOX_MAPNAME}StorageAutoScaling', get_endvalue(f'{IBOX_MAPNAME}MaxAllocatedStorage'), Ref('AWS::NoValue'))
         MonitoringInterval: 0
         MonitoringRoleArn: If(f'{IBOX_MAPNAME}MonitoringInterval', get_expvalue('RoleRDSEnhancedMonitoring'), Ref('AWS::NoValue'))
         MultiAZ: false
         PerformanceInsights: 0
         PerformanceInsightsRetentionPeriod:
           If(f'{IBOX_MAPNAME}PerformanceInsights', get_endvalue(f'{IBOX_MAPNAME}PerformanceInsights'), Ref('AWS::NoValue'))
+        SourceDBInstanceIdentifier.IBOX_CODE: If(IBOX_CURNAME, get_endvalue(IBOX_CURNAME), Ref("AWS::NoValue"))
         SourceDBInstanceIdentifier: none
         StorageThroughput.IBOX_CODE:
           If(f'{IBOX_MAPNAME}StorageThroughput', get_endvalue(f'{IBOX_MAPNAME}StorageThroughput'), Ref('AWS::NoValue'))
         StorageThroughput: 0
         StorageType: gp3
         VPCSecurityGroups:
           - Ref(f'SecurityGroup{IBOX_MAPNAME}')
 
+  RDSDBParameterGroup:
+    - IBOX_BASE:
+        IBOX_ENABLED: False
```

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/route53/hostedzones.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/route53/hostedzones.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/route53/recordsets.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/route53/recordsets.yml`

 * *Files 5% similar despite different names*

```diff
@@ -29,24 +29,14 @@
   Name: Sub('${AWS::StackName}.${EnvRole}.%s' % cfg.HostedZoneNamePrivate)
 
 LoadBalancer: &loadbalancer
   AliasTarget: &loadbalancer_alias_target
     HostedZoneId: get_endvalue('HostedZoneIdLBNET' if getattr("cfg", "LoadBalancerType", "") == "Network" else 'HostedZoneIdLB')
   Type: A
 
-EC2LoadBalancerTargetExternal: &ec2_loadbalancer_target_external
-  AliasTarget:
-    <<: *loadbalancer_alias_target
-    DNSName: GetAtt(f"LoadBalancer{cfg.LoadBalancerType}External", "DNSName")
-
-EC2LoadBalancerTargetInternal: &ec2_loadbalancer_target_internal
-  AliasTarget:
-    <<: *loadbalancer_alias_target
-    DNSName: GetAtt(f"LoadBalancer{cfg.LoadBalancerType}Internal", "DNSName")
-
 ECSLoadBalancerTargetExternal: &ecs_loadbalancer_target_external
   AliasTarget:
     <<: *loadbalancer_alias_target
     DNSName: get_subvalue('dualstack.${1E}', f'LoadBalancerApplicationExternalDNS', 'LoadBalancerApplicationStack')
 
 ECSLoadBalancerTargetInternal: &ecs_loadbalancer_target_internal
   AliasTarget:
@@ -139,22 +129,27 @@
   AliasTarget:
     DNSName: GetAtt(IBOX_INDEXNAME, 'RegionalDomainName')
     HostedZoneId: GetAtt(IBOX_INDEXNAME, 'RegionalHostedZoneId')
 
 
 global:
   Route53RecordSet:
-    - EC2ExternalLoadBalancerExternal:
-        <<: [*zone_external, *ec2_loadbalancer_target_external, *loadbalancer, *base_external]
-    - EC2ExternalLoadBalancerInternal:
-        <<: [*zone_external, *ec2_loadbalancer_target_internal, *loadbalancer, *base_external]
-    - EC2InternalLoadBalancerInternal:
-        <<: [*zone_internal, *ec2_loadbalancer_target_internal, *loadbalancer, *base_internal]
-    - EC2InternalLoadBalancerExternal:
-        <<: [*zone_internal, *ec2_loadbalancer_target_external, *loadbalancer, *base_internal]
+    - EC2External:
+        <<: [*zone_external, *loadbalancer, *base_external]
+        AliasTarget:
+          <<: *loadbalancer_alias_target
+          DNSName: If(
+            f"LoadBalancerExternal",
+            GetAtt(f"LoadBalancer{cfg.LoadBalancerType}External", "DNSName"),
+            GetAtt(f"LoadBalancer{cfg.LoadBalancerType}Internal", "DNSName"))
+    - EC2Internal:
+        <<: [*zone_internal, *loadbalancer, *base_internal]
+        AliasTarget:
+          <<: *loadbalancer_alias_target
+          DNSName: GetAtt(f"LoadBalancer{cfg.LoadBalancerType}Internal", "DNSName")
     - ECSExternal:
         <<: [*zone_external, *loadbalancer, *base_external]
         AliasTarget:
           <<: *loadbalancer_alias_target
           DNSName: If(
             "LoadBalancerApplicationExternal",
             get_subvalue('dualstack.${1E}', f'LoadBalancerApplicationExternalDNS', 'LoadBalancerApplicationStack'),
```

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/scheduler/ibox_base.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/scheduler/ibox_base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/sns/subscriptions.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/sns/subscriptions.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/res/sqs/queue-policies.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/res/sqs/queue-policies.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/stacks/agw/i_type.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/stacks/agw/i_type.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/stacks/agw/infra-info.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/stacks/agw/infra-info.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/stacks/ec2/ecs-cluster.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 IBoxLoader: 
   - !exclude
       - com/cloudfront/for-services.yml
-      - com/elasticloadbalancing/loadbalancer.yml
+      - com/autoscaling/autoscalinggroup-elasticloadbalancing.yml
   - !include
       #- com/autoscaling/imageid-ecs.yml
       - com/ecs/capacityprovider.yml
       - com/ecs/daemon-reserver-cpu.yml
       - com/ec2/bottlerocket.yml
 
 global:
```

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/stacks/ec2/i_type.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/stacks/ec2/i_type.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 IBoxLoader: !include
   - res/autoscaling/autoscalinggroups.yml
   - res/iam/instance-profiles.yml
-  - com/elasticloadbalancing/loadbalancer.yml
+  - com/autoscaling/autoscalinggroup-elasticloadbalancing.yml
   - com/ec2/securitygroup.yml
   - com/cloudfront/for-services.yml
   - com/iam/policy-parameterstore.yml
 
 global:
   Parameter:
     - UpdateMode:
@@ -61,15 +61,15 @@
   CloudFrontDistribution:
     - IBOX_BASE:
         DistributionConfig:
           Origins:
             - Default:
                 CustomOriginConfig:
                   HTTPSPort.IBOX_CODE: If(
-                    f"{IBOX_CURNAME}Override", Ref(IBOX_CURNAME), get_endvalue("ElasticLoadBalancingV2ListenerEC2HttpsExternalPort"))
+                    f"{IBOX_CURNAME}Override", Ref(IBOX_CURNAME), get_endvalue("ElasticLoadBalancingV2ListenerEC2LoadBalancerApplicationExternalHttpsPort"))
   EC2SecurityGroup:
     - InstancesRules:
         IBOX_NO_OUTPUT: True
         GroupDescription: Enable Access from LoadBalancer to Instances and between Instances
   LoadBalancerType: Classic
   IAMPolicy:
     - CloudFormation:
@@ -91,21 +91,21 @@
         ManagedPolicyArns:
           - get_expvalue('IAMPolicyBaseInstance')
           - get_expvalue('IAMPolicySSM')
         Principal: ec2.amazonaws.com
 
 dev: &cfg_dev
   CloudWatchAlarm:
-    BackendExternal5XX:
+    LoadBalancerClassicExternalBackend5XX:
       EvaluationPeriods: 0
-    BackendInternal5XX:
+    LoadBalancerClassicInternalBackend5XX:
       EvaluationPeriods: 0
-    TargetEC2External5XX:
+    LoadBalancerApplicationExternalTarget5XX:
       EvaluationPeriods: 0
-    TargetEC2Internal5XX:
+    LoadBalancerApplicationInternalTarget5XX:
       EvaluationPeriods: 0
 
 stg: *cfg_dev 
 
 
 prd:
   #AutoScalingGroupBaseHealthCheckType: ELB
```

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/stacks/ecs/buildkite.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/stacks/ecs/buildkite.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/stacks/ecs/i_type.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/stacks/ecs/i_type.yml`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
   CloudFrontDistribution:
     - IBOX_BASE:
         DistributionConfig:
           Origins:
             - Default:
                 CustomOriginConfig:
                   HTTPSPort.IBOX_CODE: If(
-                    f"{IBOX_CURNAME}Override", Ref(IBOX_CURNAME), get_endvalue("ElasticLoadBalancingV2ListenerECSHttpsExternalPort"))
+                    f"{IBOX_CURNAME}Override", Ref(IBOX_CURNAME), get_endvalue("ElasticLoadBalancingV2ListenerECSLoadBalancerApplicationExternalHttpsPort"))
   CloudWatchAlarm:
     - ECSCPUHigh:
         AlarmActions: [Ref('ApplicationAutoScalingScalingPolicyUp')]
     - ECSCPULow:
         AlarmActions: [Ref('ApplicationAutoScalingScalingPolicyDown')]
   EC2SecurityGroup:
     - EcsService:
```

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/stacks/ecs/reserve-cpu.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/stacks/lbd/stacks-ops.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-base.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-base.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-ccr-lighthouse.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-ccr-stack-replicator.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-ecs-alb.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-extra-01.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-extra-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-iam-group-01.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 global:
   StackName: iam-g-01
   IAMGroup:
     - Base:
-        Enabled: 'yes'
         ManagedPolicyArns:
           - IAMUserManageOwn
           - S3ListBuckets
           - LogGroupsDescribe
     - Power:
-        Enabled: 'yes'
         ManagedPolicyArns:
           - IAMUserManageOwn
           - PowerUserAccessNoSSM
           - SSMParameterStoreBase
     - Developer:
-        Enabled: 'yes'
         ManagedPolicyArns:
           - Developer
     - BackEndDeveloper:
-        Enabled: 'yes'
         ManagedPolicyArns:
           - Developer
           - BackEndDeveloper
     - FrontEndDeveloper:
-        Enabled: 'yes'
         ManagedPolicyArns:
           - Developer
           - FrontEndDeveloper
     - CloudWatchRead:
-        Enabled: 'yes'
         ManagedPolicyArns:
           - LogRead
           - MetricRead
     - CloudWatchReadJoker01:
-        Enabled: 'yes'
         ManagedPolicyArns:
           - LogReadJoker01
```

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-iam-policy-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/stacks/res/res-latedge-01.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg/ibox/stacks/tsk/i_type.yml` & `awsibox-0.8.8/awsibox/cfg/ibox/stacks/tsk/i_type.yml`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/cfg.py` & `awsibox-0.8.8/awsibox/cfg.py`

 * *Files 11% similar despite different names*

```diff
@@ -113,15 +113,15 @@
     "get_condition(",
     "dict(",
     "eval(",
     "str(",
     "int(",
     "list(",
     "getattr(",
-    "SG_SecurityGroups",
+    "range(",
 )
 
 EVAL_FUNCTIONS_IN_CFG = EVAL_PYTHON_FUNCTIONS_IN_CFG + EVAL_TROPO_FUNCTIONS_IN_CFG
 
 CLF_PATH_PATTERN_REPLACEMENT = {
     "/": "SLASH",
     "*": "STAR",
@@ -339,26 +339,30 @@
     },
     "CloudFrontCachePolicy": {"module": "joker", "func": ("cloudfront", "CachePolicy")},
     "CloudFrontDistribution": {
         "module": "cloudfront",
         "func": "CF_CloudFront",
         "dep": [
             "ElasticLoadBalancingV2Listener",
-            "LoadBalancer",
+            "ElasticLoadBalancingLoadBalancer",
             "CloudFrontLambdaFunctionAssociation",
         ],
     },
     "CloudFrontFunction": {
         "module": "joker",
         "func": ("cloudfront", "Function"),
     },
     "CloudFrontLambdaFunctionAssociation": {
         "module": "joker",
         "func": ("cloudfront", "LambdaFunctionAssociation"),
     },
+    "CloudFrontOriginOriginAccessControl": {
+        "module": "joker",
+        "func": ("cloudfront", "OriginAccessControl"),
+    },
     "CloudFrontOriginAccessIdentity": {
         "module": "joker",
         "func": ("cloudfront", "CloudFrontOriginAccessIdentity"),
         "dep": ["S3Bucket"],
     },
     "CloudFrontOriginRequestPolicy": {
         "module": "joker",
@@ -367,15 +371,15 @@
     "CloudFrontResponseHeadersPolicy": {
         "module": "joker",
         "func": ("cloudfront", "ResponseHeadersPolicy"),
     },
     "CloudWatchAlarm": {
         "module": "joker",
         "func": ("cloudwatch", "Alarm"),
-        "dep": ["LoadBalancer", "SQSQueue"],
+        "dep": ["ElasticLoadBalancingLoadBalancer", "SQSQueue"],
     },
     "CodeDeployApplication": {"module": "joker", "func": ("codedeploy", "Application")},
     "CodeDeployDeploymentGroup": {
         "module": "joker",
         "func": ("codedeploy", "DeploymentGroup"),
     },
     "DynamoDBTable": {"module": "joker", "func": ("dynamodb", "Table")},
@@ -383,47 +387,57 @@
     "EC2InternetGateway": {"module": "joker", "func": ("ec2", "InternetGateway")},
     "EC2NatGateway": {"module": "joker", "func": ("ec2", "NatGateway")},
     "EC2Route": {"module": "joker", "func": ("ec2", "Route")},
     "EC2RouteTable": {"module": "joker", "func": ("ec2", "RouteTable")},
     "EC2SecurityGroup": {
         "module": "ec2",
         "func": "SG_SecurityGroup",
-        "dep": ["ECSTaskDefinition"],
+        "dep": ["ECSTaskDefinition", "EFSFileSystem"],
     },
     "EC2SecurityGroupIngress": {
         "module": "ec2",
         "func": "SG_SecurityGroupIngresses",
-        "dep": ["ElasticLoadBalancingV2Listener"],
+        "dep": [
+            "ElasticLoadBalancingV2Listener",
+            "ElasticLoadBalancingLoadBalancer",
+            "EFSFileSystem",
+        ],
+    },
+    "EC2Subnet": {"module": "joker", "func": ("ec2", "Subnet"), "dep": ["EC2VPC"]},
+    "EC2SubnetRouteTableAssociation": {
+        "module": "joker",
+        "func": ("ec2", "SubnetRouteTableAssociation"),
+        "dep": ["EC2VPC"],
     },
-    "EC2Subnet": {"module": "ec2", "func": "EC2_Subnet"},
     "EC2VPC": {"module": "joker", "func": ("ec2", "VPC")},
     "EC2VPCEndpoint": {"module": "joker", "func": ("ec2", "VPCEndpoint")},
     "EC2VPCGatewayAttachment": {
         "module": "joker",
         "func": ("ec2", "VPCGatewayAttachment"),
     },
     "EC2VPCPeeringConnection": {
         "module": "joker",
         "func": ("ec2", "VPCPeeringConnection"),
     },
-    "ECRRepository": {"module": "ecr", "func": "ECR_Repositories"},
+    "ECRRepository": {"module": "joker", "func": ("ecr", "Repository")},
     "ECSCapacityProvider": {"module": "joker", "func": ("ecs", "CapacityProvider")},
     "ECSCluster": {"module": "joker", "func": ("ecs", "Cluster")},
     "ECSClusterCapacityProviderAssociations": {
         "module": "joker",
         "func": ("ecs", "ClusterCapacityProviderAssociations"),
     },
     "ECSService": {
         "module": "joker",
         "func": ("ecs", "Service"),
         "dep": ["SecurityGroups"],
     },
     "ECSTaskDefinition": {"module": "joker", "func": ("ecs", "TaskDefinition")},
     "EFSAccessPoint": {"module": "joker", "func": ("efs", "AccessPoint")},
-    "EFSFileSystem": {"module": "efs", "func": "EFS_FileStorage"},
+    "EFSFileSystem": {"module": "joker", "func": ("efs", "FileSystem")},
+    "EFSMountTarget": {"module": "joker", "func": ("efs", "MountTarget")},
     "ElastiCacheCacheCluster": {
         "module": "joker",
         "func": ("elasticache", "CacheCluster"),
     },
     "ElastiCacheParameterGroup": {
         "module": "joker",
         "func": ("elasticache", "ParameterGroup"),
@@ -432,22 +446,26 @@
         "module": "joker",
         "func": ("elasticache", "ReplicationGroup"),
     },
     "ElastiCacheSubnetGroup": {
         "module": "joker",
         "func": ("elasticache", "SubnetGroup"),
     },
+    "ElasticLoadBalancingLoadBalancer": {
+        "module": "joker",
+        "func": ("elasticloadbalancing", "LoadBalancer"),
+    },
     "ElasticLoadBalancingV2LoadBalancer": {
         "module": "joker",
         "func": ("elasticloadbalancingv2", "LoadBalancer"),
     },
     "ElasticLoadBalancingV2Listener": {
         "module": "joker",
         "func": ("elasticloadbalancingv2", "Listener"),
-        "dep": ["LoadBalancer"],
+        "dep": ["ElasticLoadBalancingLoadBalancer"],
     },
     "ElasticLoadBalancingV2ListenerRule": {
         "module": "joker",
         "func": ("elasticloadbalancingv2", "ListenerRule"),
     },
     "ElasticLoadBalancingV2TargetGroup": {
         "module": "joker",
@@ -456,29 +474,32 @@
         "dep": ["ECSTaskDefinition"],
     },
     "EventsRule": {
         "module": "joker",
         "func": ("events", "Rule"),
         "dep": ["SecurityGroups"],
     },
-    "IAMGroup": {"module": "iam", "func": "IAM_Groups"},
+    "IAMGroup": {"module": "joker", "func": ("iam", "Group")},
     "IAMInstanceProfile": {"module": "joker", "func": ("iam", "InstanceProfile")},
     "IAMManagedPolicy": {"module": "joker", "func": ("iam", "ManagedPolicy")},
     "IAMPolicy": {
         "module": "joker",
         "func": ("iam", "PolicyType"),
         "dep": ["S3Bucket"],
     },
     "IAMRole": {
         "module": "joker",
         "func": ("iam", "Role"),
         "dep": ["Lambda", "S3Bucket"],
     },
-    "IAMUser": {"module": "iam", "func": "IAM_Users"},
-    "IAMUserToGroupAddition": {"module": "iam", "func": "IAM_UserToGroupAdditions"},
+    "IAMUser": {"module": "joker", "func": ("iam", "User")},
+    "IAMUserToGroupAddition": {
+        "module": "joker",
+        "func": ("iam", "UserToGroupAddition"),
+    },
     "KMSAlias": {"module": "joker", "func": ("kms", "Alias")},
     "KMSKey": {"module": "joker", "func": ("kms", "Key")},
     "Lambda": {"module": "joker", "func": ("awslambda", "Function")},
     "LambdaEventInvokeConfig": {
         "module": "joker",
         "func": ("awslambda", "EventInvokeConfig"),
     },
@@ -498,34 +519,35 @@
         "dep": ["SNSSubscription", "Lambda", "EventsRule", "SchedulerSchedule"],
     },
     "LambdaVersion": {
         "module": "joker",
         "func": ("awslambda", "Version"),
         "dep": ["Lambda"],
     },
-    "LoadBalancer": {
-        "module": "elasticloadbalancing",
-        "func": "LB_ElasticLoadBalancing",
-    },
     "LogsLogGroup": {
         "module": "joker",
         "func": ("logs", "LogGroup"),
         "dep": ["Lambda"],
     },
-    "RDSDBInstance": {"module": "rds", "func": "RDS_DB"},
+    "RDSDBInstance": {"module": "joker", "func": ("rds", "DBInstance")},
+    "RDSDBParameterGroup": {
+        "module": "joker",
+        "func": ("rds", "DBParameterGroup"),
+        "dep": ["RDSDBInstance"],
+    },
     "RDSDBSubnetGroup": {"module": "joker", "func": ("rds", "DBSubnetGroup")},
     "Route53HostedZone": {"module": "joker", "func": ("route53", "HostedZone")},
     "Route53RecordSet": {
         "module": "joker",
         "func": ("route53", "RecordSetType"),
         "dep": [
             "ApiGatewayDomainName",
             "DBInstance",
             "EFSFileSystem",
-            "LoadBalancer",
+            "ElasticLoadBalancingLoadBalancer",
             "CloudFrontDistribution",
         ],
     },
     "Route53ResolverEndpoint": {
         "module": "joker",
         "func": ("route53resolver", "ResolverEndpoint"),
     },
@@ -533,19 +555,24 @@
         "module": "joker",
         "func": ("route53resolver", "ResolverRule"),
     },
     "Route53ResolverRuleAssociation": {
         "module": "joker",
         "func": ("route53resolver", "ResolverRuleAssociation"),
     },
-    "S3Bucket": {"module": "s3", "func": "S3_Buckets"},
+    "S3Bucket": {"module": "joker", "func": ("s3", "Bucket")},
+    "S3BucketPolicy": {
+        "module": "joker",
+        "func": ("s3", "BucketPolicy"),
+        "dep": ["S3Bucket"],
+    },
     "SecurityGroups": {
         "module": "ec2",
         "func": "SG_SecurityGroups",
-        "dep": ["LoadBalancer"],
+        "dep": ["ElasticLoadBalancingLoadBalancer"],
     },
     "ServiceDiscoveryPublicDnsNamespace": {
         "module": "joker",
         "func": ("servicediscovery", "PublicDnsNamespace"),
     },
     "ServiceDiscoveryService": {
         "module": "joker",
@@ -563,24 +590,14 @@
         "module": "joker",
         "func": ("sqs", "QueuePolicy"),
         "dep": ["SNSSubscription"],
     },
     "SNSSubscription": {"module": "joker", "func": ("sns", "SubscriptionResource")},
     "SNSTopic": {"module": "joker", "func": ("sns", "Topic")},
     "SSMParameter": {"module": "joker", "func": ("ssm", "Parameter")},
-    "WafByteMatchSet": {
-        "module": "waf",
-        "func": ["WAF_GlobalByteMatchSets", "WAF_RegionalByteMatchSets"],
-    },
-    "WafIPSet": {"module": "waf", "func": ["WAF_GlobalIPSets", "WAF_RegionalIPSets"]},
-    "WafRule": {"module": "waf", "func": ["WAF_GlobalRules", "WAF_RegionalRules"]},
-    "WafWebAcl": {
-        "module": "waf",
-        "func": ["WAF_GlobalWebAcls", "WAF_RegionalWebAcls"],
-    },
     "WAFv2IPSet": {
         "module": "joker",
         "func": ("wafv2", "IPSet"),
     },
     "WAFv2WebACL": {
         "module": "joker",
         "func": ("wafv2", "WebACL"),
```

### Comparing `awsibox-0.8.7/awsibox/discover.py` & `awsibox-0.8.8/awsibox/discover.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/generate.py` & `awsibox-0.8.8/awsibox/generate.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,15 @@
-from . import cfg
+from . import cfg, __version__
 from .shared import stack_add_res
-from . import __version__
 from .mod import (
     autoscaling,
     cloudformation,
     cloudfront,
     ec2,
-    ecr,
-    efs,
-    iam,
     joker,
-    elasticloadbalancing,
-    rds,
-    s3,
-    waf,
 )
 
 
 def execute_method(RP_cmm):
     processed = []
 
     def _process(k, v):
```

### Comparing `awsibox-0.8.7/awsibox/lambdas/ASGSpot.code` & `awsibox-0.8.8/awsibox/lambdas/ASGSpot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/AtEdgeAddHeaders.code` & `awsibox-0.8.8/awsibox/lambdas/AtEdgeAddHeaders.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/CCRFargateSpot.code` & `awsibox-0.8.8/awsibox/lambdas/CCRFargateSpot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/CCRLightHouse.code` & `awsibox-0.8.8/awsibox/lambdas/CCRLightHouse.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/CCRStackReplicator.code` & `awsibox-0.8.8/awsibox/lambdas/CCRStackReplicator.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/CloudWatchAlarmStateChange.code` & `awsibox-0.8.8/awsibox/lambdas/CloudWatchAlarmStateChange.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/CloudWatchRepeatedNotify.code` & `awsibox-0.8.8/awsibox/lambdas/CloudWatchRepeatedNotify.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/EC2StartStopTagged.code` & `awsibox-0.8.8/awsibox/lambdas/EC2StartStopTagged.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/ECSClusterAutoscale.code` & `awsibox-0.8.8/awsibox/lambdas/ECSClusterAutoscale.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/ECSDrainInstance.code` & `awsibox-0.8.8/awsibox/lambdas/ECSDrainInstance.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/ECSDrainTasks.code` & `awsibox-0.8.8/awsibox/lambdas/ECSDrainTasks.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/ECSEventTaskStateChange.code` & `awsibox-0.8.8/awsibox/lambdas/ECSEventTaskStateChange.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/ECSEventsSpot.code` & `awsibox-0.8.8/awsibox/lambdas/ECSEventsSpot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/ECSRaiseASGAlarm.code` & `awsibox-0.8.8/awsibox/lambdas/ECSRaiseASGAlarm.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/ECSRunTask.code` & `awsibox-0.8.8/awsibox/lambdas/ECSRunTask.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/ECSUpdateDesiredCount.code` & `awsibox-0.8.8/awsibox/lambdas/ECSUpdateDesiredCount.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/ElasticSearchSnapShot.code` & `awsibox-0.8.8/awsibox/lambdas/ElasticSearchSnapShot.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/InfraInfo.code` & `awsibox-0.8.8/awsibox/lambdas/InfraInfo.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/ManageService.code` & `awsibox-0.8.8/awsibox/lambdas/ManageService.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/PaidApi.code` & `awsibox-0.8.8/awsibox/lambdas/PaidApi.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/PyPackager.code` & `awsibox-0.8.8/awsibox/lambdas/PyPackager.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/Python37SSM.layer` & `awsibox-0.8.8/awsibox/lambdas/Python37SSM.layer`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/R53RecordInstanceId.code` & `awsibox-0.8.8/awsibox/lambdas/R53RecordInstanceId.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/ServiceDiscovery.code` & `awsibox-0.8.8/awsibox/lambdas/ServiceDiscovery.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/ServiceUnavailable.code` & `awsibox-0.8.8/awsibox/lambdas/ServiceUnavailable.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/lambdas/StacksOps.code` & `awsibox-0.8.8/awsibox/lambdas/StacksOps.code`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/mod/autoscaling.py` & `awsibox-0.8.8/awsibox/mod/autoscaling.py`

 * *Files 5% similar despite different names*

```diff
@@ -86,32 +86,32 @@
                 )
 
 
 def AS_Autoscaling(key):
     LoadBalancers = []
     TargetGroups = []
     if cfg.LoadBalancerType == "Classic":
-        for n in cfg.LoadBalancer:
+        for n in cfg.LoadBalancer.replace(",", " ").split():
             LoadBalancers.append(Ref(f"LoadBalancerClassic{n}"))
             setattr(
                 cfg,
                 "EC2InstanceUserDataELBClassicCheckLoadBalancerName",
                 Ref(f"LoadBalancerClassic{n}"),
             )
     if cfg.LoadBalancerType in ["Application", "Network"]:
         for n, v in getattr(cfg, "ElasticLoadBalancingV2TargetGroup", {}).items():
             # check for enabled only for EC2 ones
             if n.startswith("EC2") and v.get("IBOX_ENABLED", True):
                 TargetGroups.append(
-                    Ref(f"ElasticLoadBalancingV2TargetGroupEC2LoadBalancer{n}")
+                    Ref(f"ElasticLoadBalancingV2TargetGroup{n}")
                 )
                 setattr(
                     cfg,
                     "EC2InstanceUserDataELBV2CheckTargetGroupArn",
-                    Ref(f"ElasticLoadBalancingV2TargetGroupTargetGroupLoadBalancer{n}"),
+                    Ref(f"ElasticLoadBalancingV2TargetGroup{n}"),
                 )
 
     # Resources
     AS_LaunchTemplate()
 
     R_ASG = asg.AutoScalingGroup(
         "AutoScalingGroupBase",
```

### Comparing `awsibox-0.8.7/awsibox/mod/cloudformation.py` & `awsibox-0.8.8/awsibox/mod/cloudformation.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/mod/cloudfront.py` & `awsibox-0.8.8/awsibox/mod/cloudfront.py`

 * *Files 9% similar despite different names*

```diff
@@ -14,43 +14,32 @@
         for k in ["DefaultTTL", "MaxTTL", "MinTTL", "ForwardedValues"]:
             try:
                 del v[k]
             except Exception:
                 pass
 
 
-def cache_behavior_process(key):
-    # process default behavior
-    process_cache_policy(key["DefaultCacheBehavior"])
-    # process other behaviors
-    for n, v in key["CacheBehaviors"].items():
-        process_cache_policy(v)
-
-
-def origin_process(name, key):
-    for n, v in key["Origins"].items():
-
-        if "OriginAccessIdentity" in v.get("S3OriginConfig", []):
-            del v["CustomOriginConfig"]
-        else:
-            del v["S3OriginConfig"]
-
-
 def CF_CloudFront(key):
     for n, v in getattr(cfg, key).items():
         if not v.get("IBOX_ENABLED", True):
             continue
         resname = f"{key}{n}"
         # Resources
         R_CloudFrontDistribution = clf.Distribution(resname)
         distribution_config = v["DistributionConfig"]
 
-        # process cache_behavior and origin
-        cache_behavior_process(distribution_config)
-        origin_process(resname, distribution_config)
+        # process cache behaviors
+        process_cache_policy(distribution_config["DefaultCacheBehavior"])
+        for m, w in distribution_config["CacheBehaviors"].items():
+            process_cache_policy(w)
+
+        # process origins
+        for m, w in distribution_config["Origins"].items():
+            if "S3OriginConfig" in w:
+                del w["CustomOriginConfig"]
 
         # Automatically compute Behaviour Order based on PathPattern
         cfg.dbg_clf_compute_order = {}
         sortedcachebehaviors = sorted(
             distribution_config["CacheBehaviors"].items(),
             key=lambda x_y: clf_compute_order(x_y[1]["PathPattern"]),
         )
```

### Comparing `awsibox-0.8.7/awsibox/mod/joker.py` & `awsibox-0.8.8/awsibox/mod/joker.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
         # change resource name using key IBOX_RESNAME
         ibox_resname = v.get("IBOX_RESNAME")
         if ibox_resname:
             resname = parse_ibox_key(ibox_resname, parse_ibox_key_conf)
 
         if cfg.debug:
-            logging.error(f"Joker processing: {key}{n}")
+            logging.error(f"Joker processing: {resname}")
 
         # get IBOX_LINKED_OBJ keys
         linked_obj_name = v.get("IBOX_LINKED_OBJ_NAME", "")
         linked_obj_index = v.get("IBOX_LINKED_OBJ_INDEX", "")
 
         mod = __import__(f"troposphere.{module}")
         my_module = getattr(mod, module)
```

### Comparing `awsibox-0.8.7/awsibox/shared.py` & `awsibox-0.8.8/awsibox/shared.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,34 +68,36 @@
                 else {f"{n}Override": Not(Equals(Ref(n), default))}
             )
 
             add_obj(condition)
         # End
         cfg.template.add_parameter(v)
 
-    cfg.Parameters.clear()
 
     for n, v in cfg.Conditions.items():
         cfg.template.add_condition(n, v)
-    cfg.Conditions.clear()
 
     for n, v in cfg.Mappings.items():
         cfg.template.add_mapping(n, v)
-    cfg.Mappings.clear()
 
     for n, v in cfg.Resources.items():
         cfg.template.add_resource(v)
-    cfg.Resources.clear()
 
     for n, v in cfg.Outputs.items():
         add_objoutput(v)
         cfg.template.add_output(v)
-    cfg.Outputs.clear()
 
     cfg.template.set_metadata(get_dictvalue(cfg.Metadata, mapname="Metadata"))
+
+    # empty
+    cfg.Parameters.clear()
+    cfg.Conditions.clear()
+    cfg.Mappings.clear()
+    cfg.Resources.clear()
+    cfg.Outputs.clear()
     cfg.Metadata.clear()
 
 
 def add_obj(obj):
     if isinstance(obj, list):
         for n in obj:
             add_obj(n)
@@ -527,15 +529,15 @@
     try:
         lambda_file_trunk = os.path.join(*PurePath(lambda_file).parts[-3:])
         with open(lambda_file, "r") as f:
             fdata = f.read()
 
             try:
                 # try to minify using python_minifier
-                code = python_minifier.minify(fdata)
+                code = python_minifier.minify(fdata, preserve_shebang=False)
                 if len(code) > 4096:
                     logging.warning(
                         f"{lambda_file_trunk} > 4096, trying to minify it using a more aggressive option [rename_globals=True]"
                     )
                     code = python_minifier.minify(
                         fdata, rename_globals=True, preserve_globals=["lambda_handler"]
                     )
@@ -904,19 +906,27 @@
                 my_iter = enumerate(key_value)
                 is_dict = False
 
             for n, v in my_iter:
                 rootdict = {"Value": v}
                 obj_title = n if is_dict else v
                 if isinstance(v, dict):
+                    # Conf property can be used to process every keys in a different way,
+                    # Ex overriding Value key or adding IBOX_PARAMETER and so on...
                     rootdict.update(v.get("Conf", {}))
                     v = v.get("Value", v)
                     obj_title = f"{n}Value"
                 rootdict.update(base_rootdict)
-                obj = IBOX_Custom_Obj(obj_title)
+                obj = IBOX_Custom_Obj(
+                    obj_title.translate(
+                        "".maketrans(
+                            {":": None, "/": None, "(": None, ")": None, '"': None}
+                        )
+                    )
+                )
 
                 # save IBOX_RESNAME and IBOX_MAPNAME
                 IBOX_RESNAME_SAVE = IBOX_RESNAME
                 IBOX_MAPNAME_SAVE = IBOX_MAPNAME
                 # set IBOX_RESNAME and IBOX_MAPNAME to call _populate like auto_get_props
                 IBOX_RESNAME = obj_title
                 IBOX_MAPNAME = f"{mapname}{propname}"
@@ -937,26 +947,25 @@
 
         def _linked_obj(linked_obj_data):
             # need to parse them here to have the right values
             lo_name = parse_ibox_key(linked_obj_data.get("Name", IBOX_RESNAME))
             lo_key = parse_ibox_key(linked_obj_data.get("Key", ""))
             lo_type = parse_ibox_key(linked_obj_data.get("Type", ""))
             # this way even if without key "For", for cycle will run at least one time
-            lo_for_cycle = linked_obj_data.get("For", [""])
+            lo_for_cycle = parse_ibox_key(linked_obj_data.get("For", [""]))
 
             louc_cfg = {}
             for lo_for_index in lo_for_cycle:
                 # need to copy it because it's updated
                 lo_conf = copy.deepcopy(
                     linked_obj_data.get("Conf", {"IBOX_LINKED_OBJ_NAME": IBOX_RESNAME})
                 )
                 lo_conf["IBOX_ENABLED"] = True
                 # for all lo_conf entries, if their value is a string parse it using parse_ibox_key
                 for loc_entry_key, loc_entry_value in lo_conf.items():
-                    lo_conf[loc_entry_key] = parse_ibox_key(loc_entry_value)
                     lo_conf[loc_entry_key] = parse_ibox_key(
                         loc_entry_value, conf={"IBOX_LINKED_OBJ_FOR": lo_for_index}
                     )
 
                 linked_obj_key_name = f"{lo_key}{lo_type}{lo_for_index}"
                 target_name = f"{lo_name}{lo_for_index}"
 
@@ -989,15 +998,20 @@
 
                 # assign to louc_cfg lo_key
                 louc_cfg[target_name] = linked_obj
 
             if cfg.debug:
                 pprint(louc_cfg)
             # update cfg and fixedvalues, need to do it this way to avoid overwriting the lo_key and removing all objects
-            RP_to_cfg(louc_cfg, prefix=lo_key, mappedvalues=cfg.mappedvalues)
+            RP_to_cfg(
+                louc_cfg,
+                prefix=lo_key,
+                mappedvalues=cfg.mappedvalues,
+                check_mapped=True,
+            )
             # finally update cfg object base key with configuration including mutiple objects
             getattr(cfg, lo_key).update(louc_cfg)
 
         # Allowed object properties
         props = list(vars(obj)["propnames"])
         props.extend(vars(obj)["attributes"])
 
@@ -1239,19 +1253,19 @@
     return base_ord
 
 
 def parse_ibox_key(value, conf={}):
     if not isinstance(value, str):
         return value
     if value.startswith(cfg.EVAL_PYTHON_FUNCTIONS_IN_CFG):
-        return eval(value)
+        return eval(value, globals(), conf)
     for key in IBOX_SPECIAL_KEYS:
         if key in value:
             if key in conf:
-                value = value.replace(key, conf[key])
+                value = value.replace(key, str(conf[key]))
             else:
                 value = value.replace(key, globals().get(key, ""))
     value = value.replace("_", IBOX_RESNAME)
     value = value.replace(".", "")
 
     return value
```

### Comparing `awsibox-0.8.7/awsibox/user-data/SCRIPTS/ELBCHECK.sh` & `awsibox-0.8.8/awsibox/user-data/SCRIPTS/ELBCHECK.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/user-data/SCRIPTS/END.sh` & `awsibox-0.8.8/awsibox/user-data/SCRIPTS/END.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/user-data/SCRIPTS/INIT.sh` & `awsibox-0.8.8/awsibox/user-data/SCRIPTS/INIT.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/user-data/SCRIPTS/PACKAGE.sh` & `awsibox-0.8.8/awsibox/user-data/SCRIPTS/PACKAGE.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/user-data/SCRIPTS/SERVICE.sh` & `awsibox-0.8.8/awsibox/user-data/SCRIPTS/SERVICE.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/user-data/SCRIPTS/SETUP.sh` & `awsibox-0.8.8/awsibox/user-data/SCRIPTS/SETUP.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/awsibox/user-data/ecs-cluster.sh` & `awsibox-0.8.8/awsibox/user-data/ecs-cluster.sh`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/build/lib/awsibox.egg-info/PKG-INFO` & `awsibox-0.8.8/build/lib/awsibox.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: awsibox
-Version: 0.8.7
+Version: 0.8.8
 Summary: AWS Infrastructure in a Box
 Home-page: https://github.com/mello7tre/AwsIBox
 Author: Mello
 Author-email: mello+python@ankot.org
 License: OSI Approved :: Open Software License 3.0 (OSL-3.0)
-Description: # AwsIBox
-        AwsIBox - **AWS** **I**nfrastructure in a **Box**
-        
-        Work in progres...
-        
-        Guidelines:
-        - Infrastructure as code.
-        - Same cloudformation template for all environments and regions (Ex. development and production).
-        - Scalable as needed.
-        
-        ## Installation ##
-        `pip install awsibox`
-        
-        ## License ##
-        
-        This software is distributed under the terms of the MIT [license](LICENSE).
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Open Software License 3.0 (OSL-3.0)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# AwsIBox
+AwsIBox - **AWS** **I**nfrastructure in a **Box**
+
+Work in progres...
+
+Guidelines:
+- Infrastructure as code.
+- Same cloudformation template for all environments and regions (Ex. development and production).
+- Scalable as needed.
+
+## Installation ##
+`pip install awsibox`
+
+## License ##
+
+This software is distributed under the terms of the MIT [license](LICENSE).
```

### Comparing `awsibox-0.8.7/build/lib/awsibox.egg-info/SOURCES.txt` & `awsibox-0.8.8/build/lib/awsibox.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 ./build/lib/awsibox.egg-info/PKG-INFO
 ./build/lib/awsibox.egg-info/SOURCES.txt
 ./build/lib/awsibox.egg-info/dependency_links.txt
@@ -14,14 +15,15 @@
 awsibox/cfg.py
 awsibox/common.py
 awsibox/discover.py
 awsibox/generate.py
 awsibox/shared.py
 awsibox/aws/CloudFormationResourceSpecification.json
 awsibox/cfg/ibox/com/common.yml
+awsibox/cfg/ibox/com/autoscaling/autoscalinggroup-elasticloadbalancing.yml
 awsibox/cfg/ibox/com/autoscaling/capacity.yml
 awsibox/cfg/ibox/com/autoscaling/cloudwatch-agent.yml
 awsibox/cfg/ibox/com/autoscaling/ephemeral.yml
 awsibox/cfg/ibox/com/autoscaling/imageid-ec2.yml
 awsibox/cfg/ibox/com/autoscaling/imageid-ecs.yml
 awsibox/cfg/ibox/com/autoscaling/mixed_instances.yml
 awsibox/cfg/ibox/com/autoscaling/spot-asg.yml
@@ -87,48 +89,52 @@
 awsibox/cfg/ibox/res/application-autoscaling/scalingpolicies.yml
 awsibox/cfg/ibox/res/autoscaling/autoscalinggroups.yml
 awsibox/cfg/ibox/res/autoscaling/ibox_base.yml
 awsibox/cfg/ibox/res/autoscaling/launchtemplates.yml
 awsibox/cfg/ibox/res/autoscaling/scalingpolicies.yml
 awsibox/cfg/ibox/res/certificatemanager/ibox_base.yml
 awsibox/cfg/ibox/res/cloudfront/ibox_base.yml
-awsibox/cfg/ibox/res/cloudfront/origin-access-identities.yml
+awsibox/cfg/ibox/res/cloudfront/origin-access-controls.yml
 awsibox/cfg/ibox/res/cloudfront/policies.yml
 awsibox/cfg/ibox/res/cloudwatch/alarms.yml
 awsibox/cfg/ibox/res/cloudwatch/ibox_base.yml
 awsibox/cfg/ibox/res/cloudwatch/log_groups.yml
 awsibox/cfg/ibox/res/codedeploy/deployment-groups.yml
 awsibox/cfg/ibox/res/codedeploy/ibox_base.yml
 awsibox/cfg/ibox/res/ec2/ibox_base.yml
+awsibox/cfg/ibox/res/ec2/securitygroupingresses.yml
+awsibox/cfg/ibox/res/ec2/securitygroups.yml
+awsibox/cfg/ibox/res/ec2/subnet-routetable-associations.yml
+awsibox/cfg/ibox/res/ec2/subnets.yml
 awsibox/cfg/ibox/res/ec2/vpc-endpoints.yml
-awsibox/cfg/ibox/res/ecr/accounts.yml
 awsibox/cfg/ibox/res/ecr/ibox_base.yml
 awsibox/cfg/ibox/res/ecs/ibox_base.yml
 awsibox/cfg/ibox/res/ecs/services.yml
 awsibox/cfg/ibox/res/ecs/taskdefinitions.yml
 awsibox/cfg/ibox/res/efs/filesystems.yml
 awsibox/cfg/ibox/res/efs/ibox_base.yml
 awsibox/cfg/ibox/res/elasticache/ibox_base.yml
 awsibox/cfg/ibox/res/elasticache/subnet-groups.yml
 awsibox/cfg/ibox/res/elasticloadbalancing/ibox_base.yml
-awsibox/cfg/ibox/res/elasticloadbalancing/listeners.yml
 awsibox/cfg/ibox/res/elasticloadbalancing/v2-listener-rules.yml
+awsibox/cfg/ibox/res/elasticloadbalancing/v2-listeners.yml
 awsibox/cfg/ibox/res/elasticloadbalancing/v2-loadbalancers.yml
 awsibox/cfg/ibox/res/elasticloadbalancing/v2-targetgroups.yml
 awsibox/cfg/ibox/res/events/ibox_base.yml
 awsibox/cfg/ibox/res/iam/ibox_base.yml
 awsibox/cfg/ibox/res/iam/instance-profiles.yml
 awsibox/cfg/ibox/res/iam/managed-policies.yml
 awsibox/cfg/ibox/res/iam/policies.yml
 awsibox/cfg/ibox/res/iam/roles.yml
 awsibox/cfg/ibox/res/lambda/functions.yml
 awsibox/cfg/ibox/res/lambda/ibox_base.yml
 awsibox/cfg/ibox/res/lambda/layer_permissions.yml
 awsibox/cfg/ibox/res/lambda/permissions.yml
 awsibox/cfg/ibox/res/lambda/versions.yml
+awsibox/cfg/ibox/res/rds/db-parameter_groups.yml
 awsibox/cfg/ibox/res/rds/db-subnet-groups.yml
 awsibox/cfg/ibox/res/rds/ibox_base.yml
 awsibox/cfg/ibox/res/route53/hostedzones.yml
 awsibox/cfg/ibox/res/route53/ibox_base.yml
 awsibox/cfg/ibox/res/route53/recordsets.yml
 awsibox/cfg/ibox/res/s3/bucket-policies.yml
 awsibox/cfg/ibox/res/s3/ibox_base.yml
@@ -187,22 +193,25 @@
 awsibox/lambdas/ServiceDiscovery.code
 awsibox/lambdas/ServiceUnavailable.code
 awsibox/lambdas/StacksOps.code
 awsibox/mod/autoscaling.py
 awsibox/mod/cloudformation.py
 awsibox/mod/cloudfront.py
 awsibox/mod/ec2.py
-awsibox/mod/ecr.py
-awsibox/mod/efs.py
-awsibox/mod/elasticloadbalancing.py
-awsibox/mod/iam.py
 awsibox/mod/joker.py
-awsibox/mod/rds.py
-awsibox/mod/s3.py
-awsibox/mod/waf.py
+awsibox/mod/__pycache__/autoscaling.cpython-311.pyc
+awsibox/mod/__pycache__/cloudformation.cpython-311.pyc
+awsibox/mod/__pycache__/cloudfront.cpython-311.pyc
+awsibox/mod/__pycache__/ec2.cpython-311.pyc
+awsibox/mod/__pycache__/elasticloadbalancing.cpython-311.pyc
+awsibox/mod/__pycache__/iam.cpython-311.pyc
+awsibox/mod/__pycache__/joker.cpython-311.pyc
+awsibox/mod/__pycache__/rds.cpython-311.pyc
+awsibox/mod/__pycache__/s3.cpython-311.pyc
+awsibox/mod/__pycache__/waf.cpython-311.pyc
 awsibox/user-data/ecs-cluster.sh
 awsibox/user-data/SCRIPTS/ELBCHECK.sh
 awsibox/user-data/SCRIPTS/END.sh
 awsibox/user-data/SCRIPTS/INIT.sh
 awsibox/user-data/SCRIPTS/PACKAGE.sh
 awsibox/user-data/SCRIPTS/SERVICE.sh
 awsibox/user-data/SCRIPTS/SETUP.sh
```

### Comparing `awsibox-0.8.7/scripts/ibox_generate_templates.py` & `awsibox-0.8.8/scripts/ibox_generate_templates.py`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/setup.cfg` & `awsibox-0.8.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `awsibox-0.8.7/setup.py` & `awsibox-0.8.8/setup.py`

 * *Files identical despite different names*

