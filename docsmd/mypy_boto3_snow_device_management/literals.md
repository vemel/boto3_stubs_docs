# Literals

> [Index](../README.md) > [SnowDeviceManagement](./README.md) > Literals

!!! note ""

    Auto-generated documentation for [SnowDeviceManagement](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/snow-device-management.html#SnowDeviceManagement)
    type annotations stubs module [mypy-boto3-snow-device-management](https://pypi.org/project/mypy-boto3-snow-device-management/).

## AttachmentStatusType

```python title="Usage Example"
from mypy_boto3_snow_device_management.literals import AttachmentStatusType

def get_value() -> AttachmentStatusType:
    return "ATTACHED"
```

```python title="Definition"
AttachmentStatusType = Literal[
    "ATTACHED",
    "ATTACHING",
    "DETACHED",
    "DETACHING",
]
```
## ExecutionStateType

```python title="Usage Example"
from mypy_boto3_snow_device_management.literals import ExecutionStateType

def get_value() -> ExecutionStateType:
    return "CANCELED"
```

```python title="Definition"
ExecutionStateType = Literal[
    "CANCELED",
    "FAILED",
    "IN_PROGRESS",
    "QUEUED",
    "REJECTED",
    "SUCCEEDED",
    "TIMED_OUT",
]
```
## InstanceStateNameType

```python title="Usage Example"
from mypy_boto3_snow_device_management.literals import InstanceStateNameType

def get_value() -> InstanceStateNameType:
    return "PENDING"
```

```python title="Definition"
InstanceStateNameType = Literal[
    "PENDING",
    "RUNNING",
    "SHUTTING_DOWN",
    "STOPPED",
    "STOPPING",
    "TERMINATED",
]
```
## IpAddressAssignmentType

```python title="Usage Example"
from mypy_boto3_snow_device_management.literals import IpAddressAssignmentType

def get_value() -> IpAddressAssignmentType:
    return "DHCP"
```

```python title="Definition"
IpAddressAssignmentType = Literal[
    "DHCP",
    "STATIC",
]
```
## ListDeviceResourcesPaginatorName

```python title="Usage Example"
from mypy_boto3_snow_device_management.literals import ListDeviceResourcesPaginatorName

def get_value() -> ListDeviceResourcesPaginatorName:
    return "list_device_resources"
```

```python title="Definition"
ListDeviceResourcesPaginatorName = Literal[
    "list_device_resources",
]
```
## ListDevicesPaginatorName

```python title="Usage Example"
from mypy_boto3_snow_device_management.literals import ListDevicesPaginatorName

def get_value() -> ListDevicesPaginatorName:
    return "list_devices"
```

```python title="Definition"
ListDevicesPaginatorName = Literal[
    "list_devices",
]
```
## ListExecutionsPaginatorName

```python title="Usage Example"
from mypy_boto3_snow_device_management.literals import ListExecutionsPaginatorName

def get_value() -> ListExecutionsPaginatorName:
    return "list_executions"
```

```python title="Definition"
ListExecutionsPaginatorName = Literal[
    "list_executions",
]
```
## ListTasksPaginatorName

```python title="Usage Example"
from mypy_boto3_snow_device_management.literals import ListTasksPaginatorName

def get_value() -> ListTasksPaginatorName:
    return "list_tasks"
```

```python title="Definition"
ListTasksPaginatorName = Literal[
    "list_tasks",
]
```
## PhysicalConnectorTypeType

```python title="Usage Example"
from mypy_boto3_snow_device_management.literals import PhysicalConnectorTypeType

def get_value() -> PhysicalConnectorTypeType:
    return "QSFP"
```

```python title="Definition"
PhysicalConnectorTypeType = Literal[
    "QSFP",
    "RJ45",
    "RJ45_2",
    "SFP_PLUS",
    "WIFI",
]
```
## TaskStateType

```python title="Usage Example"
from mypy_boto3_snow_device_management.literals import TaskStateType

def get_value() -> TaskStateType:
    return "CANCELED"
```

```python title="Definition"
TaskStateType = Literal[
    "CANCELED",
    "COMPLETED",
    "IN_PROGRESS",
]
```
## UnlockStateType

```python title="Usage Example"
from mypy_boto3_snow_device_management.literals import UnlockStateType

def get_value() -> UnlockStateType:
    return "LOCKED"
```

```python title="Definition"
UnlockStateType = Literal[
    "LOCKED",
    "UNLOCKED",
    "UNLOCKING",
]
```
## SnowDeviceManagementServiceName

```python title="Usage Example"
from mypy_boto3_snow_device_management.literals import SnowDeviceManagementServiceName

def get_value() -> SnowDeviceManagementServiceName:
    return "snow-device-management"
```

```python title="Definition"
SnowDeviceManagementServiceName = Literal[
    "snow-device-management",
]
```
## ServiceName

```python title="Usage Example"
from mypy_boto3_snow_device_management.literals import ServiceName

def get_value() -> ServiceName:
    return "accessanalyzer"
```

```python title="Definition"
ServiceName = Literal[
    "accessanalyzer",
    "account",
    "acm",
    "acm-pca",
    "alexaforbusiness",
    "amp",
    "amplify",
    "amplifybackend",
    "amplifyuibuilder",
    "apigateway",
    "apigatewaymanagementapi",
    "apigatewayv2",
    "appconfig",
    "appconfigdata",
    "appflow",
    "appintegrations",
    "application-autoscaling",
    "application-insights",
    "applicationcostprofiler",
    "appmesh",
    "apprunner",
    "appstream",
    "appsync",
    "athena",
    "auditmanager",
    "autoscaling",
    "autoscaling-plans",
    "backup",
    "backup-gateway",
    "batch",
    "billingconductor",
    "braket",
    "budgets",
    "ce",
    "chime",
    "chime-sdk-identity",
    "chime-sdk-meetings",
    "chime-sdk-messaging",
    "cloud9",
    "cloudcontrol",
    "clouddirectory",
    "cloudformation",
    "cloudfront",
    "cloudhsm",
    "cloudhsmv2",
    "cloudsearch",
    "cloudsearchdomain",
    "cloudtrail",
    "cloudwatch",
    "codeartifact",
    "codebuild",
    "codecommit",
    "codedeploy",
    "codeguru-reviewer",
    "codeguruprofiler",
    "codepipeline",
    "codestar",
    "codestar-connections",
    "codestar-notifications",
    "cognito-identity",
    "cognito-idp",
    "cognito-sync",
    "comprehend",
    "comprehendmedical",
    "compute-optimizer",
    "config",
    "connect",
    "connect-contact-lens",
    "connectparticipant",
    "cur",
    "customer-profiles",
    "databrew",
    "dataexchange",
    "datapipeline",
    "datasync",
    "dax",
    "detective",
    "devicefarm",
    "devops-guru",
    "directconnect",
    "discovery",
    "dlm",
    "dms",
    "docdb",
    "drs",
    "ds",
    "dynamodb",
    "dynamodbstreams",
    "ebs",
    "ec2",
    "ec2-instance-connect",
    "ecr",
    "ecr-public",
    "ecs",
    "efs",
    "eks",
    "elastic-inference",
    "elasticache",
    "elasticbeanstalk",
    "elastictranscoder",
    "elb",
    "elbv2",
    "emr",
    "emr-containers",
    "es",
    "events",
    "evidently",
    "finspace",
    "finspace-data",
    "firehose",
    "fis",
    "fms",
    "forecast",
    "forecastquery",
    "frauddetector",
    "fsx",
    "gamelift",
    "gamesparks",
    "glacier",
    "globalaccelerator",
    "glue",
    "grafana",
    "greengrass",
    "greengrassv2",
    "groundstation",
    "guardduty",
    "health",
    "healthlake",
    "honeycode",
    "iam",
    "identitystore",
    "imagebuilder",
    "importexport",
    "inspector",
    "inspector2",
    "iot",
    "iot-data",
    "iot-jobs-data",
    "iot1click-devices",
    "iot1click-projects",
    "iotanalytics",
    "iotdeviceadvisor",
    "iotevents",
    "iotevents-data",
    "iotfleethub",
    "iotsecuretunneling",
    "iotsitewise",
    "iotthingsgraph",
    "iottwinmaker",
    "iotwireless",
    "ivs",
    "kafka",
    "kafkaconnect",
    "kendra",
    "keyspaces",
    "kinesis",
    "kinesis-video-archived-media",
    "kinesis-video-media",
    "kinesis-video-signaling",
    "kinesisanalytics",
    "kinesisanalyticsv2",
    "kinesisvideo",
    "kms",
    "lakeformation",
    "lambda",
    "lex-models",
    "lex-runtime",
    "lexv2-models",
    "lexv2-runtime",
    "license-manager",
    "lightsail",
    "location",
    "logs",
    "lookoutequipment",
    "lookoutmetrics",
    "lookoutvision",
    "machinelearning",
    "macie",
    "macie2",
    "managedblockchain",
    "marketplace-catalog",
    "marketplace-entitlement",
    "marketplacecommerceanalytics",
    "mediaconnect",
    "mediaconvert",
    "medialive",
    "mediapackage",
    "mediapackage-vod",
    "mediastore",
    "mediastore-data",
    "mediatailor",
    "memorydb",
    "meteringmarketplace",
    "mgh",
    "mgn",
    "migration-hub-refactor-spaces",
    "migrationhub-config",
    "migrationhubstrategy",
    "mobile",
    "mq",
    "mturk",
    "mwaa",
    "neptune",
    "network-firewall",
    "networkmanager",
    "nimble",
    "opensearch",
    "opsworks",
    "opsworkscm",
    "organizations",
    "outposts",
    "panorama",
    "personalize",
    "personalize-events",
    "personalize-runtime",
    "pi",
    "pinpoint",
    "pinpoint-email",
    "pinpoint-sms-voice",
    "pinpoint-sms-voice-v2",
    "polly",
    "pricing",
    "proton",
    "qldb",
    "qldb-session",
    "quicksight",
    "ram",
    "rbin",
    "rds",
    "rds-data",
    "redshift",
    "redshift-data",
    "rekognition",
    "resiliencehub",
    "resource-groups",
    "resourcegroupstaggingapi",
    "robomaker",
    "route53",
    "route53-recovery-cluster",
    "route53-recovery-control-config",
    "route53-recovery-readiness",
    "route53domains",
    "route53resolver",
    "rum",
    "s3",
    "s3control",
    "s3outposts",
    "sagemaker",
    "sagemaker-a2i-runtime",
    "sagemaker-edge",
    "sagemaker-featurestore-runtime",
    "sagemaker-runtime",
    "savingsplans",
    "schemas",
    "sdb",
    "secretsmanager",
    "securityhub",
    "serverlessrepo",
    "service-quotas",
    "servicecatalog",
    "servicecatalog-appregistry",
    "servicediscovery",
    "ses",
    "sesv2",
    "shield",
    "signer",
    "sms",
    "sms-voice",
    "snow-device-management",
    "snowball",
    "sns",
    "sqs",
    "ssm",
    "ssm-contacts",
    "ssm-incidents",
    "sso",
    "sso-admin",
    "sso-oidc",
    "stepfunctions",
    "storagegateway",
    "sts",
    "support",
    "swf",
    "synthetics",
    "textract",
    "timestream-query",
    "timestream-write",
    "transcribe",
    "transfer",
    "translate",
    "voice-id",
    "waf",
    "waf-regional",
    "wafv2",
    "wellarchitected",
    "wisdom",
    "workdocs",
    "worklink",
    "workmail",
    "workmailmessageflow",
    "workspaces",
    "workspaces-web",
    "xray",
]
```
## ResourceServiceName

```python title="Usage Example"
from mypy_boto3_snow_device_management.literals import ResourceServiceName

def get_value() -> ResourceServiceName:
    return "cloudformation"
```

```python title="Definition"
ResourceServiceName = Literal[
    "cloudformation",
    "cloudwatch",
    "dynamodb",
    "ec2",
    "glacier",
    "iam",
    "opsworks",
    "s3",
    "sns",
    "sqs",
]
```
## PaginatorName

```python title="Usage Example"
from mypy_boto3_snow_device_management.literals import PaginatorName

def get_value() -> PaginatorName:
    return "list_device_resources"
```

```python title="Definition"
PaginatorName = Literal[
    "list_device_resources",
    "list_devices",
    "list_executions",
    "list_tasks",
]
```
