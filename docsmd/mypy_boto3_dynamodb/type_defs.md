# Typed dictionaries

> [Index](../README.md) > [DynamoDB](./README.md) > Typed dictionaries

!!! note ""

    Auto-generated documentation for [DynamoDB](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/dynamodb.html#DynamoDB)
    type annotations stubs module [mypy-boto3-dynamodb](https://pypi.org/project/mypy-boto3-dynamodb/).

## ArchivalSummaryResponseMetadataTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ArchivalSummaryResponseMetadataTypeDef

def get_value() -> ArchivalSummaryResponseMetadataTypeDef:
    return {
        "ArchivalDateTime": ...,
        "ArchivalReason": ...,
        "ArchivalBackupArn": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ArchivalSummaryResponseMetadataTypeDef(TypedDict):
    ArchivalDateTime: datetime,
    ArchivalReason: str,
    ArchivalBackupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ArchivalSummaryTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ArchivalSummaryTypeDef

def get_value() -> ArchivalSummaryTypeDef:
    return {
        "ArchivalDateTime": ...,
    }
```

```python title="Definition"
class ArchivalSummaryTypeDef(TypedDict):
    ArchivalDateTime: NotRequired[datetime],
    ArchivalReason: NotRequired[str],
    ArchivalBackupArn: NotRequired[str],
```

## AttributeDefinitionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import AttributeDefinitionTypeDef

def get_value() -> AttributeDefinitionTypeDef:
    return {
        "AttributeName": ...,
        "AttributeType": ...,
    }
```

```python title="Definition"
class AttributeDefinitionTypeDef(TypedDict):
    AttributeName: str,
    AttributeType: ScalarAttributeTypeType,  # (1)
```

1. See [:material-code-brackets: ScalarAttributeTypeType](./literals.md#scalarattributetypetype) 
## AttributeValueUpdateTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import AttributeValueUpdateTypeDef

def get_value() -> AttributeValueUpdateTypeDef:
    return {
        "Value": ...,
    }
```

```python title="Definition"
class AttributeValueUpdateTypeDef(TypedDict):
    Value: NotRequired[Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    Action: NotRequired[AttributeActionType],  # (1)
```

1. See [:material-code-brackets: AttributeActionType](./literals.md#attributeactiontype) 
## AutoScalingPolicyDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import AutoScalingPolicyDescriptionTypeDef

def get_value() -> AutoScalingPolicyDescriptionTypeDef:
    return {
        "PolicyName": ...,
    }
```

```python title="Definition"
class AutoScalingPolicyDescriptionTypeDef(TypedDict):
    PolicyName: NotRequired[str],
    TargetTrackingScalingPolicyConfiguration: NotRequired[AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef](./type_defs.md#autoscalingtargettrackingscalingpolicyconfigurationdescriptiontypedef) 
## AutoScalingPolicyUpdateTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import AutoScalingPolicyUpdateTypeDef

def get_value() -> AutoScalingPolicyUpdateTypeDef:
    return {
        "TargetTrackingScalingPolicyConfiguration": ...,
    }
```

```python title="Definition"
class AutoScalingPolicyUpdateTypeDef(TypedDict):
    TargetTrackingScalingPolicyConfiguration: AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef,  # (1)
    PolicyName: NotRequired[str],
```

1. See [:material-code-braces: AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef](./type_defs.md#autoscalingtargettrackingscalingpolicyconfigurationupdatetypedef) 
## AutoScalingSettingsDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import AutoScalingSettingsDescriptionTypeDef

def get_value() -> AutoScalingSettingsDescriptionTypeDef:
    return {
        "MinimumUnits": ...,
    }
```

```python title="Definition"
class AutoScalingSettingsDescriptionTypeDef(TypedDict):
    MinimumUnits: NotRequired[int],
    MaximumUnits: NotRequired[int],
    AutoScalingDisabled: NotRequired[bool],
    AutoScalingRoleArn: NotRequired[str],
    ScalingPolicies: NotRequired[List[AutoScalingPolicyDescriptionTypeDef]],  # (1)
```

1. See [:material-code-braces: AutoScalingPolicyDescriptionTypeDef](./type_defs.md#autoscalingpolicydescriptiontypedef) 
## AutoScalingSettingsUpdateTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import AutoScalingSettingsUpdateTypeDef

def get_value() -> AutoScalingSettingsUpdateTypeDef:
    return {
        "MinimumUnits": ...,
    }
```

```python title="Definition"
class AutoScalingSettingsUpdateTypeDef(TypedDict):
    MinimumUnits: NotRequired[int],
    MaximumUnits: NotRequired[int],
    AutoScalingDisabled: NotRequired[bool],
    AutoScalingRoleArn: NotRequired[str],
    ScalingPolicyUpdate: NotRequired[AutoScalingPolicyUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingPolicyUpdateTypeDef](./type_defs.md#autoscalingpolicyupdatetypedef) 
## AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef

def get_value() -> AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef:
    return {
        "TargetValue": ...,
    }
```

```python title="Definition"
class AutoScalingTargetTrackingScalingPolicyConfigurationDescriptionTypeDef(TypedDict):
    TargetValue: float,
    DisableScaleIn: NotRequired[bool],
    ScaleInCooldown: NotRequired[int],
    ScaleOutCooldown: NotRequired[int],
```

## AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef

def get_value() -> AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef:
    return {
        "TargetValue": ...,
    }
```

```python title="Definition"
class AutoScalingTargetTrackingScalingPolicyConfigurationUpdateTypeDef(TypedDict):
    TargetValue: float,
    DisableScaleIn: NotRequired[bool],
    ScaleInCooldown: NotRequired[int],
    ScaleOutCooldown: NotRequired[int],
```

## BackupDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import BackupDescriptionTypeDef

def get_value() -> BackupDescriptionTypeDef:
    return {
        "BackupDetails": ...,
    }
```

```python title="Definition"
class BackupDescriptionTypeDef(TypedDict):
    BackupDetails: NotRequired[BackupDetailsTypeDef],  # (1)
    SourceTableDetails: NotRequired[SourceTableDetailsTypeDef],  # (2)
    SourceTableFeatureDetails: NotRequired[SourceTableFeatureDetailsTypeDef],  # (3)
```

1. See [:material-code-braces: BackupDetailsTypeDef](./type_defs.md#backupdetailstypedef) 
2. See [:material-code-braces: SourceTableDetailsTypeDef](./type_defs.md#sourcetabledetailstypedef) 
3. See [:material-code-braces: SourceTableFeatureDetailsTypeDef](./type_defs.md#sourcetablefeaturedetailstypedef) 
## BackupDetailsTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import BackupDetailsTypeDef

def get_value() -> BackupDetailsTypeDef:
    return {
        "BackupArn": ...,
        "BackupName": ...,
        "BackupStatus": ...,
        "BackupType": ...,
        "BackupCreationDateTime": ...,
    }
```

```python title="Definition"
class BackupDetailsTypeDef(TypedDict):
    BackupArn: str,
    BackupName: str,
    BackupStatus: BackupStatusType,  # (1)
    BackupType: BackupTypeType,  # (2)
    BackupCreationDateTime: datetime,
    BackupSizeBytes: NotRequired[int],
    BackupExpiryDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: BackupStatusType](./literals.md#backupstatustype) 
2. See [:material-code-brackets: BackupTypeType](./literals.md#backuptypetype) 
## BackupSummaryTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import BackupSummaryTypeDef

def get_value() -> BackupSummaryTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class BackupSummaryTypeDef(TypedDict):
    TableName: NotRequired[str],
    TableId: NotRequired[str],
    TableArn: NotRequired[str],
    BackupArn: NotRequired[str],
    BackupName: NotRequired[str],
    BackupCreationDateTime: NotRequired[datetime],
    BackupExpiryDateTime: NotRequired[datetime],
    BackupStatus: NotRequired[BackupStatusType],  # (1)
    BackupType: NotRequired[BackupTypeType],  # (2)
    BackupSizeBytes: NotRequired[int],
```

1. See [:material-code-brackets: BackupStatusType](./literals.md#backupstatustype) 
2. See [:material-code-brackets: BackupTypeType](./literals.md#backuptypetype) 
## BatchExecuteStatementInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import BatchExecuteStatementInputRequestTypeDef

def get_value() -> BatchExecuteStatementInputRequestTypeDef:
    return {
        "Statements": ...,
    }
```

```python title="Definition"
class BatchExecuteStatementInputRequestTypeDef(TypedDict):
    Statements: Sequence[BatchStatementRequestTypeDef],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
```

1. See [:material-code-braces: BatchStatementRequestTypeDef](./type_defs.md#batchstatementrequesttypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## BatchExecuteStatementOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import BatchExecuteStatementOutputTypeDef

def get_value() -> BatchExecuteStatementOutputTypeDef:
    return {
        "Responses": ...,
        "ConsumedCapacity": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class BatchExecuteStatementOutputTypeDef(TypedDict):
    Responses: List[BatchStatementResponseTypeDef],  # (1)
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: BatchStatementResponseTypeDef](./type_defs.md#batchstatementresponsetypedef) 
2. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetItemInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import BatchGetItemInputRequestTypeDef

def get_value() -> BatchGetItemInputRequestTypeDef:
    return {
        "RequestItems": ...,
    }
```

```python title="Definition"
class BatchGetItemInputRequestTypeDef(TypedDict):
    RequestItems: Mapping[str, KeysAndAttributesTypeDef],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
```

1. See [:material-code-braces: KeysAndAttributesTypeDef](./type_defs.md#keysandattributestypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## BatchGetItemInputServiceResourceBatchGetItemTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import BatchGetItemInputServiceResourceBatchGetItemTypeDef

def get_value() -> BatchGetItemInputServiceResourceBatchGetItemTypeDef:
    return {
        "RequestItems": ...,
    }
```

```python title="Definition"
class BatchGetItemInputServiceResourceBatchGetItemTypeDef(TypedDict):
    RequestItems: Mapping[str, KeysAndAttributesTypeDef],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
```

1. See [:material-code-braces: KeysAndAttributesTypeDef](./type_defs.md#keysandattributestypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## BatchGetItemOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import BatchGetItemOutputTypeDef

def get_value() -> BatchGetItemOutputTypeDef:
    return {
        "Responses": ...,
        "UnprocessedKeys": ...,
        "ConsumedCapacity": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class BatchGetItemOutputTypeDef(TypedDict):
    Responses: Dict[str, List[Dict[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]]],
    UnprocessedKeys: Dict[str, KeysAndAttributesTypeDef],  # (1)
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: KeysAndAttributesTypeDef](./type_defs.md#keysandattributestypedef) 
2. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchStatementErrorTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import BatchStatementErrorTypeDef

def get_value() -> BatchStatementErrorTypeDef:
    return {
        "Code": ...,
    }
```

```python title="Definition"
class BatchStatementErrorTypeDef(TypedDict):
    Code: NotRequired[BatchStatementErrorCodeEnumType],  # (1)
    Message: NotRequired[str],
```

1. See [:material-code-brackets: BatchStatementErrorCodeEnumType](./literals.md#batchstatementerrorcodeenumtype) 
## BatchStatementRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import BatchStatementRequestTypeDef

def get_value() -> BatchStatementRequestTypeDef:
    return {
        "Statement": ...,
    }
```

```python title="Definition"
class BatchStatementRequestTypeDef(TypedDict):
    Statement: str,
    Parameters: NotRequired[Sequence[Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
    ConsistentRead: NotRequired[bool],
```

## BatchStatementResponseTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import BatchStatementResponseTypeDef

def get_value() -> BatchStatementResponseTypeDef:
    return {
        "Error": ...,
    }
```

```python title="Definition"
class BatchStatementResponseTypeDef(TypedDict):
    Error: NotRequired[BatchStatementErrorTypeDef],  # (1)
    TableName: NotRequired[str],
    Item: NotRequired[Dict[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
```

1. See [:material-code-braces: BatchStatementErrorTypeDef](./type_defs.md#batchstatementerrortypedef) 
## BatchWriteItemInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import BatchWriteItemInputRequestTypeDef

def get_value() -> BatchWriteItemInputRequestTypeDef:
    return {
        "RequestItems": ...,
    }
```

```python title="Definition"
class BatchWriteItemInputRequestTypeDef(TypedDict):
    RequestItems: Mapping[str, Sequence[WriteRequestTypeDef]],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (3)
```

1. See [:material-code-braces: WriteRequestTypeDef](./type_defs.md#writerequesttypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
3. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
## BatchWriteItemInputServiceResourceBatchWriteItemTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import BatchWriteItemInputServiceResourceBatchWriteItemTypeDef

def get_value() -> BatchWriteItemInputServiceResourceBatchWriteItemTypeDef:
    return {
        "RequestItems": ...,
    }
```

```python title="Definition"
class BatchWriteItemInputServiceResourceBatchWriteItemTypeDef(TypedDict):
    RequestItems: Mapping[str, Sequence[WriteRequestTypeDef]],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (3)
```

1. See [:material-code-braces: WriteRequestTypeDef](./type_defs.md#writerequesttypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
3. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
## BatchWriteItemOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import BatchWriteItemOutputTypeDef

def get_value() -> BatchWriteItemOutputTypeDef:
    return {
        "UnprocessedItems": ...,
        "ItemCollectionMetrics": ...,
        "ConsumedCapacity": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class BatchWriteItemOutputTypeDef(TypedDict):
    UnprocessedItems: Dict[str, List[WriteRequestTypeDef]],  # (1)
    ItemCollectionMetrics: Dict[str, List[ItemCollectionMetricsTypeDef]],  # (2)
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (3)
    ResponseMetadata: ResponseMetadataTypeDef,  # (4)
```

1. See [:material-code-braces: WriteRequestTypeDef](./type_defs.md#writerequesttypedef) 
2. See [:material-code-braces: ItemCollectionMetricsTypeDef](./type_defs.md#itemcollectionmetricstypedef) 
3. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
4. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BillingModeSummaryResponseMetadataTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import BillingModeSummaryResponseMetadataTypeDef

def get_value() -> BillingModeSummaryResponseMetadataTypeDef:
    return {
        "BillingMode": ...,
        "LastUpdateToPayPerRequestDateTime": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class BillingModeSummaryResponseMetadataTypeDef(TypedDict):
    BillingMode: BillingModeType,  # (1)
    LastUpdateToPayPerRequestDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BillingModeSummaryTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import BillingModeSummaryTypeDef

def get_value() -> BillingModeSummaryTypeDef:
    return {
        "BillingMode": ...,
    }
```

```python title="Definition"
class BillingModeSummaryTypeDef(TypedDict):
    BillingMode: NotRequired[BillingModeType],  # (1)
    LastUpdateToPayPerRequestDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
## CapacityTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import CapacityTypeDef

def get_value() -> CapacityTypeDef:
    return {
        "ReadCapacityUnits": ...,
    }
```

```python title="Definition"
class CapacityTypeDef(TypedDict):
    ReadCapacityUnits: NotRequired[float],
    WriteCapacityUnits: NotRequired[float],
    CapacityUnits: NotRequired[float],
```

## ConditionCheckTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ConditionCheckTypeDef

def get_value() -> ConditionCheckTypeDef:
    return {
        "Key": ...,
        "TableName": ...,
        "ConditionExpression": ...,
    }
```

```python title="Definition"
class ConditionCheckTypeDef(TypedDict):
    Key: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    TableName: str,
    ConditionExpression: str,
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (1)
```

1. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## ConditionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ConditionTypeDef

def get_value() -> ConditionTypeDef:
    return {
        "ComparisonOperator": ...,
    }
```

```python title="Definition"
class ConditionTypeDef(TypedDict):
    ComparisonOperator: ComparisonOperatorType,  # (1)
    AttributeValueList: NotRequired[Sequence[Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## ConsumedCapacityTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ConsumedCapacityTypeDef

def get_value() -> ConsumedCapacityTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class ConsumedCapacityTypeDef(TypedDict):
    TableName: NotRequired[str],
    CapacityUnits: NotRequired[float],
    ReadCapacityUnits: NotRequired[float],
    WriteCapacityUnits: NotRequired[float],
    Table: NotRequired[CapacityTypeDef],  # (1)
    LocalSecondaryIndexes: NotRequired[Dict[str, CapacityTypeDef]],  # (2)
    GlobalSecondaryIndexes: NotRequired[Dict[str, CapacityTypeDef]],  # (2)
```

1. See [:material-code-braces: CapacityTypeDef](./type_defs.md#capacitytypedef) 
2. See [:material-code-braces: CapacityTypeDef](./type_defs.md#capacitytypedef) 
3. See [:material-code-braces: CapacityTypeDef](./type_defs.md#capacitytypedef) 
## ContinuousBackupsDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ContinuousBackupsDescriptionTypeDef

def get_value() -> ContinuousBackupsDescriptionTypeDef:
    return {
        "ContinuousBackupsStatus": ...,
    }
```

```python title="Definition"
class ContinuousBackupsDescriptionTypeDef(TypedDict):
    ContinuousBackupsStatus: ContinuousBackupsStatusType,  # (1)
    PointInTimeRecoveryDescription: NotRequired[PointInTimeRecoveryDescriptionTypeDef],  # (2)
```

1. See [:material-code-brackets: ContinuousBackupsStatusType](./literals.md#continuousbackupsstatustype) 
2. See [:material-code-braces: PointInTimeRecoveryDescriptionTypeDef](./type_defs.md#pointintimerecoverydescriptiontypedef) 
## ContributorInsightsSummaryTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ContributorInsightsSummaryTypeDef

def get_value() -> ContributorInsightsSummaryTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class ContributorInsightsSummaryTypeDef(TypedDict):
    TableName: NotRequired[str],
    IndexName: NotRequired[str],
    ContributorInsightsStatus: NotRequired[ContributorInsightsStatusType],  # (1)
```

1. See [:material-code-brackets: ContributorInsightsStatusType](./literals.md#contributorinsightsstatustype) 
## CreateBackupInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import CreateBackupInputRequestTypeDef

def get_value() -> CreateBackupInputRequestTypeDef:
    return {
        "TableName": ...,
        "BackupName": ...,
    }
```

```python title="Definition"
class CreateBackupInputRequestTypeDef(TypedDict):
    TableName: str,
    BackupName: str,
```

## CreateBackupOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import CreateBackupOutputTypeDef

def get_value() -> CreateBackupOutputTypeDef:
    return {
        "BackupDetails": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class CreateBackupOutputTypeDef(TypedDict):
    BackupDetails: BackupDetailsTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupDetailsTypeDef](./type_defs.md#backupdetailstypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateGlobalSecondaryIndexActionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import CreateGlobalSecondaryIndexActionTypeDef

def get_value() -> CreateGlobalSecondaryIndexActionTypeDef:
    return {
        "IndexName": ...,
        "KeySchema": ...,
        "Projection": ...,
    }
```

```python title="Definition"
class CreateGlobalSecondaryIndexActionTypeDef(TypedDict):
    IndexName: str,
    KeySchema: Sequence[KeySchemaElementTypeDef],  # (1)
    Projection: ProjectionTypeDef,  # (2)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (3)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionTypeDef](./type_defs.md#projectiontypedef) 
3. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
## CreateGlobalTableInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import CreateGlobalTableInputRequestTypeDef

def get_value() -> CreateGlobalTableInputRequestTypeDef:
    return {
        "GlobalTableName": ...,
        "ReplicationGroup": ...,
    }
```

```python title="Definition"
class CreateGlobalTableInputRequestTypeDef(TypedDict):
    GlobalTableName: str,
    ReplicationGroup: Sequence[ReplicaTypeDef],  # (1)
```

1. See [:material-code-braces: ReplicaTypeDef](./type_defs.md#replicatypedef) 
## CreateGlobalTableOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import CreateGlobalTableOutputTypeDef

def get_value() -> CreateGlobalTableOutputTypeDef:
    return {
        "GlobalTableDescription": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class CreateGlobalTableOutputTypeDef(TypedDict):
    GlobalTableDescription: GlobalTableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalTableDescriptionTypeDef](./type_defs.md#globaltabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreateReplicaActionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import CreateReplicaActionTypeDef

def get_value() -> CreateReplicaActionTypeDef:
    return {
        "RegionName": ...,
    }
```

```python title="Definition"
class CreateReplicaActionTypeDef(TypedDict):
    RegionName: str,
```

## CreateReplicationGroupMemberActionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import CreateReplicationGroupMemberActionTypeDef

def get_value() -> CreateReplicationGroupMemberActionTypeDef:
    return {
        "RegionName": ...,
    }
```

```python title="Definition"
class CreateReplicationGroupMemberActionTypeDef(TypedDict):
    RegionName: str,
    KMSMasterKeyId: NotRequired[str],
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputOverrideTypeDef],  # (1)
    GlobalSecondaryIndexes: NotRequired[Sequence[ReplicaGlobalSecondaryIndexTypeDef]],  # (2)
    TableClassOverride: NotRequired[TableClassType],  # (3)
```

1. See [:material-code-braces: ProvisionedThroughputOverrideTypeDef](./type_defs.md#provisionedthroughputoverridetypedef) 
2. See [:material-code-braces: ReplicaGlobalSecondaryIndexTypeDef](./type_defs.md#replicaglobalsecondaryindextypedef) 
3. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
## CreateTableInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import CreateTableInputRequestTypeDef

def get_value() -> CreateTableInputRequestTypeDef:
    return {
        "AttributeDefinitions": ...,
        "TableName": ...,
        "KeySchema": ...,
    }
```

```python title="Definition"
class CreateTableInputRequestTypeDef(TypedDict):
    AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],  # (1)
    TableName: str,
    KeySchema: Sequence[KeySchemaElementTypeDef],  # (2)
    LocalSecondaryIndexes: NotRequired[Sequence[LocalSecondaryIndexTypeDef]],  # (3)
    GlobalSecondaryIndexes: NotRequired[Sequence[GlobalSecondaryIndexTypeDef]],  # (4)
    BillingMode: NotRequired[BillingModeType],  # (5)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (6)
    StreamSpecification: NotRequired[StreamSpecificationTypeDef],  # (7)
    SSESpecification: NotRequired[SSESpecificationTypeDef],  # (8)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (9)
    TableClass: NotRequired[TableClassType],  # (10)
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
3. See [:material-code-braces: LocalSecondaryIndexTypeDef](./type_defs.md#localsecondaryindextypedef) 
4. See [:material-code-braces: GlobalSecondaryIndexTypeDef](./type_defs.md#globalsecondaryindextypedef) 
5. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
6. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
7. See [:material-code-braces: StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef) 
8. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
9. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
10. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
## CreateTableInputServiceResourceCreateTableTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import CreateTableInputServiceResourceCreateTableTypeDef

def get_value() -> CreateTableInputServiceResourceCreateTableTypeDef:
    return {
        "AttributeDefinitions": ...,
        "TableName": ...,
        "KeySchema": ...,
    }
```

```python title="Definition"
class CreateTableInputServiceResourceCreateTableTypeDef(TypedDict):
    AttributeDefinitions: Sequence[AttributeDefinitionTypeDef],  # (1)
    TableName: str,
    KeySchema: Sequence[KeySchemaElementTypeDef],  # (2)
    LocalSecondaryIndexes: NotRequired[Sequence[LocalSecondaryIndexTypeDef]],  # (3)
    GlobalSecondaryIndexes: NotRequired[Sequence[GlobalSecondaryIndexTypeDef]],  # (4)
    BillingMode: NotRequired[BillingModeType],  # (5)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (6)
    StreamSpecification: NotRequired[StreamSpecificationTypeDef],  # (7)
    SSESpecification: NotRequired[SSESpecificationTypeDef],  # (8)
    Tags: NotRequired[Sequence[TagTypeDef]],  # (9)
    TableClass: NotRequired[TableClassType],  # (10)
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
3. See [:material-code-braces: LocalSecondaryIndexTypeDef](./type_defs.md#localsecondaryindextypedef) 
4. See [:material-code-braces: GlobalSecondaryIndexTypeDef](./type_defs.md#globalsecondaryindextypedef) 
5. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
6. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
7. See [:material-code-braces: StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef) 
8. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
9. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
10. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
## CreateTableOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import CreateTableOutputTypeDef

def get_value() -> CreateTableOutputTypeDef:
    return {
        "TableDescription": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class CreateTableOutputTypeDef(TypedDict):
    TableDescription: TableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableDescriptionTypeDef](./type_defs.md#tabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteBackupInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DeleteBackupInputRequestTypeDef

def get_value() -> DeleteBackupInputRequestTypeDef:
    return {
        "BackupArn": ...,
    }
```

```python title="Definition"
class DeleteBackupInputRequestTypeDef(TypedDict):
    BackupArn: str,
```

## DeleteBackupOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DeleteBackupOutputTypeDef

def get_value() -> DeleteBackupOutputTypeDef:
    return {
        "BackupDescription": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DeleteBackupOutputTypeDef(TypedDict):
    BackupDescription: BackupDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupDescriptionTypeDef](./type_defs.md#backupdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteGlobalSecondaryIndexActionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DeleteGlobalSecondaryIndexActionTypeDef

def get_value() -> DeleteGlobalSecondaryIndexActionTypeDef:
    return {
        "IndexName": ...,
    }
```

```python title="Definition"
class DeleteGlobalSecondaryIndexActionTypeDef(TypedDict):
    IndexName: str,
```

## DeleteItemInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DeleteItemInputRequestTypeDef

def get_value() -> DeleteItemInputRequestTypeDef:
    return {
        "TableName": ...,
        "Key": ...,
    }
```

```python title="Definition"
class DeleteItemInputRequestTypeDef(TypedDict):
    TableName: str,
    Key: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    Expected: NotRequired[Mapping[str, ExpectedAttributeValueTypeDef]],  # (1)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (2)
    ReturnValues: NotRequired[ReturnValueType],  # (3)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (4)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (5)
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
```

1. See [:material-code-braces: ExpectedAttributeValueTypeDef](./type_defs.md#expectedattributevaluetypedef) 
2. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
3. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
4. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
5. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
## DeleteItemInputTableDeleteItemTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DeleteItemInputTableDeleteItemTypeDef

def get_value() -> DeleteItemInputTableDeleteItemTypeDef:
    return {
        "Key": ...,
    }
```

```python title="Definition"
class DeleteItemInputTableDeleteItemTypeDef(TypedDict):
    Key: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    Expected: NotRequired[Mapping[str, ExpectedAttributeValueTypeDef]],  # (1)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (2)
    ReturnValues: NotRequired[ReturnValueType],  # (3)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (4)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (5)
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
```

1. See [:material-code-braces: ExpectedAttributeValueTypeDef](./type_defs.md#expectedattributevaluetypedef) 
2. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
3. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
4. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
5. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
## DeleteItemOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DeleteItemOutputTypeDef

def get_value() -> DeleteItemOutputTypeDef:
    return {
        "Attributes": ...,
        "ConsumedCapacity": ...,
        "ItemCollectionMetrics": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DeleteItemOutputTypeDef(TypedDict):
    Attributes: Dict[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (1)
    ItemCollectionMetrics: ItemCollectionMetricsTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ItemCollectionMetricsTypeDef](./type_defs.md#itemcollectionmetricstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteReplicaActionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DeleteReplicaActionTypeDef

def get_value() -> DeleteReplicaActionTypeDef:
    return {
        "RegionName": ...,
    }
```

```python title="Definition"
class DeleteReplicaActionTypeDef(TypedDict):
    RegionName: str,
```

## DeleteReplicationGroupMemberActionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DeleteReplicationGroupMemberActionTypeDef

def get_value() -> DeleteReplicationGroupMemberActionTypeDef:
    return {
        "RegionName": ...,
    }
```

```python title="Definition"
class DeleteReplicationGroupMemberActionTypeDef(TypedDict):
    RegionName: str,
```

## DeleteRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DeleteRequestTypeDef

def get_value() -> DeleteRequestTypeDef:
    return {
        "Key": ...,
    }
```

```python title="Definition"
class DeleteRequestTypeDef(TypedDict):
    Key: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
```

## DeleteTableInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DeleteTableInputRequestTypeDef

def get_value() -> DeleteTableInputRequestTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class DeleteTableInputRequestTypeDef(TypedDict):
    TableName: str,
```

## DeleteTableOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DeleteTableOutputTypeDef

def get_value() -> DeleteTableOutputTypeDef:
    return {
        "TableDescription": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DeleteTableOutputTypeDef(TypedDict):
    TableDescription: TableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableDescriptionTypeDef](./type_defs.md#tabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DeleteTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DeleteTypeDef

def get_value() -> DeleteTypeDef:
    return {
        "Key": ...,
        "TableName": ...,
    }
```

```python title="Definition"
class DeleteTypeDef(TypedDict):
    Key: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    TableName: str,
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (1)
```

1. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## DescribeBackupInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeBackupInputRequestTypeDef

def get_value() -> DescribeBackupInputRequestTypeDef:
    return {
        "BackupArn": ...,
    }
```

```python title="Definition"
class DescribeBackupInputRequestTypeDef(TypedDict):
    BackupArn: str,
```

## DescribeBackupOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeBackupOutputTypeDef

def get_value() -> DescribeBackupOutputTypeDef:
    return {
        "BackupDescription": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DescribeBackupOutputTypeDef(TypedDict):
    BackupDescription: BackupDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupDescriptionTypeDef](./type_defs.md#backupdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeContinuousBackupsInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeContinuousBackupsInputRequestTypeDef

def get_value() -> DescribeContinuousBackupsInputRequestTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class DescribeContinuousBackupsInputRequestTypeDef(TypedDict):
    TableName: str,
```

## DescribeContinuousBackupsOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeContinuousBackupsOutputTypeDef

def get_value() -> DescribeContinuousBackupsOutputTypeDef:
    return {
        "ContinuousBackupsDescription": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DescribeContinuousBackupsOutputTypeDef(TypedDict):
    ContinuousBackupsDescription: ContinuousBackupsDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContinuousBackupsDescriptionTypeDef](./type_defs.md#continuousbackupsdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeContributorInsightsInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeContributorInsightsInputRequestTypeDef

def get_value() -> DescribeContributorInsightsInputRequestTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class DescribeContributorInsightsInputRequestTypeDef(TypedDict):
    TableName: str,
    IndexName: NotRequired[str],
```

## DescribeContributorInsightsOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeContributorInsightsOutputTypeDef

def get_value() -> DescribeContributorInsightsOutputTypeDef:
    return {
        "TableName": ...,
        "IndexName": ...,
        "ContributorInsightsRuleList": ...,
        "ContributorInsightsStatus": ...,
        "LastUpdateDateTime": ...,
        "FailureException": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DescribeContributorInsightsOutputTypeDef(TypedDict):
    TableName: str,
    IndexName: str,
    ContributorInsightsRuleList: List[str],
    ContributorInsightsStatus: ContributorInsightsStatusType,  # (1)
    LastUpdateDateTime: datetime,
    FailureException: FailureExceptionTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: ContributorInsightsStatusType](./literals.md#contributorinsightsstatustype) 
2. See [:material-code-braces: FailureExceptionTypeDef](./type_defs.md#failureexceptiontypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeEndpointsResponseTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeEndpointsResponseTypeDef

def get_value() -> DescribeEndpointsResponseTypeDef:
    return {
        "Endpoints": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DescribeEndpointsResponseTypeDef(TypedDict):
    Endpoints: List[EndpointTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EndpointTypeDef](./type_defs.md#endpointtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeExportInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeExportInputRequestTypeDef

def get_value() -> DescribeExportInputRequestTypeDef:
    return {
        "ExportArn": ...,
    }
```

```python title="Definition"
class DescribeExportInputRequestTypeDef(TypedDict):
    ExportArn: str,
```

## DescribeExportOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeExportOutputTypeDef

def get_value() -> DescribeExportOutputTypeDef:
    return {
        "ExportDescription": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DescribeExportOutputTypeDef(TypedDict):
    ExportDescription: ExportDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExportDescriptionTypeDef](./type_defs.md#exportdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGlobalTableInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeGlobalTableInputRequestTypeDef

def get_value() -> DescribeGlobalTableInputRequestTypeDef:
    return {
        "GlobalTableName": ...,
    }
```

```python title="Definition"
class DescribeGlobalTableInputRequestTypeDef(TypedDict):
    GlobalTableName: str,
```

## DescribeGlobalTableOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeGlobalTableOutputTypeDef

def get_value() -> DescribeGlobalTableOutputTypeDef:
    return {
        "GlobalTableDescription": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DescribeGlobalTableOutputTypeDef(TypedDict):
    GlobalTableDescription: GlobalTableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalTableDescriptionTypeDef](./type_defs.md#globaltabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeGlobalTableSettingsInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeGlobalTableSettingsInputRequestTypeDef

def get_value() -> DescribeGlobalTableSettingsInputRequestTypeDef:
    return {
        "GlobalTableName": ...,
    }
```

```python title="Definition"
class DescribeGlobalTableSettingsInputRequestTypeDef(TypedDict):
    GlobalTableName: str,
```

## DescribeGlobalTableSettingsOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeGlobalTableSettingsOutputTypeDef

def get_value() -> DescribeGlobalTableSettingsOutputTypeDef:
    return {
        "GlobalTableName": ...,
        "ReplicaSettings": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DescribeGlobalTableSettingsOutputTypeDef(TypedDict):
    GlobalTableName: str,
    ReplicaSettings: List[ReplicaSettingsDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicaSettingsDescriptionTypeDef](./type_defs.md#replicasettingsdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeKinesisStreamingDestinationInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeKinesisStreamingDestinationInputRequestTypeDef

def get_value() -> DescribeKinesisStreamingDestinationInputRequestTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class DescribeKinesisStreamingDestinationInputRequestTypeDef(TypedDict):
    TableName: str,
```

## DescribeKinesisStreamingDestinationOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeKinesisStreamingDestinationOutputTypeDef

def get_value() -> DescribeKinesisStreamingDestinationOutputTypeDef:
    return {
        "TableName": ...,
        "KinesisDataStreamDestinations": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DescribeKinesisStreamingDestinationOutputTypeDef(TypedDict):
    TableName: str,
    KinesisDataStreamDestinations: List[KinesisDataStreamDestinationTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: KinesisDataStreamDestinationTypeDef](./type_defs.md#kinesisdatastreamdestinationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeLimitsOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeLimitsOutputTypeDef

def get_value() -> DescribeLimitsOutputTypeDef:
    return {
        "AccountMaxReadCapacityUnits": ...,
        "AccountMaxWriteCapacityUnits": ...,
        "TableMaxReadCapacityUnits": ...,
        "TableMaxWriteCapacityUnits": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DescribeLimitsOutputTypeDef(TypedDict):
    AccountMaxReadCapacityUnits: int,
    AccountMaxWriteCapacityUnits: int,
    TableMaxReadCapacityUnits: int,
    TableMaxWriteCapacityUnits: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTableInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeTableInputRequestTypeDef

def get_value() -> DescribeTableInputRequestTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class DescribeTableInputRequestTypeDef(TypedDict):
    TableName: str,
```

## DescribeTableInputTableExistsWaitTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeTableInputTableExistsWaitTypeDef

def get_value() -> DescribeTableInputTableExistsWaitTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class DescribeTableInputTableExistsWaitTypeDef(TypedDict):
    TableName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeTableInputTableNotExistsWaitTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeTableInputTableNotExistsWaitTypeDef

def get_value() -> DescribeTableInputTableNotExistsWaitTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class DescribeTableInputTableNotExistsWaitTypeDef(TypedDict):
    TableName: str,
    WaiterConfig: NotRequired[WaiterConfigTypeDef],  # (1)
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 
## DescribeTableOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeTableOutputTypeDef

def get_value() -> DescribeTableOutputTypeDef:
    return {
        "Table": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DescribeTableOutputTypeDef(TypedDict):
    Table: TableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableDescriptionTypeDef](./type_defs.md#tabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTableReplicaAutoScalingInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeTableReplicaAutoScalingInputRequestTypeDef

def get_value() -> DescribeTableReplicaAutoScalingInputRequestTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class DescribeTableReplicaAutoScalingInputRequestTypeDef(TypedDict):
    TableName: str,
```

## DescribeTableReplicaAutoScalingOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeTableReplicaAutoScalingOutputTypeDef

def get_value() -> DescribeTableReplicaAutoScalingOutputTypeDef:
    return {
        "TableAutoScalingDescription": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DescribeTableReplicaAutoScalingOutputTypeDef(TypedDict):
    TableAutoScalingDescription: TableAutoScalingDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableAutoScalingDescriptionTypeDef](./type_defs.md#tableautoscalingdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## DescribeTimeToLiveInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeTimeToLiveInputRequestTypeDef

def get_value() -> DescribeTimeToLiveInputRequestTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class DescribeTimeToLiveInputRequestTypeDef(TypedDict):
    TableName: str,
```

## DescribeTimeToLiveOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import DescribeTimeToLiveOutputTypeDef

def get_value() -> DescribeTimeToLiveOutputTypeDef:
    return {
        "TimeToLiveDescription": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class DescribeTimeToLiveOutputTypeDef(TypedDict):
    TimeToLiveDescription: TimeToLiveDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TimeToLiveDescriptionTypeDef](./type_defs.md#timetolivedescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## EndpointTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import EndpointTypeDef

def get_value() -> EndpointTypeDef:
    return {
        "Address": ...,
        "CachePeriodInMinutes": ...,
    }
```

```python title="Definition"
class EndpointTypeDef(TypedDict):
    Address: str,
    CachePeriodInMinutes: int,
```

## ExecuteStatementInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ExecuteStatementInputRequestTypeDef

def get_value() -> ExecuteStatementInputRequestTypeDef:
    return {
        "Statement": ...,
    }
```

```python title="Definition"
class ExecuteStatementInputRequestTypeDef(TypedDict):
    Statement: str,
    Parameters: NotRequired[Sequence[Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
    ConsistentRead: NotRequired[bool],
    NextToken: NotRequired[str],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (1)
    Limit: NotRequired[int],
```

1. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## ExecuteStatementOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ExecuteStatementOutputTypeDef

def get_value() -> ExecuteStatementOutputTypeDef:
    return {
        "Items": ...,
        "NextToken": ...,
        "ConsumedCapacity": ...,
        "LastEvaluatedKey": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ExecuteStatementOutputTypeDef(TypedDict):
    Items: List[Dict[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
    NextToken: str,
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (1)
    LastEvaluatedKey: Dict[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExecuteTransactionInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ExecuteTransactionInputRequestTypeDef

def get_value() -> ExecuteTransactionInputRequestTypeDef:
    return {
        "TransactStatements": ...,
    }
```

```python title="Definition"
class ExecuteTransactionInputRequestTypeDef(TypedDict):
    TransactStatements: Sequence[ParameterizedStatementTypeDef],  # (1)
    ClientRequestToken: NotRequired[str],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
```

1. See [:material-code-braces: ParameterizedStatementTypeDef](./type_defs.md#parameterizedstatementtypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## ExecuteTransactionOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ExecuteTransactionOutputTypeDef

def get_value() -> ExecuteTransactionOutputTypeDef:
    return {
        "Responses": ...,
        "ConsumedCapacity": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ExecuteTransactionOutputTypeDef(TypedDict):
    Responses: List[ItemResponseTypeDef],  # (1)
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ItemResponseTypeDef](./type_defs.md#itemresponsetypedef) 
2. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ExpectedAttributeValueTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ExpectedAttributeValueTypeDef

def get_value() -> ExpectedAttributeValueTypeDef:
    return {
        "Value": ...,
    }
```

```python title="Definition"
class ExpectedAttributeValueTypeDef(TypedDict):
    Value: NotRequired[Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    Exists: NotRequired[bool],
    ComparisonOperator: NotRequired[ComparisonOperatorType],  # (1)
    AttributeValueList: NotRequired[Sequence[Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
```

1. See [:material-code-brackets: ComparisonOperatorType](./literals.md#comparisonoperatortype) 
## ExportDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ExportDescriptionTypeDef

def get_value() -> ExportDescriptionTypeDef:
    return {
        "ExportArn": ...,
    }
```

```python title="Definition"
class ExportDescriptionTypeDef(TypedDict):
    ExportArn: NotRequired[str],
    ExportStatus: NotRequired[ExportStatusType],  # (1)
    StartTime: NotRequired[datetime],
    EndTime: NotRequired[datetime],
    ExportManifest: NotRequired[str],
    TableArn: NotRequired[str],
    TableId: NotRequired[str],
    ExportTime: NotRequired[datetime],
    ClientToken: NotRequired[str],
    S3Bucket: NotRequired[str],
    S3BucketOwner: NotRequired[str],
    S3Prefix: NotRequired[str],
    S3SseAlgorithm: NotRequired[S3SseAlgorithmType],  # (2)
    S3SseKmsKeyId: NotRequired[str],
    FailureCode: NotRequired[str],
    FailureMessage: NotRequired[str],
    ExportFormat: NotRequired[ExportFormatType],  # (3)
    BilledSizeBytes: NotRequired[int],
    ItemCount: NotRequired[int],
```

1. See [:material-code-brackets: ExportStatusType](./literals.md#exportstatustype) 
2. See [:material-code-brackets: S3SseAlgorithmType](./literals.md#s3ssealgorithmtype) 
3. See [:material-code-brackets: ExportFormatType](./literals.md#exportformattype) 
## ExportSummaryTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ExportSummaryTypeDef

def get_value() -> ExportSummaryTypeDef:
    return {
        "ExportArn": ...,
    }
```

```python title="Definition"
class ExportSummaryTypeDef(TypedDict):
    ExportArn: NotRequired[str],
    ExportStatus: NotRequired[ExportStatusType],  # (1)
```

1. See [:material-code-brackets: ExportStatusType](./literals.md#exportstatustype) 
## ExportTableToPointInTimeInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ExportTableToPointInTimeInputRequestTypeDef

def get_value() -> ExportTableToPointInTimeInputRequestTypeDef:
    return {
        "TableArn": ...,
        "S3Bucket": ...,
    }
```

```python title="Definition"
class ExportTableToPointInTimeInputRequestTypeDef(TypedDict):
    TableArn: str,
    S3Bucket: str,
    ExportTime: NotRequired[Union[datetime, str]],
    ClientToken: NotRequired[str],
    S3BucketOwner: NotRequired[str],
    S3Prefix: NotRequired[str],
    S3SseAlgorithm: NotRequired[S3SseAlgorithmType],  # (1)
    S3SseKmsKeyId: NotRequired[str],
    ExportFormat: NotRequired[ExportFormatType],  # (2)
```

1. See [:material-code-brackets: S3SseAlgorithmType](./literals.md#s3ssealgorithmtype) 
2. See [:material-code-brackets: ExportFormatType](./literals.md#exportformattype) 
## ExportTableToPointInTimeOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ExportTableToPointInTimeOutputTypeDef

def get_value() -> ExportTableToPointInTimeOutputTypeDef:
    return {
        "ExportDescription": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ExportTableToPointInTimeOutputTypeDef(TypedDict):
    ExportDescription: ExportDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExportDescriptionTypeDef](./type_defs.md#exportdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## FailureExceptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import FailureExceptionTypeDef

def get_value() -> FailureExceptionTypeDef:
    return {
        "ExceptionName": ...,
    }
```

```python title="Definition"
class FailureExceptionTypeDef(TypedDict):
    ExceptionName: NotRequired[str],
    ExceptionDescription: NotRequired[str],
```

## GetItemInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import GetItemInputRequestTypeDef

def get_value() -> GetItemInputRequestTypeDef:
    return {
        "TableName": ...,
        "Key": ...,
    }
```

```python title="Definition"
class GetItemInputRequestTypeDef(TypedDict):
    TableName: str,
    Key: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    AttributesToGet: NotRequired[Sequence[str]],
    ConsistentRead: NotRequired[bool],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (1)
    ProjectionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## GetItemInputTableGetItemTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import GetItemInputTableGetItemTypeDef

def get_value() -> GetItemInputTableGetItemTypeDef:
    return {
        "Key": ...,
    }
```

```python title="Definition"
class GetItemInputTableGetItemTypeDef(TypedDict):
    Key: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    AttributesToGet: NotRequired[Sequence[str]],
    ConsistentRead: NotRequired[bool],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (1)
    ProjectionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## GetItemOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import GetItemOutputTypeDef

def get_value() -> GetItemOutputTypeDef:
    return {
        "Item": ...,
        "ConsumedCapacity": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetItemOutputTypeDef(TypedDict):
    Item: Dict[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import GetTypeDef

def get_value() -> GetTypeDef:
    return {
        "Key": ...,
        "TableName": ...,
    }
```

```python title="Definition"
class GetTypeDef(TypedDict):
    Key: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    TableName: str,
    ProjectionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
```

## GlobalSecondaryIndexAutoScalingUpdateTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import GlobalSecondaryIndexAutoScalingUpdateTypeDef

def get_value() -> GlobalSecondaryIndexAutoScalingUpdateTypeDef:
    return {
        "IndexName": ...,
    }
```

```python title="Definition"
class GlobalSecondaryIndexAutoScalingUpdateTypeDef(TypedDict):
    IndexName: NotRequired[str],
    ProvisionedWriteCapacityAutoScalingUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
## GlobalSecondaryIndexDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import GlobalSecondaryIndexDescriptionTypeDef

def get_value() -> GlobalSecondaryIndexDescriptionTypeDef:
    return {
        "IndexName": ...,
    }
```

```python title="Definition"
class GlobalSecondaryIndexDescriptionTypeDef(TypedDict):
    IndexName: NotRequired[str],
    KeySchema: NotRequired[List[KeySchemaElementTypeDef]],  # (1)
    Projection: NotRequired[ProjectionTypeDef],  # (2)
    IndexStatus: NotRequired[IndexStatusType],  # (3)
    Backfilling: NotRequired[bool],
    ProvisionedThroughput: NotRequired[ProvisionedThroughputDescriptionTypeDef],  # (4)
    IndexSizeBytes: NotRequired[int],
    ItemCount: NotRequired[int],
    IndexArn: NotRequired[str],
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionTypeDef](./type_defs.md#projectiontypedef) 
3. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
4. See [:material-code-braces: ProvisionedThroughputDescriptionTypeDef](./type_defs.md#provisionedthroughputdescriptiontypedef) 
## GlobalSecondaryIndexInfoTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import GlobalSecondaryIndexInfoTypeDef

def get_value() -> GlobalSecondaryIndexInfoTypeDef:
    return {
        "IndexName": ...,
    }
```

```python title="Definition"
class GlobalSecondaryIndexInfoTypeDef(TypedDict):
    IndexName: NotRequired[str],
    KeySchema: NotRequired[List[KeySchemaElementTypeDef]],  # (1)
    Projection: NotRequired[ProjectionTypeDef],  # (2)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (3)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionTypeDef](./type_defs.md#projectiontypedef) 
3. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
## GlobalSecondaryIndexTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import GlobalSecondaryIndexTypeDef

def get_value() -> GlobalSecondaryIndexTypeDef:
    return {
        "IndexName": ...,
        "KeySchema": ...,
        "Projection": ...,
    }
```

```python title="Definition"
class GlobalSecondaryIndexTypeDef(TypedDict):
    IndexName: str,
    KeySchema: Sequence[KeySchemaElementTypeDef],  # (1)
    Projection: ProjectionTypeDef,  # (2)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (3)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionTypeDef](./type_defs.md#projectiontypedef) 
3. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
## GlobalSecondaryIndexUpdateTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import GlobalSecondaryIndexUpdateTypeDef

def get_value() -> GlobalSecondaryIndexUpdateTypeDef:
    return {
        "Update": ...,
    }
```

```python title="Definition"
class GlobalSecondaryIndexUpdateTypeDef(TypedDict):
    Update: NotRequired[UpdateGlobalSecondaryIndexActionTypeDef],  # (1)
    Create: NotRequired[CreateGlobalSecondaryIndexActionTypeDef],  # (2)
    Delete: NotRequired[DeleteGlobalSecondaryIndexActionTypeDef],  # (3)
```

1. See [:material-code-braces: UpdateGlobalSecondaryIndexActionTypeDef](./type_defs.md#updateglobalsecondaryindexactiontypedef) 
2. See [:material-code-braces: CreateGlobalSecondaryIndexActionTypeDef](./type_defs.md#createglobalsecondaryindexactiontypedef) 
3. See [:material-code-braces: DeleteGlobalSecondaryIndexActionTypeDef](./type_defs.md#deleteglobalsecondaryindexactiontypedef) 
## GlobalTableDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import GlobalTableDescriptionTypeDef

def get_value() -> GlobalTableDescriptionTypeDef:
    return {
        "ReplicationGroup": ...,
    }
```

```python title="Definition"
class GlobalTableDescriptionTypeDef(TypedDict):
    ReplicationGroup: NotRequired[List[ReplicaDescriptionTypeDef]],  # (1)
    GlobalTableArn: NotRequired[str],
    CreationDateTime: NotRequired[datetime],
    GlobalTableStatus: NotRequired[GlobalTableStatusType],  # (2)
    GlobalTableName: NotRequired[str],
```

1. See [:material-code-braces: ReplicaDescriptionTypeDef](./type_defs.md#replicadescriptiontypedef) 
2. See [:material-code-brackets: GlobalTableStatusType](./literals.md#globaltablestatustype) 
## GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef

def get_value() -> GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef:
    return {
        "IndexName": ...,
    }
```

```python title="Definition"
class GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef(TypedDict):
    IndexName: str,
    ProvisionedWriteCapacityUnits: NotRequired[int],
    ProvisionedWriteCapacityAutoScalingSettingsUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
## GlobalTableTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import GlobalTableTypeDef

def get_value() -> GlobalTableTypeDef:
    return {
        "GlobalTableName": ...,
    }
```

```python title="Definition"
class GlobalTableTypeDef(TypedDict):
    GlobalTableName: NotRequired[str],
    ReplicationGroup: NotRequired[List[ReplicaTypeDef]],  # (1)
```

1. See [:material-code-braces: ReplicaTypeDef](./type_defs.md#replicatypedef) 
## ItemCollectionMetricsTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ItemCollectionMetricsTypeDef

def get_value() -> ItemCollectionMetricsTypeDef:
    return {
        "ItemCollectionKey": ...,
    }
```

```python title="Definition"
class ItemCollectionMetricsTypeDef(TypedDict):
    ItemCollectionKey: NotRequired[Dict[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
    SizeEstimateRangeGB: NotRequired[List[float]],
```

## ItemResponseTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ItemResponseTypeDef

def get_value() -> ItemResponseTypeDef:
    return {
        "Item": ...,
    }
```

```python title="Definition"
class ItemResponseTypeDef(TypedDict):
    Item: NotRequired[Dict[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
```

## KeySchemaElementTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import KeySchemaElementTypeDef

def get_value() -> KeySchemaElementTypeDef:
    return {
        "AttributeName": ...,
        "KeyType": ...,
    }
```

```python title="Definition"
class KeySchemaElementTypeDef(TypedDict):
    AttributeName: str,
    KeyType: KeyTypeType,  # (1)
```

1. See [:material-code-brackets: KeyTypeType](./literals.md#keytypetype) 
## KeysAndAttributesTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import KeysAndAttributesTypeDef

def get_value() -> KeysAndAttributesTypeDef:
    return {
        "Keys": ...,
    }
```

```python title="Definition"
class KeysAndAttributesTypeDef(TypedDict):
    Keys: Sequence[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
    AttributesToGet: NotRequired[Sequence[str]],
    ConsistentRead: NotRequired[bool],
    ProjectionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
```

## KinesisDataStreamDestinationTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import KinesisDataStreamDestinationTypeDef

def get_value() -> KinesisDataStreamDestinationTypeDef:
    return {
        "StreamArn": ...,
    }
```

```python title="Definition"
class KinesisDataStreamDestinationTypeDef(TypedDict):
    StreamArn: NotRequired[str],
    DestinationStatus: NotRequired[DestinationStatusType],  # (1)
    DestinationStatusDescription: NotRequired[str],
```

1. See [:material-code-brackets: DestinationStatusType](./literals.md#destinationstatustype) 
## KinesisStreamingDestinationInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import KinesisStreamingDestinationInputRequestTypeDef

def get_value() -> KinesisStreamingDestinationInputRequestTypeDef:
    return {
        "TableName": ...,
        "StreamArn": ...,
    }
```

```python title="Definition"
class KinesisStreamingDestinationInputRequestTypeDef(TypedDict):
    TableName: str,
    StreamArn: str,
```

## KinesisStreamingDestinationOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import KinesisStreamingDestinationOutputTypeDef

def get_value() -> KinesisStreamingDestinationOutputTypeDef:
    return {
        "TableName": ...,
        "StreamArn": ...,
        "DestinationStatus": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class KinesisStreamingDestinationOutputTypeDef(TypedDict):
    TableName: str,
    StreamArn: str,
    DestinationStatus: DestinationStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: DestinationStatusType](./literals.md#destinationstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListBackupsInputListBackupsPaginateTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ListBackupsInputListBackupsPaginateTypeDef

def get_value() -> ListBackupsInputListBackupsPaginateTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class ListBackupsInputListBackupsPaginateTypeDef(TypedDict):
    TableName: NotRequired[str],
    TimeRangeLowerBound: NotRequired[Union[datetime, str]],
    TimeRangeUpperBound: NotRequired[Union[datetime, str]],
    BackupType: NotRequired[BackupTypeFilterType],  # (1)
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (2)
```

1. See [:material-code-brackets: BackupTypeFilterType](./literals.md#backuptypefiltertype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListBackupsInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ListBackupsInputRequestTypeDef

def get_value() -> ListBackupsInputRequestTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class ListBackupsInputRequestTypeDef(TypedDict):
    TableName: NotRequired[str],
    Limit: NotRequired[int],
    TimeRangeLowerBound: NotRequired[Union[datetime, str]],
    TimeRangeUpperBound: NotRequired[Union[datetime, str]],
    ExclusiveStartBackupArn: NotRequired[str],
    BackupType: NotRequired[BackupTypeFilterType],  # (1)
```

1. See [:material-code-brackets: BackupTypeFilterType](./literals.md#backuptypefiltertype) 
## ListBackupsOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ListBackupsOutputTypeDef

def get_value() -> ListBackupsOutputTypeDef:
    return {
        "BackupSummaries": ...,
        "LastEvaluatedBackupArn": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListBackupsOutputTypeDef(TypedDict):
    BackupSummaries: List[BackupSummaryTypeDef],  # (1)
    LastEvaluatedBackupArn: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: BackupSummaryTypeDef](./type_defs.md#backupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListContributorInsightsInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ListContributorInsightsInputRequestTypeDef

def get_value() -> ListContributorInsightsInputRequestTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class ListContributorInsightsInputRequestTypeDef(TypedDict):
    TableName: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListContributorInsightsOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ListContributorInsightsOutputTypeDef

def get_value() -> ListContributorInsightsOutputTypeDef:
    return {
        "ContributorInsightsSummaries": ...,
        "NextToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListContributorInsightsOutputTypeDef(TypedDict):
    ContributorInsightsSummaries: List[ContributorInsightsSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContributorInsightsSummaryTypeDef](./type_defs.md#contributorinsightssummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListExportsInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ListExportsInputRequestTypeDef

def get_value() -> ListExportsInputRequestTypeDef:
    return {
        "TableArn": ...,
    }
```

```python title="Definition"
class ListExportsInputRequestTypeDef(TypedDict):
    TableArn: NotRequired[str],
    MaxResults: NotRequired[int],
    NextToken: NotRequired[str],
```

## ListExportsOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ListExportsOutputTypeDef

def get_value() -> ListExportsOutputTypeDef:
    return {
        "ExportSummaries": ...,
        "NextToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListExportsOutputTypeDef(TypedDict):
    ExportSummaries: List[ExportSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ExportSummaryTypeDef](./type_defs.md#exportsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListGlobalTablesInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ListGlobalTablesInputRequestTypeDef

def get_value() -> ListGlobalTablesInputRequestTypeDef:
    return {
        "ExclusiveStartGlobalTableName": ...,
    }
```

```python title="Definition"
class ListGlobalTablesInputRequestTypeDef(TypedDict):
    ExclusiveStartGlobalTableName: NotRequired[str],
    Limit: NotRequired[int],
    RegionName: NotRequired[str],
```

## ListGlobalTablesOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ListGlobalTablesOutputTypeDef

def get_value() -> ListGlobalTablesOutputTypeDef:
    return {
        "GlobalTables": ...,
        "LastEvaluatedGlobalTableName": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListGlobalTablesOutputTypeDef(TypedDict):
    GlobalTables: List[GlobalTableTypeDef],  # (1)
    LastEvaluatedGlobalTableName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalTableTypeDef](./type_defs.md#globaltabletypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTablesInputListTablesPaginateTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ListTablesInputListTablesPaginateTypeDef

def get_value() -> ListTablesInputListTablesPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }
```

```python title="Definition"
class ListTablesInputListTablesPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTablesInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ListTablesInputRequestTypeDef

def get_value() -> ListTablesInputRequestTypeDef:
    return {
        "ExclusiveStartTableName": ...,
    }
```

```python title="Definition"
class ListTablesInputRequestTypeDef(TypedDict):
    ExclusiveStartTableName: NotRequired[str],
    Limit: NotRequired[int],
```

## ListTablesOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ListTablesOutputTypeDef

def get_value() -> ListTablesOutputTypeDef:
    return {
        "TableNames": ...,
        "LastEvaluatedTableName": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListTablesOutputTypeDef(TypedDict):
    TableNames: List[str],
    LastEvaluatedTableName: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef

def get_value() -> ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef:
    return {
        "ResourceArn": ...,
    }
```

```python title="Definition"
class ListTagsOfResourceInputListTagsOfResourcePaginateTypeDef(TypedDict):
    ResourceArn: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsOfResourceInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ListTagsOfResourceInputRequestTypeDef

def get_value() -> ListTagsOfResourceInputRequestTypeDef:
    return {
        "ResourceArn": ...,
    }
```

```python title="Definition"
class ListTagsOfResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    NextToken: NotRequired[str],
```

## ListTagsOfResourceOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ListTagsOfResourceOutputTypeDef

def get_value() -> ListTagsOfResourceOutputTypeDef:
    return {
        "Tags": ...,
        "NextToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListTagsOfResourceOutputTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## LocalSecondaryIndexDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import LocalSecondaryIndexDescriptionTypeDef

def get_value() -> LocalSecondaryIndexDescriptionTypeDef:
    return {
        "IndexName": ...,
    }
```

```python title="Definition"
class LocalSecondaryIndexDescriptionTypeDef(TypedDict):
    IndexName: NotRequired[str],
    KeySchema: NotRequired[List[KeySchemaElementTypeDef]],  # (1)
    Projection: NotRequired[ProjectionTypeDef],  # (2)
    IndexSizeBytes: NotRequired[int],
    ItemCount: NotRequired[int],
    IndexArn: NotRequired[str],
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionTypeDef](./type_defs.md#projectiontypedef) 
## LocalSecondaryIndexInfoTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import LocalSecondaryIndexInfoTypeDef

def get_value() -> LocalSecondaryIndexInfoTypeDef:
    return {
        "IndexName": ...,
    }
```

```python title="Definition"
class LocalSecondaryIndexInfoTypeDef(TypedDict):
    IndexName: NotRequired[str],
    KeySchema: NotRequired[List[KeySchemaElementTypeDef]],  # (1)
    Projection: NotRequired[ProjectionTypeDef],  # (2)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionTypeDef](./type_defs.md#projectiontypedef) 
## LocalSecondaryIndexTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import LocalSecondaryIndexTypeDef

def get_value() -> LocalSecondaryIndexTypeDef:
    return {
        "IndexName": ...,
        "KeySchema": ...,
        "Projection": ...,
    }
```

```python title="Definition"
class LocalSecondaryIndexTypeDef(TypedDict):
    IndexName: str,
    KeySchema: Sequence[KeySchemaElementTypeDef],  # (1)
    Projection: ProjectionTypeDef,  # (2)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProjectionTypeDef](./type_defs.md#projectiontypedef) 
## PaginatorConfigTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import PaginatorConfigTypeDef

def get_value() -> PaginatorConfigTypeDef:
    return {
        "MaxItems": ...,
    }
```

```python title="Definition"
class PaginatorConfigTypeDef(TypedDict):
    MaxItems: NotRequired[int],
    PageSize: NotRequired[int],
    StartingToken: NotRequired[str],
```

## ParameterizedStatementTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ParameterizedStatementTypeDef

def get_value() -> ParameterizedStatementTypeDef:
    return {
        "Statement": ...,
    }
```

```python title="Definition"
class ParameterizedStatementTypeDef(TypedDict):
    Statement: str,
    Parameters: NotRequired[Sequence[Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
```

## PointInTimeRecoveryDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import PointInTimeRecoveryDescriptionTypeDef

def get_value() -> PointInTimeRecoveryDescriptionTypeDef:
    return {
        "PointInTimeRecoveryStatus": ...,
    }
```

```python title="Definition"
class PointInTimeRecoveryDescriptionTypeDef(TypedDict):
    PointInTimeRecoveryStatus: NotRequired[PointInTimeRecoveryStatusType],  # (1)
    EarliestRestorableDateTime: NotRequired[datetime],
    LatestRestorableDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: PointInTimeRecoveryStatusType](./literals.md#pointintimerecoverystatustype) 
## PointInTimeRecoverySpecificationTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import PointInTimeRecoverySpecificationTypeDef

def get_value() -> PointInTimeRecoverySpecificationTypeDef:
    return {
        "PointInTimeRecoveryEnabled": ...,
    }
```

```python title="Definition"
class PointInTimeRecoverySpecificationTypeDef(TypedDict):
    PointInTimeRecoveryEnabled: bool,
```

## ProjectionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ProjectionTypeDef

def get_value() -> ProjectionTypeDef:
    return {
        "ProjectionType": ...,
    }
```

```python title="Definition"
class ProjectionTypeDef(TypedDict):
    ProjectionType: NotRequired[ProjectionTypeType],  # (1)
    NonKeyAttributes: NotRequired[Sequence[str]],
```

1. See [:material-code-brackets: ProjectionTypeType](./literals.md#projectiontypetype) 
## ProvisionedThroughputDescriptionResponseMetadataTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ProvisionedThroughputDescriptionResponseMetadataTypeDef

def get_value() -> ProvisionedThroughputDescriptionResponseMetadataTypeDef:
    return {
        "LastIncreaseDateTime": ...,
        "LastDecreaseDateTime": ...,
        "NumberOfDecreasesToday": ...,
        "ReadCapacityUnits": ...,
        "WriteCapacityUnits": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ProvisionedThroughputDescriptionResponseMetadataTypeDef(TypedDict):
    LastIncreaseDateTime: datetime,
    LastDecreaseDateTime: datetime,
    NumberOfDecreasesToday: int,
    ReadCapacityUnits: int,
    WriteCapacityUnits: int,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ProvisionedThroughputDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ProvisionedThroughputDescriptionTypeDef

def get_value() -> ProvisionedThroughputDescriptionTypeDef:
    return {
        "LastIncreaseDateTime": ...,
    }
```

```python title="Definition"
class ProvisionedThroughputDescriptionTypeDef(TypedDict):
    LastIncreaseDateTime: NotRequired[datetime],
    LastDecreaseDateTime: NotRequired[datetime],
    NumberOfDecreasesToday: NotRequired[int],
    ReadCapacityUnits: NotRequired[int],
    WriteCapacityUnits: NotRequired[int],
```

## ProvisionedThroughputOverrideTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ProvisionedThroughputOverrideTypeDef

def get_value() -> ProvisionedThroughputOverrideTypeDef:
    return {
        "ReadCapacityUnits": ...,
    }
```

```python title="Definition"
class ProvisionedThroughputOverrideTypeDef(TypedDict):
    ReadCapacityUnits: NotRequired[int],
```

## ProvisionedThroughputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ProvisionedThroughputTypeDef

def get_value() -> ProvisionedThroughputTypeDef:
    return {
        "ReadCapacityUnits": ...,
        "WriteCapacityUnits": ...,
    }
```

```python title="Definition"
class ProvisionedThroughputTypeDef(TypedDict):
    ReadCapacityUnits: int,
    WriteCapacityUnits: int,
```

## PutItemInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import PutItemInputRequestTypeDef

def get_value() -> PutItemInputRequestTypeDef:
    return {
        "TableName": ...,
        "Item": ...,
    }
```

```python title="Definition"
class PutItemInputRequestTypeDef(TypedDict):
    TableName: str,
    Item: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    Expected: NotRequired[Mapping[str, ExpectedAttributeValueTypeDef]],  # (1)
    ReturnValues: NotRequired[ReturnValueType],  # (2)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (3)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (4)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (5)
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
```

1. See [:material-code-braces: ExpectedAttributeValueTypeDef](./type_defs.md#expectedattributevaluetypedef) 
2. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
3. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
4. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
5. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
## PutItemInputTablePutItemTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import PutItemInputTablePutItemTypeDef

def get_value() -> PutItemInputTablePutItemTypeDef:
    return {
        "Item": ...,
    }
```

```python title="Definition"
class PutItemInputTablePutItemTypeDef(TypedDict):
    Item: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    Expected: NotRequired[Mapping[str, ExpectedAttributeValueTypeDef]],  # (1)
    ReturnValues: NotRequired[ReturnValueType],  # (2)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (3)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (4)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (5)
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
```

1. See [:material-code-braces: ExpectedAttributeValueTypeDef](./type_defs.md#expectedattributevaluetypedef) 
2. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
3. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
4. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
5. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
## PutItemOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import PutItemOutputTypeDef

def get_value() -> PutItemOutputTypeDef:
    return {
        "Attributes": ...,
        "ConsumedCapacity": ...,
        "ItemCollectionMetrics": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class PutItemOutputTypeDef(TypedDict):
    Attributes: Dict[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (1)
    ItemCollectionMetrics: ItemCollectionMetricsTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ItemCollectionMetricsTypeDef](./type_defs.md#itemcollectionmetricstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## PutRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import PutRequestTypeDef

def get_value() -> PutRequestTypeDef:
    return {
        "Item": ...,
    }
```

```python title="Definition"
class PutRequestTypeDef(TypedDict):
    Item: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
```

## PutTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import PutTypeDef

def get_value() -> PutTypeDef:
    return {
        "Item": ...,
        "TableName": ...,
    }
```

```python title="Definition"
class PutTypeDef(TypedDict):
    Item: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    TableName: str,
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (1)
```

1. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## QueryInputQueryPaginateTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import QueryInputQueryPaginateTypeDef

def get_value() -> QueryInputQueryPaginateTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class QueryInputQueryPaginateTypeDef(TypedDict):
    TableName: str,
    IndexName: NotRequired[str],
    Select: NotRequired[SelectType],  # (1)
    AttributesToGet: NotRequired[Sequence[str]],
    ConsistentRead: NotRequired[bool],
    KeyConditions: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    QueryFilter: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (4)
    ScanIndexForward: NotRequired[bool],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (5)
    ProjectionExpression: NotRequired[str],
    FilterExpression: NotRequired[str],
    KeyConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (6)
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
3. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
4. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
6. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## QueryInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import QueryInputRequestTypeDef

def get_value() -> QueryInputRequestTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class QueryInputRequestTypeDef(TypedDict):
    TableName: str,
    IndexName: NotRequired[str],
    Select: NotRequired[SelectType],  # (1)
    AttributesToGet: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    ConsistentRead: NotRequired[bool],
    KeyConditions: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    QueryFilter: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (4)
    ScanIndexForward: NotRequired[bool],
    ExclusiveStartKey: NotRequired[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (5)
    ProjectionExpression: NotRequired[str],
    FilterExpression: NotRequired[str],
    KeyConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
3. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
4. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## QueryInputTableQueryTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import QueryInputTableQueryTypeDef

def get_value() -> QueryInputTableQueryTypeDef:
    return {
        "IndexName": ...,
    }
```

```python title="Definition"
class QueryInputTableQueryTypeDef(TypedDict):
    IndexName: NotRequired[str],
    Select: NotRequired[SelectType],  # (1)
    AttributesToGet: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    ConsistentRead: NotRequired[bool],
    KeyConditions: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    QueryFilter: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (4)
    ScanIndexForward: NotRequired[bool],
    ExclusiveStartKey: NotRequired[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (5)
    ProjectionExpression: NotRequired[str],
    FilterExpression: NotRequired[Union[str, ConditionBase]],
    KeyConditionExpression: NotRequired[Union[str, ConditionBase]],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
3. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
4. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## QueryOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import QueryOutputTypeDef

def get_value() -> QueryOutputTypeDef:
    return {
        "Items": ...,
        "Count": ...,
        "ScannedCount": ...,
        "LastEvaluatedKey": ...,
        "ConsumedCapacity": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class QueryOutputTypeDef(TypedDict):
    Items: List[Dict[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
    Count: int,
    ScannedCount: int,
    LastEvaluatedKey: Dict[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ReplicaAutoScalingDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ReplicaAutoScalingDescriptionTypeDef

def get_value() -> ReplicaAutoScalingDescriptionTypeDef:
    return {
        "RegionName": ...,
    }
```

```python title="Definition"
class ReplicaAutoScalingDescriptionTypeDef(TypedDict):
    RegionName: NotRequired[str],
    GlobalSecondaryIndexes: NotRequired[List[ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef]],  # (1)
    ReplicaProvisionedReadCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (2)
    ReplicaProvisionedWriteCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (2)
    ReplicaStatus: NotRequired[ReplicaStatusType],  # (4)
```

1. See [:material-code-braces: ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef](./type_defs.md#replicaglobalsecondaryindexautoscalingdescriptiontypedef) 
2. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
3. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
4. See [:material-code-brackets: ReplicaStatusType](./literals.md#replicastatustype) 
## ReplicaAutoScalingUpdateTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ReplicaAutoScalingUpdateTypeDef

def get_value() -> ReplicaAutoScalingUpdateTypeDef:
    return {
        "RegionName": ...,
    }
```

```python title="Definition"
class ReplicaAutoScalingUpdateTypeDef(TypedDict):
    RegionName: str,
    ReplicaGlobalSecondaryIndexUpdates: NotRequired[Sequence[ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef]],  # (1)
    ReplicaProvisionedReadCapacityAutoScalingUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (2)
```

1. See [:material-code-braces: ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef](./type_defs.md#replicaglobalsecondaryindexautoscalingupdatetypedef) 
2. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
## ReplicaDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ReplicaDescriptionTypeDef

def get_value() -> ReplicaDescriptionTypeDef:
    return {
        "RegionName": ...,
    }
```

```python title="Definition"
class ReplicaDescriptionTypeDef(TypedDict):
    RegionName: NotRequired[str],
    ReplicaStatus: NotRequired[ReplicaStatusType],  # (1)
    ReplicaStatusDescription: NotRequired[str],
    ReplicaStatusPercentProgress: NotRequired[str],
    KMSMasterKeyId: NotRequired[str],
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputOverrideTypeDef],  # (2)
    GlobalSecondaryIndexes: NotRequired[List[ReplicaGlobalSecondaryIndexDescriptionTypeDef]],  # (3)
    ReplicaInaccessibleDateTime: NotRequired[datetime],
    ReplicaTableClassSummary: NotRequired[TableClassSummaryTypeDef],  # (4)
```

1. See [:material-code-brackets: ReplicaStatusType](./literals.md#replicastatustype) 
2. See [:material-code-braces: ProvisionedThroughputOverrideTypeDef](./type_defs.md#provisionedthroughputoverridetypedef) 
3. See [:material-code-braces: ReplicaGlobalSecondaryIndexDescriptionTypeDef](./type_defs.md#replicaglobalsecondaryindexdescriptiontypedef) 
4. See [:material-code-braces: TableClassSummaryTypeDef](./type_defs.md#tableclasssummarytypedef) 
## ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef

def get_value() -> ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef:
    return {
        "IndexName": ...,
    }
```

```python title="Definition"
class ReplicaGlobalSecondaryIndexAutoScalingDescriptionTypeDef(TypedDict):
    IndexName: NotRequired[str],
    IndexStatus: NotRequired[IndexStatusType],  # (1)
    ProvisionedReadCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (2)
    ProvisionedWriteCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (2)
```

1. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
2. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
3. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
## ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef

def get_value() -> ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef:
    return {
        "IndexName": ...,
    }
```

```python title="Definition"
class ReplicaGlobalSecondaryIndexAutoScalingUpdateTypeDef(TypedDict):
    IndexName: NotRequired[str],
    ProvisionedReadCapacityAutoScalingUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
## ReplicaGlobalSecondaryIndexDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ReplicaGlobalSecondaryIndexDescriptionTypeDef

def get_value() -> ReplicaGlobalSecondaryIndexDescriptionTypeDef:
    return {
        "IndexName": ...,
    }
```

```python title="Definition"
class ReplicaGlobalSecondaryIndexDescriptionTypeDef(TypedDict):
    IndexName: NotRequired[str],
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputOverrideTypeDef],  # (1)
```

1. See [:material-code-braces: ProvisionedThroughputOverrideTypeDef](./type_defs.md#provisionedthroughputoverridetypedef) 
## ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef

def get_value() -> ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef:
    return {
        "IndexName": ...,
    }
```

```python title="Definition"
class ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef(TypedDict):
    IndexName: str,
    IndexStatus: NotRequired[IndexStatusType],  # (1)
    ProvisionedReadCapacityUnits: NotRequired[int],
    ProvisionedReadCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (2)
    ProvisionedWriteCapacityUnits: NotRequired[int],
    ProvisionedWriteCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (2)
```

1. See [:material-code-brackets: IndexStatusType](./literals.md#indexstatustype) 
2. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
3. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
## ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef

def get_value() -> ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef:
    return {
        "IndexName": ...,
    }
```

```python title="Definition"
class ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef(TypedDict):
    IndexName: str,
    ProvisionedReadCapacityUnits: NotRequired[int],
    ProvisionedReadCapacityAutoScalingSettingsUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
## ReplicaGlobalSecondaryIndexTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ReplicaGlobalSecondaryIndexTypeDef

def get_value() -> ReplicaGlobalSecondaryIndexTypeDef:
    return {
        "IndexName": ...,
    }
```

```python title="Definition"
class ReplicaGlobalSecondaryIndexTypeDef(TypedDict):
    IndexName: str,
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputOverrideTypeDef],  # (1)
```

1. See [:material-code-braces: ProvisionedThroughputOverrideTypeDef](./type_defs.md#provisionedthroughputoverridetypedef) 
## ReplicaSettingsDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ReplicaSettingsDescriptionTypeDef

def get_value() -> ReplicaSettingsDescriptionTypeDef:
    return {
        "RegionName": ...,
    }
```

```python title="Definition"
class ReplicaSettingsDescriptionTypeDef(TypedDict):
    RegionName: str,
    ReplicaStatus: NotRequired[ReplicaStatusType],  # (1)
    ReplicaBillingModeSummary: NotRequired[BillingModeSummaryTypeDef],  # (2)
    ReplicaProvisionedReadCapacityUnits: NotRequired[int],
    ReplicaProvisionedReadCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (3)
    ReplicaProvisionedWriteCapacityUnits: NotRequired[int],
    ReplicaProvisionedWriteCapacityAutoScalingSettings: NotRequired[AutoScalingSettingsDescriptionTypeDef],  # (3)
    ReplicaGlobalSecondaryIndexSettings: NotRequired[List[ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef]],  # (5)
    ReplicaTableClassSummary: NotRequired[TableClassSummaryTypeDef],  # (6)
```

1. See [:material-code-brackets: ReplicaStatusType](./literals.md#replicastatustype) 
2. See [:material-code-braces: BillingModeSummaryTypeDef](./type_defs.md#billingmodesummarytypedef) 
3. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
4. See [:material-code-braces: AutoScalingSettingsDescriptionTypeDef](./type_defs.md#autoscalingsettingsdescriptiontypedef) 
5. See [:material-code-braces: ReplicaGlobalSecondaryIndexSettingsDescriptionTypeDef](./type_defs.md#replicaglobalsecondaryindexsettingsdescriptiontypedef) 
6. See [:material-code-braces: TableClassSummaryTypeDef](./type_defs.md#tableclasssummarytypedef) 
## ReplicaSettingsUpdateTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ReplicaSettingsUpdateTypeDef

def get_value() -> ReplicaSettingsUpdateTypeDef:
    return {
        "RegionName": ...,
    }
```

```python title="Definition"
class ReplicaSettingsUpdateTypeDef(TypedDict):
    RegionName: str,
    ReplicaProvisionedReadCapacityUnits: NotRequired[int],
    ReplicaProvisionedReadCapacityAutoScalingSettingsUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (1)
    ReplicaGlobalSecondaryIndexSettingsUpdate: NotRequired[Sequence[ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef]],  # (2)
    ReplicaTableClass: NotRequired[TableClassType],  # (3)
```

1. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
2. See [:material-code-braces: ReplicaGlobalSecondaryIndexSettingsUpdateTypeDef](./type_defs.md#replicaglobalsecondaryindexsettingsupdatetypedef) 
3. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
## ReplicaTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ReplicaTypeDef

def get_value() -> ReplicaTypeDef:
    return {
        "RegionName": ...,
    }
```

```python title="Definition"
class ReplicaTypeDef(TypedDict):
    RegionName: NotRequired[str],
```

## ReplicaUpdateTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ReplicaUpdateTypeDef

def get_value() -> ReplicaUpdateTypeDef:
    return {
        "Create": ...,
    }
```

```python title="Definition"
class ReplicaUpdateTypeDef(TypedDict):
    Create: NotRequired[CreateReplicaActionTypeDef],  # (1)
    Delete: NotRequired[DeleteReplicaActionTypeDef],  # (2)
```

1. See [:material-code-braces: CreateReplicaActionTypeDef](./type_defs.md#createreplicaactiontypedef) 
2. See [:material-code-braces: DeleteReplicaActionTypeDef](./type_defs.md#deletereplicaactiontypedef) 
## ReplicationGroupUpdateTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ReplicationGroupUpdateTypeDef

def get_value() -> ReplicationGroupUpdateTypeDef:
    return {
        "Create": ...,
    }
```

```python title="Definition"
class ReplicationGroupUpdateTypeDef(TypedDict):
    Create: NotRequired[CreateReplicationGroupMemberActionTypeDef],  # (1)
    Update: NotRequired[UpdateReplicationGroupMemberActionTypeDef],  # (2)
    Delete: NotRequired[DeleteReplicationGroupMemberActionTypeDef],  # (3)
```

1. See [:material-code-braces: CreateReplicationGroupMemberActionTypeDef](./type_defs.md#createreplicationgroupmemberactiontypedef) 
2. See [:material-code-braces: UpdateReplicationGroupMemberActionTypeDef](./type_defs.md#updatereplicationgroupmemberactiontypedef) 
3. See [:material-code-braces: DeleteReplicationGroupMemberActionTypeDef](./type_defs.md#deletereplicationgroupmemberactiontypedef) 
## ResponseMetadataTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ResponseMetadataTypeDef

def get_value() -> ResponseMetadataTypeDef:
    return {
        "RequestId": ...,
        "HostId": ...,
        "HTTPStatusCode": ...,
        "HTTPHeaders": ...,
        "RetryAttempts": ...,
    }
```

```python title="Definition"
class ResponseMetadataTypeDef(TypedDict):
    RequestId: str,
    HostId: str,
    HTTPStatusCode: int,
    HTTPHeaders: Dict[str, str],
    RetryAttempts: int,
```

## RestoreSummaryResponseMetadataTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import RestoreSummaryResponseMetadataTypeDef

def get_value() -> RestoreSummaryResponseMetadataTypeDef:
    return {
        "SourceBackupArn": ...,
        "SourceTableArn": ...,
        "RestoreDateTime": ...,
        "RestoreInProgress": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class RestoreSummaryResponseMetadataTypeDef(TypedDict):
    SourceBackupArn: str,
    SourceTableArn: str,
    RestoreDateTime: datetime,
    RestoreInProgress: bool,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreSummaryTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import RestoreSummaryTypeDef

def get_value() -> RestoreSummaryTypeDef:
    return {
        "RestoreDateTime": ...,
        "RestoreInProgress": ...,
    }
```

```python title="Definition"
class RestoreSummaryTypeDef(TypedDict):
    RestoreDateTime: datetime,
    RestoreInProgress: bool,
    SourceBackupArn: NotRequired[str],
    SourceTableArn: NotRequired[str],
```

## RestoreTableFromBackupInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import RestoreTableFromBackupInputRequestTypeDef

def get_value() -> RestoreTableFromBackupInputRequestTypeDef:
    return {
        "TargetTableName": ...,
        "BackupArn": ...,
    }
```

```python title="Definition"
class RestoreTableFromBackupInputRequestTypeDef(TypedDict):
    TargetTableName: str,
    BackupArn: str,
    BillingModeOverride: NotRequired[BillingModeType],  # (1)
    GlobalSecondaryIndexOverride: NotRequired[Sequence[GlobalSecondaryIndexTypeDef]],  # (2)
    LocalSecondaryIndexOverride: NotRequired[Sequence[LocalSecondaryIndexTypeDef]],  # (3)
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputTypeDef],  # (4)
    SSESpecificationOverride: NotRequired[SSESpecificationTypeDef],  # (5)
```

1. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
2. See [:material-code-braces: GlobalSecondaryIndexTypeDef](./type_defs.md#globalsecondaryindextypedef) 
3. See [:material-code-braces: LocalSecondaryIndexTypeDef](./type_defs.md#localsecondaryindextypedef) 
4. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
5. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
## RestoreTableFromBackupOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import RestoreTableFromBackupOutputTypeDef

def get_value() -> RestoreTableFromBackupOutputTypeDef:
    return {
        "TableDescription": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class RestoreTableFromBackupOutputTypeDef(TypedDict):
    TableDescription: TableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableDescriptionTypeDef](./type_defs.md#tabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## RestoreTableToPointInTimeInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import RestoreTableToPointInTimeInputRequestTypeDef

def get_value() -> RestoreTableToPointInTimeInputRequestTypeDef:
    return {
        "TargetTableName": ...,
    }
```

```python title="Definition"
class RestoreTableToPointInTimeInputRequestTypeDef(TypedDict):
    TargetTableName: str,
    SourceTableArn: NotRequired[str],
    SourceTableName: NotRequired[str],
    UseLatestRestorableTime: NotRequired[bool],
    RestoreDateTime: NotRequired[Union[datetime, str]],
    BillingModeOverride: NotRequired[BillingModeType],  # (1)
    GlobalSecondaryIndexOverride: NotRequired[Sequence[GlobalSecondaryIndexTypeDef]],  # (2)
    LocalSecondaryIndexOverride: NotRequired[Sequence[LocalSecondaryIndexTypeDef]],  # (3)
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputTypeDef],  # (4)
    SSESpecificationOverride: NotRequired[SSESpecificationTypeDef],  # (5)
```

1. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
2. See [:material-code-braces: GlobalSecondaryIndexTypeDef](./type_defs.md#globalsecondaryindextypedef) 
3. See [:material-code-braces: LocalSecondaryIndexTypeDef](./type_defs.md#localsecondaryindextypedef) 
4. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
5. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
## RestoreTableToPointInTimeOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import RestoreTableToPointInTimeOutputTypeDef

def get_value() -> RestoreTableToPointInTimeOutputTypeDef:
    return {
        "TableDescription": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class RestoreTableToPointInTimeOutputTypeDef(TypedDict):
    TableDescription: TableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableDescriptionTypeDef](./type_defs.md#tabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SSEDescriptionResponseMetadataTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import SSEDescriptionResponseMetadataTypeDef

def get_value() -> SSEDescriptionResponseMetadataTypeDef:
    return {
        "Status": ...,
        "SSEType": ...,
        "KMSMasterKeyArn": ...,
        "InaccessibleEncryptionDateTime": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class SSEDescriptionResponseMetadataTypeDef(TypedDict):
    Status: SSEStatusType,  # (1)
    SSEType: SSETypeType,  # (2)
    KMSMasterKeyArn: str,
    InaccessibleEncryptionDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-brackets: SSEStatusType](./literals.md#ssestatustype) 
2. See [:material-code-brackets: SSETypeType](./literals.md#ssetypetype) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## SSEDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import SSEDescriptionTypeDef

def get_value() -> SSEDescriptionTypeDef:
    return {
        "Status": ...,
    }
```

```python title="Definition"
class SSEDescriptionTypeDef(TypedDict):
    Status: NotRequired[SSEStatusType],  # (1)
    SSEType: NotRequired[SSETypeType],  # (2)
    KMSMasterKeyArn: NotRequired[str],
    InaccessibleEncryptionDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: SSEStatusType](./literals.md#ssestatustype) 
2. See [:material-code-brackets: SSETypeType](./literals.md#ssetypetype) 
## SSESpecificationTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import SSESpecificationTypeDef

def get_value() -> SSESpecificationTypeDef:
    return {
        "Enabled": ...,
    }
```

```python title="Definition"
class SSESpecificationTypeDef(TypedDict):
    Enabled: NotRequired[bool],
    SSEType: NotRequired[SSETypeType],  # (1)
    KMSMasterKeyId: NotRequired[str],
```

1. See [:material-code-brackets: SSETypeType](./literals.md#ssetypetype) 
## ScanInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ScanInputRequestTypeDef

def get_value() -> ScanInputRequestTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class ScanInputRequestTypeDef(TypedDict):
    TableName: str,
    IndexName: NotRequired[str],
    AttributesToGet: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    Select: NotRequired[SelectType],  # (1)
    ScanFilter: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (3)
    ExclusiveStartKey: NotRequired[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (4)
    TotalSegments: NotRequired[int],
    Segment: NotRequired[int],
    ProjectionExpression: NotRequired[str],
    FilterExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
    ConsistentRead: NotRequired[bool],
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## ScanInputScanPaginateTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ScanInputScanPaginateTypeDef

def get_value() -> ScanInputScanPaginateTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class ScanInputScanPaginateTypeDef(TypedDict):
    TableName: str,
    IndexName: NotRequired[str],
    AttributesToGet: NotRequired[Sequence[str]],
    Select: NotRequired[SelectType],  # (1)
    ScanFilter: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (3)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (4)
    TotalSegments: NotRequired[int],
    Segment: NotRequired[int],
    ProjectionExpression: NotRequired[str],
    FilterExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
    ConsistentRead: NotRequired[bool],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (5)
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
5. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ScanInputTableScanTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ScanInputTableScanTypeDef

def get_value() -> ScanInputTableScanTypeDef:
    return {
        "IndexName": ...,
    }
```

```python title="Definition"
class ScanInputTableScanTypeDef(TypedDict):
    IndexName: NotRequired[str],
    AttributesToGet: NotRequired[Sequence[str]],
    Limit: NotRequired[int],
    Select: NotRequired[SelectType],  # (1)
    ScanFilter: NotRequired[Mapping[str, ConditionTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (3)
    ExclusiveStartKey: NotRequired[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (4)
    TotalSegments: NotRequired[int],
    Segment: NotRequired[int],
    ProjectionExpression: NotRequired[str],
    FilterExpression: NotRequired[Union[str, ConditionBase]],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
    ConsistentRead: NotRequired[bool],
```

1. See [:material-code-brackets: SelectType](./literals.md#selecttype) 
2. See [:material-code-braces: ConditionTypeDef](./type_defs.md#conditiontypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## ScanOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ScanOutputTypeDef

def get_value() -> ScanOutputTypeDef:
    return {
        "Items": ...,
        "Count": ...,
        "ScannedCount": ...,
        "LastEvaluatedKey": ...,
        "ConsumedCapacity": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ScanOutputTypeDef(TypedDict):
    Items: List[Dict[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
    Count: int,
    ScannedCount: int,
    LastEvaluatedKey: Dict[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ServiceResourceTableRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import ServiceResourceTableRequestTypeDef

def get_value() -> ServiceResourceTableRequestTypeDef:
    return {
        "name": ...,
    }
```

```python title="Definition"
class ServiceResourceTableRequestTypeDef(TypedDict):
    name: str,
```

## SourceTableDetailsTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import SourceTableDetailsTypeDef

def get_value() -> SourceTableDetailsTypeDef:
    return {
        "TableName": ...,
        "TableId": ...,
        "KeySchema": ...,
        "TableCreationDateTime": ...,
        "ProvisionedThroughput": ...,
    }
```

```python title="Definition"
class SourceTableDetailsTypeDef(TypedDict):
    TableName: str,
    TableId: str,
    KeySchema: List[KeySchemaElementTypeDef],  # (1)
    TableCreationDateTime: datetime,
    ProvisionedThroughput: ProvisionedThroughputTypeDef,  # (2)
    TableArn: NotRequired[str],
    TableSizeBytes: NotRequired[int],
    ItemCount: NotRequired[int],
    BillingMode: NotRequired[BillingModeType],  # (3)
```

1. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
2. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
3. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
## SourceTableFeatureDetailsTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import SourceTableFeatureDetailsTypeDef

def get_value() -> SourceTableFeatureDetailsTypeDef:
    return {
        "LocalSecondaryIndexes": ...,
    }
```

```python title="Definition"
class SourceTableFeatureDetailsTypeDef(TypedDict):
    LocalSecondaryIndexes: NotRequired[List[LocalSecondaryIndexInfoTypeDef]],  # (1)
    GlobalSecondaryIndexes: NotRequired[List[GlobalSecondaryIndexInfoTypeDef]],  # (2)
    StreamDescription: NotRequired[StreamSpecificationTypeDef],  # (3)
    TimeToLiveDescription: NotRequired[TimeToLiveDescriptionTypeDef],  # (4)
    SSEDescription: NotRequired[SSEDescriptionTypeDef],  # (5)
```

1. See [:material-code-braces: LocalSecondaryIndexInfoTypeDef](./type_defs.md#localsecondaryindexinfotypedef) 
2. See [:material-code-braces: GlobalSecondaryIndexInfoTypeDef](./type_defs.md#globalsecondaryindexinfotypedef) 
3. See [:material-code-braces: StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef) 
4. See [:material-code-braces: TimeToLiveDescriptionTypeDef](./type_defs.md#timetolivedescriptiontypedef) 
5. See [:material-code-braces: SSEDescriptionTypeDef](./type_defs.md#ssedescriptiontypedef) 
## StreamSpecificationResponseMetadataTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import StreamSpecificationResponseMetadataTypeDef

def get_value() -> StreamSpecificationResponseMetadataTypeDef:
    return {
        "StreamEnabled": ...,
        "StreamViewType": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class StreamSpecificationResponseMetadataTypeDef(TypedDict):
    StreamEnabled: bool,
    StreamViewType: StreamViewTypeType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: StreamViewTypeType](./literals.md#streamviewtypetype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StreamSpecificationTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import StreamSpecificationTypeDef

def get_value() -> StreamSpecificationTypeDef:
    return {
        "StreamEnabled": ...,
    }
```

```python title="Definition"
class StreamSpecificationTypeDef(TypedDict):
    StreamEnabled: bool,
    StreamViewType: NotRequired[StreamViewTypeType],  # (1)
```

1. See [:material-code-brackets: StreamViewTypeType](./literals.md#streamviewtypetype) 
## TableAutoScalingDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import TableAutoScalingDescriptionTypeDef

def get_value() -> TableAutoScalingDescriptionTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class TableAutoScalingDescriptionTypeDef(TypedDict):
    TableName: NotRequired[str],
    TableStatus: NotRequired[TableStatusType],  # (1)
    Replicas: NotRequired[List[ReplicaAutoScalingDescriptionTypeDef]],  # (2)
```

1. See [:material-code-brackets: TableStatusType](./literals.md#tablestatustype) 
2. See [:material-code-braces: ReplicaAutoScalingDescriptionTypeDef](./type_defs.md#replicaautoscalingdescriptiontypedef) 
## TableBatchWriterRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import TableBatchWriterRequestTypeDef

def get_value() -> TableBatchWriterRequestTypeDef:
    return {
        "overwrite_by_pkeys": ...,
    }
```

```python title="Definition"
class TableBatchWriterRequestTypeDef(TypedDict):
    overwrite_by_pkeys: NotRequired[List[str]],
```

## TableClassSummaryResponseMetadataTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import TableClassSummaryResponseMetadataTypeDef

def get_value() -> TableClassSummaryResponseMetadataTypeDef:
    return {
        "TableClass": ...,
        "LastUpdateDateTime": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class TableClassSummaryResponseMetadataTypeDef(TypedDict):
    TableClass: TableClassType,  # (1)
    LastUpdateDateTime: datetime,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TableClassSummaryTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import TableClassSummaryTypeDef

def get_value() -> TableClassSummaryTypeDef:
    return {
        "TableClass": ...,
    }
```

```python title="Definition"
class TableClassSummaryTypeDef(TypedDict):
    TableClass: NotRequired[TableClassType],  # (1)
    LastUpdateDateTime: NotRequired[datetime],
```

1. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
## TableDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import TableDescriptionTypeDef

def get_value() -> TableDescriptionTypeDef:
    return {
        "AttributeDefinitions": ...,
    }
```

```python title="Definition"
class TableDescriptionTypeDef(TypedDict):
    AttributeDefinitions: NotRequired[List[AttributeDefinitionTypeDef]],  # (1)
    TableName: NotRequired[str],
    KeySchema: NotRequired[List[KeySchemaElementTypeDef]],  # (2)
    TableStatus: NotRequired[TableStatusType],  # (3)
    CreationDateTime: NotRequired[datetime],
    ProvisionedThroughput: NotRequired[ProvisionedThroughputDescriptionTypeDef],  # (4)
    TableSizeBytes: NotRequired[int],
    ItemCount: NotRequired[int],
    TableArn: NotRequired[str],
    TableId: NotRequired[str],
    BillingModeSummary: NotRequired[BillingModeSummaryTypeDef],  # (5)
    LocalSecondaryIndexes: NotRequired[List[LocalSecondaryIndexDescriptionTypeDef]],  # (6)
    GlobalSecondaryIndexes: NotRequired[List[GlobalSecondaryIndexDescriptionTypeDef]],  # (7)
    StreamSpecification: NotRequired[StreamSpecificationTypeDef],  # (8)
    LatestStreamLabel: NotRequired[str],
    LatestStreamArn: NotRequired[str],
    GlobalTableVersion: NotRequired[str],
    Replicas: NotRequired[List[ReplicaDescriptionTypeDef]],  # (9)
    RestoreSummary: NotRequired[RestoreSummaryTypeDef],  # (10)
    SSEDescription: NotRequired[SSEDescriptionTypeDef],  # (11)
    ArchivalSummary: NotRequired[ArchivalSummaryTypeDef],  # (12)
    TableClassSummary: NotRequired[TableClassSummaryTypeDef],  # (13)
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-braces: KeySchemaElementTypeDef](./type_defs.md#keyschemaelementtypedef) 
3. See [:material-code-brackets: TableStatusType](./literals.md#tablestatustype) 
4. See [:material-code-braces: ProvisionedThroughputDescriptionTypeDef](./type_defs.md#provisionedthroughputdescriptiontypedef) 
5. See [:material-code-braces: BillingModeSummaryTypeDef](./type_defs.md#billingmodesummarytypedef) 
6. See [:material-code-braces: LocalSecondaryIndexDescriptionTypeDef](./type_defs.md#localsecondaryindexdescriptiontypedef) 
7. See [:material-code-braces: GlobalSecondaryIndexDescriptionTypeDef](./type_defs.md#globalsecondaryindexdescriptiontypedef) 
8. See [:material-code-braces: StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef) 
9. See [:material-code-braces: ReplicaDescriptionTypeDef](./type_defs.md#replicadescriptiontypedef) 
10. See [:material-code-braces: RestoreSummaryTypeDef](./type_defs.md#restoresummarytypedef) 
11. See [:material-code-braces: SSEDescriptionTypeDef](./type_defs.md#ssedescriptiontypedef) 
12. See [:material-code-braces: ArchivalSummaryTypeDef](./type_defs.md#archivalsummarytypedef) 
13. See [:material-code-braces: TableClassSummaryTypeDef](./type_defs.md#tableclasssummarytypedef) 
## TagResourceInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import TagResourceInputRequestTypeDef

def get_value() -> TagResourceInputRequestTypeDef:
    return {
        "ResourceArn": ...,
        "Tags": ...,
    }
```

```python title="Definition"
class TagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import TagTypeDef

def get_value() -> TagTypeDef:
    return {
        "Key": ...,
        "Value": ...,
    }
```

```python title="Definition"
class TagTypeDef(TypedDict):
    Key: str,
    Value: str,
```

## TimeToLiveDescriptionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import TimeToLiveDescriptionTypeDef

def get_value() -> TimeToLiveDescriptionTypeDef:
    return {
        "TimeToLiveStatus": ...,
    }
```

```python title="Definition"
class TimeToLiveDescriptionTypeDef(TypedDict):
    TimeToLiveStatus: NotRequired[TimeToLiveStatusType],  # (1)
    AttributeName: NotRequired[str],
```

1. See [:material-code-brackets: TimeToLiveStatusType](./literals.md#timetolivestatustype) 
## TimeToLiveSpecificationTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import TimeToLiveSpecificationTypeDef

def get_value() -> TimeToLiveSpecificationTypeDef:
    return {
        "Enabled": ...,
        "AttributeName": ...,
    }
```

```python title="Definition"
class TimeToLiveSpecificationTypeDef(TypedDict):
    Enabled: bool,
    AttributeName: str,
```

## TransactGetItemTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import TransactGetItemTypeDef

def get_value() -> TransactGetItemTypeDef:
    return {
        "Get": ...,
    }
```

```python title="Definition"
class TransactGetItemTypeDef(TypedDict):
    Get: GetTypeDef,  # (1)
```

1. See [:material-code-braces: GetTypeDef](./type_defs.md#gettypedef) 
## TransactGetItemsInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import TransactGetItemsInputRequestTypeDef

def get_value() -> TransactGetItemsInputRequestTypeDef:
    return {
        "TransactItems": ...,
    }
```

```python title="Definition"
class TransactGetItemsInputRequestTypeDef(TypedDict):
    TransactItems: Sequence[TransactGetItemTypeDef],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
```

1. See [:material-code-braces: TransactGetItemTypeDef](./type_defs.md#transactgetitemtypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
## TransactGetItemsOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import TransactGetItemsOutputTypeDef

def get_value() -> TransactGetItemsOutputTypeDef:
    return {
        "ConsumedCapacity": ...,
        "Responses": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class TransactGetItemsOutputTypeDef(TypedDict):
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (1)
    Responses: List[ItemResponseTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ItemResponseTypeDef](./type_defs.md#itemresponsetypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## TransactWriteItemTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import TransactWriteItemTypeDef

def get_value() -> TransactWriteItemTypeDef:
    return {
        "ConditionCheck": ...,
    }
```

```python title="Definition"
class TransactWriteItemTypeDef(TypedDict):
    ConditionCheck: NotRequired[ConditionCheckTypeDef],  # (1)
    Put: NotRequired[PutTypeDef],  # (2)
    Delete: NotRequired[DeleteTypeDef],  # (3)
    Update: NotRequired[UpdateTypeDef],  # (4)
```

1. See [:material-code-braces: ConditionCheckTypeDef](./type_defs.md#conditionchecktypedef) 
2. See [:material-code-braces: PutTypeDef](./type_defs.md#puttypedef) 
3. See [:material-code-braces: DeleteTypeDef](./type_defs.md#deletetypedef) 
4. See [:material-code-braces: UpdateTypeDef](./type_defs.md#updatetypedef) 
## TransactWriteItemsInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import TransactWriteItemsInputRequestTypeDef

def get_value() -> TransactWriteItemsInputRequestTypeDef:
    return {
        "TransactItems": ...,
    }
```

```python title="Definition"
class TransactWriteItemsInputRequestTypeDef(TypedDict):
    TransactItems: Sequence[TransactWriteItemTypeDef],  # (1)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (2)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (3)
    ClientRequestToken: NotRequired[str],
```

1. See [:material-code-braces: TransactWriteItemTypeDef](./type_defs.md#transactwriteitemtypedef) 
2. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
3. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
## TransactWriteItemsOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import TransactWriteItemsOutputTypeDef

def get_value() -> TransactWriteItemsOutputTypeDef:
    return {
        "ConsumedCapacity": ...,
        "ItemCollectionMetrics": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class TransactWriteItemsOutputTypeDef(TypedDict):
    ConsumedCapacity: List[ConsumedCapacityTypeDef],  # (1)
    ItemCollectionMetrics: Dict[str, List[ItemCollectionMetricsTypeDef]],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ItemCollectionMetricsTypeDef](./type_defs.md#itemcollectionmetricstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UntagResourceInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UntagResourceInputRequestTypeDef

def get_value() -> UntagResourceInputRequestTypeDef:
    return {
        "ResourceArn": ...,
        "TagKeys": ...,
    }
```

```python title="Definition"
class UntagResourceInputRequestTypeDef(TypedDict):
    ResourceArn: str,
    TagKeys: Sequence[str],
```

## UpdateContinuousBackupsInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateContinuousBackupsInputRequestTypeDef

def get_value() -> UpdateContinuousBackupsInputRequestTypeDef:
    return {
        "TableName": ...,
        "PointInTimeRecoverySpecification": ...,
    }
```

```python title="Definition"
class UpdateContinuousBackupsInputRequestTypeDef(TypedDict):
    TableName: str,
    PointInTimeRecoverySpecification: PointInTimeRecoverySpecificationTypeDef,  # (1)
```

1. See [:material-code-braces: PointInTimeRecoverySpecificationTypeDef](./type_defs.md#pointintimerecoveryspecificationtypedef) 
## UpdateContinuousBackupsOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateContinuousBackupsOutputTypeDef

def get_value() -> UpdateContinuousBackupsOutputTypeDef:
    return {
        "ContinuousBackupsDescription": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateContinuousBackupsOutputTypeDef(TypedDict):
    ContinuousBackupsDescription: ContinuousBackupsDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ContinuousBackupsDescriptionTypeDef](./type_defs.md#continuousbackupsdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateContributorInsightsInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateContributorInsightsInputRequestTypeDef

def get_value() -> UpdateContributorInsightsInputRequestTypeDef:
    return {
        "TableName": ...,
        "ContributorInsightsAction": ...,
    }
```

```python title="Definition"
class UpdateContributorInsightsInputRequestTypeDef(TypedDict):
    TableName: str,
    ContributorInsightsAction: ContributorInsightsActionType,  # (1)
    IndexName: NotRequired[str],
```

1. See [:material-code-brackets: ContributorInsightsActionType](./literals.md#contributorinsightsactiontype) 
## UpdateContributorInsightsOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateContributorInsightsOutputTypeDef

def get_value() -> UpdateContributorInsightsOutputTypeDef:
    return {
        "TableName": ...,
        "IndexName": ...,
        "ContributorInsightsStatus": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateContributorInsightsOutputTypeDef(TypedDict):
    TableName: str,
    IndexName: str,
    ContributorInsightsStatus: ContributorInsightsStatusType,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-brackets: ContributorInsightsStatusType](./literals.md#contributorinsightsstatustype) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGlobalSecondaryIndexActionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateGlobalSecondaryIndexActionTypeDef

def get_value() -> UpdateGlobalSecondaryIndexActionTypeDef:
    return {
        "IndexName": ...,
        "ProvisionedThroughput": ...,
    }
```

```python title="Definition"
class UpdateGlobalSecondaryIndexActionTypeDef(TypedDict):
    IndexName: str,
    ProvisionedThroughput: ProvisionedThroughputTypeDef,  # (1)
```

1. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
## UpdateGlobalTableInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateGlobalTableInputRequestTypeDef

def get_value() -> UpdateGlobalTableInputRequestTypeDef:
    return {
        "GlobalTableName": ...,
        "ReplicaUpdates": ...,
    }
```

```python title="Definition"
class UpdateGlobalTableInputRequestTypeDef(TypedDict):
    GlobalTableName: str,
    ReplicaUpdates: Sequence[ReplicaUpdateTypeDef],  # (1)
```

1. See [:material-code-braces: ReplicaUpdateTypeDef](./type_defs.md#replicaupdatetypedef) 
## UpdateGlobalTableOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateGlobalTableOutputTypeDef

def get_value() -> UpdateGlobalTableOutputTypeDef:
    return {
        "GlobalTableDescription": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateGlobalTableOutputTypeDef(TypedDict):
    GlobalTableDescription: GlobalTableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: GlobalTableDescriptionTypeDef](./type_defs.md#globaltabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateGlobalTableSettingsInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateGlobalTableSettingsInputRequestTypeDef

def get_value() -> UpdateGlobalTableSettingsInputRequestTypeDef:
    return {
        "GlobalTableName": ...,
    }
```

```python title="Definition"
class UpdateGlobalTableSettingsInputRequestTypeDef(TypedDict):
    GlobalTableName: str,
    GlobalTableBillingMode: NotRequired[BillingModeType],  # (1)
    GlobalTableProvisionedWriteCapacityUnits: NotRequired[int],
    GlobalTableProvisionedWriteCapacityAutoScalingSettingsUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (2)
    GlobalTableGlobalSecondaryIndexSettingsUpdate: NotRequired[Sequence[GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef]],  # (3)
    ReplicaSettingsUpdate: NotRequired[Sequence[ReplicaSettingsUpdateTypeDef]],  # (4)
```

1. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
2. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
3. See [:material-code-braces: GlobalTableGlobalSecondaryIndexSettingsUpdateTypeDef](./type_defs.md#globaltableglobalsecondaryindexsettingsupdatetypedef) 
4. See [:material-code-braces: ReplicaSettingsUpdateTypeDef](./type_defs.md#replicasettingsupdatetypedef) 
## UpdateGlobalTableSettingsOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateGlobalTableSettingsOutputTypeDef

def get_value() -> UpdateGlobalTableSettingsOutputTypeDef:
    return {
        "GlobalTableName": ...,
        "ReplicaSettings": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateGlobalTableSettingsOutputTypeDef(TypedDict):
    GlobalTableName: str,
    ReplicaSettings: List[ReplicaSettingsDescriptionTypeDef],  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ReplicaSettingsDescriptionTypeDef](./type_defs.md#replicasettingsdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateItemInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateItemInputRequestTypeDef

def get_value() -> UpdateItemInputRequestTypeDef:
    return {
        "TableName": ...,
        "Key": ...,
    }
```

```python title="Definition"
class UpdateItemInputRequestTypeDef(TypedDict):
    TableName: str,
    Key: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    AttributeUpdates: NotRequired[Mapping[str, AttributeValueUpdateTypeDef]],  # (1)
    Expected: NotRequired[Mapping[str, ExpectedAttributeValueTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (3)
    ReturnValues: NotRequired[ReturnValueType],  # (4)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (5)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (6)
    UpdateExpression: NotRequired[str],
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
```

1. See [:material-code-braces: AttributeValueUpdateTypeDef](./type_defs.md#attributevalueupdatetypedef) 
2. See [:material-code-braces: ExpectedAttributeValueTypeDef](./type_defs.md#expectedattributevaluetypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
6. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
## UpdateItemInputTableUpdateItemTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateItemInputTableUpdateItemTypeDef

def get_value() -> UpdateItemInputTableUpdateItemTypeDef:
    return {
        "Key": ...,
    }
```

```python title="Definition"
class UpdateItemInputTableUpdateItemTypeDef(TypedDict):
    Key: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    AttributeUpdates: NotRequired[Mapping[str, AttributeValueUpdateTypeDef]],  # (1)
    Expected: NotRequired[Mapping[str, ExpectedAttributeValueTypeDef]],  # (2)
    ConditionalOperator: NotRequired[ConditionalOperatorType],  # (3)
    ReturnValues: NotRequired[ReturnValueType],  # (4)
    ReturnConsumedCapacity: NotRequired[ReturnConsumedCapacityType],  # (5)
    ReturnItemCollectionMetrics: NotRequired[ReturnItemCollectionMetricsType],  # (6)
    UpdateExpression: NotRequired[str],
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
```

1. See [:material-code-braces: AttributeValueUpdateTypeDef](./type_defs.md#attributevalueupdatetypedef) 
2. See [:material-code-braces: ExpectedAttributeValueTypeDef](./type_defs.md#expectedattributevaluetypedef) 
3. See [:material-code-brackets: ConditionalOperatorType](./literals.md#conditionaloperatortype) 
4. See [:material-code-brackets: ReturnValueType](./literals.md#returnvaluetype) 
5. See [:material-code-brackets: ReturnConsumedCapacityType](./literals.md#returnconsumedcapacitytype) 
6. See [:material-code-brackets: ReturnItemCollectionMetricsType](./literals.md#returnitemcollectionmetricstype) 
## UpdateItemOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateItemOutputTypeDef

def get_value() -> UpdateItemOutputTypeDef:
    return {
        "Attributes": ...,
        "ConsumedCapacity": ...,
        "ItemCollectionMetrics": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateItemOutputTypeDef(TypedDict):
    Attributes: Dict[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    ConsumedCapacity: ConsumedCapacityTypeDef,  # (1)
    ItemCollectionMetrics: ItemCollectionMetricsTypeDef,  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: ConsumedCapacityTypeDef](./type_defs.md#consumedcapacitytypedef) 
2. See [:material-code-braces: ItemCollectionMetricsTypeDef](./type_defs.md#itemcollectionmetricstypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateReplicationGroupMemberActionTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateReplicationGroupMemberActionTypeDef

def get_value() -> UpdateReplicationGroupMemberActionTypeDef:
    return {
        "RegionName": ...,
    }
```

```python title="Definition"
class UpdateReplicationGroupMemberActionTypeDef(TypedDict):
    RegionName: str,
    KMSMasterKeyId: NotRequired[str],
    ProvisionedThroughputOverride: NotRequired[ProvisionedThroughputOverrideTypeDef],  # (1)
    GlobalSecondaryIndexes: NotRequired[Sequence[ReplicaGlobalSecondaryIndexTypeDef]],  # (2)
    TableClassOverride: NotRequired[TableClassType],  # (3)
```

1. See [:material-code-braces: ProvisionedThroughputOverrideTypeDef](./type_defs.md#provisionedthroughputoverridetypedef) 
2. See [:material-code-braces: ReplicaGlobalSecondaryIndexTypeDef](./type_defs.md#replicaglobalsecondaryindextypedef) 
3. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
## UpdateTableInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateTableInputRequestTypeDef

def get_value() -> UpdateTableInputRequestTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class UpdateTableInputRequestTypeDef(TypedDict):
    TableName: str,
    AttributeDefinitions: NotRequired[Sequence[AttributeDefinitionTypeDef]],  # (1)
    BillingMode: NotRequired[BillingModeType],  # (2)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (3)
    GlobalSecondaryIndexUpdates: NotRequired[Sequence[GlobalSecondaryIndexUpdateTypeDef]],  # (4)
    StreamSpecification: NotRequired[StreamSpecificationTypeDef],  # (5)
    SSESpecification: NotRequired[SSESpecificationTypeDef],  # (6)
    ReplicaUpdates: NotRequired[Sequence[ReplicationGroupUpdateTypeDef]],  # (7)
    TableClass: NotRequired[TableClassType],  # (8)
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
3. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
4. See [:material-code-braces: GlobalSecondaryIndexUpdateTypeDef](./type_defs.md#globalsecondaryindexupdatetypedef) 
5. See [:material-code-braces: StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef) 
6. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
7. See [:material-code-braces: ReplicationGroupUpdateTypeDef](./type_defs.md#replicationgroupupdatetypedef) 
8. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
## UpdateTableInputTableUpdateTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateTableInputTableUpdateTypeDef

def get_value() -> UpdateTableInputTableUpdateTypeDef:
    return {
        "AttributeDefinitions": ...,
    }
```

```python title="Definition"
class UpdateTableInputTableUpdateTypeDef(TypedDict):
    AttributeDefinitions: NotRequired[Sequence[AttributeDefinitionTypeDef]],  # (1)
    BillingMode: NotRequired[BillingModeType],  # (2)
    ProvisionedThroughput: NotRequired[ProvisionedThroughputTypeDef],  # (3)
    GlobalSecondaryIndexUpdates: NotRequired[Sequence[GlobalSecondaryIndexUpdateTypeDef]],  # (4)
    StreamSpecification: NotRequired[StreamSpecificationTypeDef],  # (5)
    SSESpecification: NotRequired[SSESpecificationTypeDef],  # (6)
    ReplicaUpdates: NotRequired[Sequence[ReplicationGroupUpdateTypeDef]],  # (7)
    TableClass: NotRequired[TableClassType],  # (8)
```

1. See [:material-code-braces: AttributeDefinitionTypeDef](./type_defs.md#attributedefinitiontypedef) 
2. See [:material-code-brackets: BillingModeType](./literals.md#billingmodetype) 
3. See [:material-code-braces: ProvisionedThroughputTypeDef](./type_defs.md#provisionedthroughputtypedef) 
4. See [:material-code-braces: GlobalSecondaryIndexUpdateTypeDef](./type_defs.md#globalsecondaryindexupdatetypedef) 
5. See [:material-code-braces: StreamSpecificationTypeDef](./type_defs.md#streamspecificationtypedef) 
6. See [:material-code-braces: SSESpecificationTypeDef](./type_defs.md#ssespecificationtypedef) 
7. See [:material-code-braces: ReplicationGroupUpdateTypeDef](./type_defs.md#replicationgroupupdatetypedef) 
8. See [:material-code-brackets: TableClassType](./literals.md#tableclasstype) 
## UpdateTableOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateTableOutputTypeDef

def get_value() -> UpdateTableOutputTypeDef:
    return {
        "TableDescription": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateTableOutputTypeDef(TypedDict):
    TableDescription: TableDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableDescriptionTypeDef](./type_defs.md#tabledescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTableReplicaAutoScalingInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateTableReplicaAutoScalingInputRequestTypeDef

def get_value() -> UpdateTableReplicaAutoScalingInputRequestTypeDef:
    return {
        "TableName": ...,
    }
```

```python title="Definition"
class UpdateTableReplicaAutoScalingInputRequestTypeDef(TypedDict):
    TableName: str,
    GlobalSecondaryIndexUpdates: NotRequired[Sequence[GlobalSecondaryIndexAutoScalingUpdateTypeDef]],  # (1)
    ProvisionedWriteCapacityAutoScalingUpdate: NotRequired[AutoScalingSettingsUpdateTypeDef],  # (2)
    ReplicaUpdates: NotRequired[Sequence[ReplicaAutoScalingUpdateTypeDef]],  # (3)
```

1. See [:material-code-braces: GlobalSecondaryIndexAutoScalingUpdateTypeDef](./type_defs.md#globalsecondaryindexautoscalingupdatetypedef) 
2. See [:material-code-braces: AutoScalingSettingsUpdateTypeDef](./type_defs.md#autoscalingsettingsupdatetypedef) 
3. See [:material-code-braces: ReplicaAutoScalingUpdateTypeDef](./type_defs.md#replicaautoscalingupdatetypedef) 
## UpdateTableReplicaAutoScalingOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateTableReplicaAutoScalingOutputTypeDef

def get_value() -> UpdateTableReplicaAutoScalingOutputTypeDef:
    return {
        "TableAutoScalingDescription": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateTableReplicaAutoScalingOutputTypeDef(TypedDict):
    TableAutoScalingDescription: TableAutoScalingDescriptionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableAutoScalingDescriptionTypeDef](./type_defs.md#tableautoscalingdescriptiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTimeToLiveInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateTimeToLiveInputRequestTypeDef

def get_value() -> UpdateTimeToLiveInputRequestTypeDef:
    return {
        "TableName": ...,
        "TimeToLiveSpecification": ...,
    }
```

```python title="Definition"
class UpdateTimeToLiveInputRequestTypeDef(TypedDict):
    TableName: str,
    TimeToLiveSpecification: TimeToLiveSpecificationTypeDef,  # (1)
```

1. See [:material-code-braces: TimeToLiveSpecificationTypeDef](./type_defs.md#timetolivespecificationtypedef) 
## UpdateTimeToLiveOutputTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateTimeToLiveOutputTypeDef

def get_value() -> UpdateTimeToLiveOutputTypeDef:
    return {
        "TimeToLiveSpecification": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class UpdateTimeToLiveOutputTypeDef(TypedDict):
    TimeToLiveSpecification: TimeToLiveSpecificationTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TimeToLiveSpecificationTypeDef](./type_defs.md#timetolivespecificationtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## UpdateTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import UpdateTypeDef

def get_value() -> UpdateTypeDef:
    return {
        "Key": ...,
        "UpdateExpression": ...,
        "TableName": ...,
    }
```

```python title="Definition"
class UpdateTypeDef(TypedDict):
    Key: Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]],
    UpdateExpression: str,
    TableName: str,
    ConditionExpression: NotRequired[str],
    ExpressionAttributeNames: NotRequired[Mapping[str, str]],
    ExpressionAttributeValues: NotRequired[Mapping[str, Union[bytes, bytearray, str, int, Decimal, bool, Set[int], Set[Decimal], Set[str], Set[bytes], Set[bytearray], Sequence[Any], Mapping[str, Any], None]]],
    ReturnValuesOnConditionCheckFailure: NotRequired[ReturnValuesOnConditionCheckFailureType],  # (1)
```

1. See [:material-code-brackets: ReturnValuesOnConditionCheckFailureType](./literals.md#returnvaluesonconditioncheckfailuretype) 
## WaiterConfigTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import WaiterConfigTypeDef

def get_value() -> WaiterConfigTypeDef:
    return {
        "Delay": ...,
    }
```

```python title="Definition"
class WaiterConfigTypeDef(TypedDict):
    Delay: NotRequired[int],
    MaxAttempts: NotRequired[int],
```

## WriteRequestTypeDef

```python title="Usage Example"
from mypy_boto3_dynamodb.type_defs import WriteRequestTypeDef

def get_value() -> WriteRequestTypeDef:
    return {
        "PutRequest": ...,
    }
```

```python title="Definition"
class WriteRequestTypeDef(TypedDict):
    PutRequest: NotRequired[PutRequestTypeDef],  # (1)
    DeleteRequest: NotRequired[DeleteRequestTypeDef],  # (2)
```

1. See [:material-code-braces: PutRequestTypeDef](./type_defs.md#putrequesttypedef) 
2. See [:material-code-braces: DeleteRequestTypeDef](./type_defs.md#deleterequesttypedef) 
