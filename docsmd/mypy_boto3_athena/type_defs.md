# Typed dictionaries

> [Index](../README.md) > [Athena](./README.md) > Typed dictionaries

!!! note ""

    Auto-generated documentation for [Athena](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/athena.html#Athena)
    type annotations stubs module [mypy-boto3-athena](https://pypi.org/project/mypy-boto3-athena/).

## AclConfigurationTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import AclConfigurationTypeDef

def get_value() -> AclConfigurationTypeDef:
    return {
        "S3AclOption": ...,
    }
```

```python title="Definition"
class AclConfigurationTypeDef(TypedDict):
    S3AclOption: S3AclOptionType,  # (1)
```

1. See [:material-code-brackets: S3AclOptionType](./literals.md#s3acloptiontype) 
## AthenaErrorTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import AthenaErrorTypeDef

def get_value() -> AthenaErrorTypeDef:
    return {
        "ErrorCategory": ...,
    }
```

```python title="Definition"
class AthenaErrorTypeDef(TypedDict):
    ErrorCategory: NotRequired[int],
    ErrorType: NotRequired[int],
```

## BatchGetNamedQueryInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import BatchGetNamedQueryInputRequestTypeDef

def get_value() -> BatchGetNamedQueryInputRequestTypeDef:
    return {
        "NamedQueryIds": ...,
    }
```

```python title="Definition"
class BatchGetNamedQueryInputRequestTypeDef(TypedDict):
    NamedQueryIds: Sequence[str],
```

## BatchGetNamedQueryOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import BatchGetNamedQueryOutputTypeDef

def get_value() -> BatchGetNamedQueryOutputTypeDef:
    return {
        "NamedQueries": ...,
        "UnprocessedNamedQueryIds": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class BatchGetNamedQueryOutputTypeDef(TypedDict):
    NamedQueries: List[NamedQueryTypeDef],  # (1)
    UnprocessedNamedQueryIds: List[UnprocessedNamedQueryIdTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: NamedQueryTypeDef](./type_defs.md#namedquerytypedef) 
2. See [:material-code-braces: UnprocessedNamedQueryIdTypeDef](./type_defs.md#unprocessednamedqueryidtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## BatchGetQueryExecutionInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import BatchGetQueryExecutionInputRequestTypeDef

def get_value() -> BatchGetQueryExecutionInputRequestTypeDef:
    return {
        "QueryExecutionIds": ...,
    }
```

```python title="Definition"
class BatchGetQueryExecutionInputRequestTypeDef(TypedDict):
    QueryExecutionIds: Sequence[str],
```

## BatchGetQueryExecutionOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import BatchGetQueryExecutionOutputTypeDef

def get_value() -> BatchGetQueryExecutionOutputTypeDef:
    return {
        "QueryExecutions": ...,
        "UnprocessedQueryExecutionIds": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class BatchGetQueryExecutionOutputTypeDef(TypedDict):
    QueryExecutions: List[QueryExecutionTypeDef],  # (1)
    UnprocessedQueryExecutionIds: List[UnprocessedQueryExecutionIdTypeDef],  # (2)
    ResponseMetadata: ResponseMetadataTypeDef,  # (3)
```

1. See [:material-code-braces: QueryExecutionTypeDef](./type_defs.md#queryexecutiontypedef) 
2. See [:material-code-braces: UnprocessedQueryExecutionIdTypeDef](./type_defs.md#unprocessedqueryexecutionidtypedef) 
3. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ColumnInfoTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ColumnInfoTypeDef

def get_value() -> ColumnInfoTypeDef:
    return {
        "Name": ...,
        "Type": ...,
    }
```

```python title="Definition"
class ColumnInfoTypeDef(TypedDict):
    Name: str,
    Type: str,
    CatalogName: NotRequired[str],
    SchemaName: NotRequired[str],
    TableName: NotRequired[str],
    Label: NotRequired[str],
    Precision: NotRequired[int],
    Scale: NotRequired[int],
    Nullable: NotRequired[ColumnNullableType],  # (1)
    CaseSensitive: NotRequired[bool],
```

1. See [:material-code-brackets: ColumnNullableType](./literals.md#columnnullabletype) 
## ColumnTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ColumnTypeDef

def get_value() -> ColumnTypeDef:
    return {
        "Name": ...,
    }
```

```python title="Definition"
class ColumnTypeDef(TypedDict):
    Name: str,
    Type: NotRequired[str],
    Comment: NotRequired[str],
```

## CreateDataCatalogInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import CreateDataCatalogInputRequestTypeDef

def get_value() -> CreateDataCatalogInputRequestTypeDef:
    return {
        "Name": ...,
        "Type": ...,
    }
```

```python title="Definition"
class CreateDataCatalogInputRequestTypeDef(TypedDict):
    Name: str,
    Type: DataCatalogTypeType,  # (1)
    Description: NotRequired[str],
    Parameters: NotRequired[Mapping[str, str]],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-brackets: DataCatalogTypeType](./literals.md#datacatalogtypetype) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## CreateNamedQueryInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import CreateNamedQueryInputRequestTypeDef

def get_value() -> CreateNamedQueryInputRequestTypeDef:
    return {
        "Name": ...,
        "Database": ...,
        "QueryString": ...,
    }
```

```python title="Definition"
class CreateNamedQueryInputRequestTypeDef(TypedDict):
    Name: str,
    Database: str,
    QueryString: str,
    Description: NotRequired[str],
    ClientRequestToken: NotRequired[str],
    WorkGroup: NotRequired[str],
```

## CreateNamedQueryOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import CreateNamedQueryOutputTypeDef

def get_value() -> CreateNamedQueryOutputTypeDef:
    return {
        "NamedQueryId": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class CreateNamedQueryOutputTypeDef(TypedDict):
    NamedQueryId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## CreatePreparedStatementInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import CreatePreparedStatementInputRequestTypeDef

def get_value() -> CreatePreparedStatementInputRequestTypeDef:
    return {
        "StatementName": ...,
        "WorkGroup": ...,
        "QueryStatement": ...,
    }
```

```python title="Definition"
class CreatePreparedStatementInputRequestTypeDef(TypedDict):
    StatementName: str,
    WorkGroup: str,
    QueryStatement: str,
    Description: NotRequired[str],
```

## CreateWorkGroupInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import CreateWorkGroupInputRequestTypeDef

def get_value() -> CreateWorkGroupInputRequestTypeDef:
    return {
        "Name": ...,
    }
```

```python title="Definition"
class CreateWorkGroupInputRequestTypeDef(TypedDict):
    Name: str,
    Configuration: NotRequired[WorkGroupConfigurationTypeDef],  # (1)
    Description: NotRequired[str],
    Tags: NotRequired[Sequence[TagTypeDef]],  # (2)
```

1. See [:material-code-braces: WorkGroupConfigurationTypeDef](./type_defs.md#workgroupconfigurationtypedef) 
2. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## DataCatalogSummaryTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import DataCatalogSummaryTypeDef

def get_value() -> DataCatalogSummaryTypeDef:
    return {
        "CatalogName": ...,
    }
```

```python title="Definition"
class DataCatalogSummaryTypeDef(TypedDict):
    CatalogName: NotRequired[str],
    Type: NotRequired[DataCatalogTypeType],  # (1)
```

1. See [:material-code-brackets: DataCatalogTypeType](./literals.md#datacatalogtypetype) 
## DataCatalogTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import DataCatalogTypeDef

def get_value() -> DataCatalogTypeDef:
    return {
        "Name": ...,
        "Type": ...,
    }
```

```python title="Definition"
class DataCatalogTypeDef(TypedDict):
    Name: str,
    Type: DataCatalogTypeType,  # (1)
    Description: NotRequired[str],
    Parameters: NotRequired[Dict[str, str]],
```

1. See [:material-code-brackets: DataCatalogTypeType](./literals.md#datacatalogtypetype) 
## DatabaseTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import DatabaseTypeDef

def get_value() -> DatabaseTypeDef:
    return {
        "Name": ...,
    }
```

```python title="Definition"
class DatabaseTypeDef(TypedDict):
    Name: str,
    Description: NotRequired[str],
    Parameters: NotRequired[Dict[str, str]],
```

## DatumTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import DatumTypeDef

def get_value() -> DatumTypeDef:
    return {
        "VarCharValue": ...,
    }
```

```python title="Definition"
class DatumTypeDef(TypedDict):
    VarCharValue: NotRequired[str],
```

## DeleteDataCatalogInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import DeleteDataCatalogInputRequestTypeDef

def get_value() -> DeleteDataCatalogInputRequestTypeDef:
    return {
        "Name": ...,
    }
```

```python title="Definition"
class DeleteDataCatalogInputRequestTypeDef(TypedDict):
    Name: str,
```

## DeleteNamedQueryInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import DeleteNamedQueryInputRequestTypeDef

def get_value() -> DeleteNamedQueryInputRequestTypeDef:
    return {
        "NamedQueryId": ...,
    }
```

```python title="Definition"
class DeleteNamedQueryInputRequestTypeDef(TypedDict):
    NamedQueryId: str,
```

## DeletePreparedStatementInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import DeletePreparedStatementInputRequestTypeDef

def get_value() -> DeletePreparedStatementInputRequestTypeDef:
    return {
        "StatementName": ...,
        "WorkGroup": ...,
    }
```

```python title="Definition"
class DeletePreparedStatementInputRequestTypeDef(TypedDict):
    StatementName: str,
    WorkGroup: str,
```

## DeleteWorkGroupInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import DeleteWorkGroupInputRequestTypeDef

def get_value() -> DeleteWorkGroupInputRequestTypeDef:
    return {
        "WorkGroup": ...,
    }
```

```python title="Definition"
class DeleteWorkGroupInputRequestTypeDef(TypedDict):
    WorkGroup: str,
    RecursiveDeleteOption: NotRequired[bool],
```

## EncryptionConfigurationTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import EncryptionConfigurationTypeDef

def get_value() -> EncryptionConfigurationTypeDef:
    return {
        "EncryptionOption": ...,
    }
```

```python title="Definition"
class EncryptionConfigurationTypeDef(TypedDict):
    EncryptionOption: EncryptionOptionType,  # (1)
    KmsKey: NotRequired[str],
```

1. See [:material-code-brackets: EncryptionOptionType](./literals.md#encryptionoptiontype) 
## EngineVersionTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import EngineVersionTypeDef

def get_value() -> EngineVersionTypeDef:
    return {
        "SelectedEngineVersion": ...,
    }
```

```python title="Definition"
class EngineVersionTypeDef(TypedDict):
    SelectedEngineVersion: NotRequired[str],
    EffectiveEngineVersion: NotRequired[str],
```

## GetDataCatalogInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import GetDataCatalogInputRequestTypeDef

def get_value() -> GetDataCatalogInputRequestTypeDef:
    return {
        "Name": ...,
    }
```

```python title="Definition"
class GetDataCatalogInputRequestTypeDef(TypedDict):
    Name: str,
```

## GetDataCatalogOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import GetDataCatalogOutputTypeDef

def get_value() -> GetDataCatalogOutputTypeDef:
    return {
        "DataCatalog": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetDataCatalogOutputTypeDef(TypedDict):
    DataCatalog: DataCatalogTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataCatalogTypeDef](./type_defs.md#datacatalogtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetDatabaseInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import GetDatabaseInputRequestTypeDef

def get_value() -> GetDatabaseInputRequestTypeDef:
    return {
        "CatalogName": ...,
        "DatabaseName": ...,
    }
```

```python title="Definition"
class GetDatabaseInputRequestTypeDef(TypedDict):
    CatalogName: str,
    DatabaseName: str,
```

## GetDatabaseOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import GetDatabaseOutputTypeDef

def get_value() -> GetDatabaseOutputTypeDef:
    return {
        "Database": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetDatabaseOutputTypeDef(TypedDict):
    Database: DatabaseTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatabaseTypeDef](./type_defs.md#databasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetNamedQueryInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import GetNamedQueryInputRequestTypeDef

def get_value() -> GetNamedQueryInputRequestTypeDef:
    return {
        "NamedQueryId": ...,
    }
```

```python title="Definition"
class GetNamedQueryInputRequestTypeDef(TypedDict):
    NamedQueryId: str,
```

## GetNamedQueryOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import GetNamedQueryOutputTypeDef

def get_value() -> GetNamedQueryOutputTypeDef:
    return {
        "NamedQuery": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetNamedQueryOutputTypeDef(TypedDict):
    NamedQuery: NamedQueryTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: NamedQueryTypeDef](./type_defs.md#namedquerytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetPreparedStatementInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import GetPreparedStatementInputRequestTypeDef

def get_value() -> GetPreparedStatementInputRequestTypeDef:
    return {
        "StatementName": ...,
        "WorkGroup": ...,
    }
```

```python title="Definition"
class GetPreparedStatementInputRequestTypeDef(TypedDict):
    StatementName: str,
    WorkGroup: str,
```

## GetPreparedStatementOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import GetPreparedStatementOutputTypeDef

def get_value() -> GetPreparedStatementOutputTypeDef:
    return {
        "PreparedStatement": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetPreparedStatementOutputTypeDef(TypedDict):
    PreparedStatement: PreparedStatementTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PreparedStatementTypeDef](./type_defs.md#preparedstatementtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQueryExecutionInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import GetQueryExecutionInputRequestTypeDef

def get_value() -> GetQueryExecutionInputRequestTypeDef:
    return {
        "QueryExecutionId": ...,
    }
```

```python title="Definition"
class GetQueryExecutionInputRequestTypeDef(TypedDict):
    QueryExecutionId: str,
```

## GetQueryExecutionOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import GetQueryExecutionOutputTypeDef

def get_value() -> GetQueryExecutionOutputTypeDef:
    return {
        "QueryExecution": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetQueryExecutionOutputTypeDef(TypedDict):
    QueryExecution: QueryExecutionTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: QueryExecutionTypeDef](./type_defs.md#queryexecutiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetQueryResultsInputGetQueryResultsPaginateTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import GetQueryResultsInputGetQueryResultsPaginateTypeDef

def get_value() -> GetQueryResultsInputGetQueryResultsPaginateTypeDef:
    return {
        "QueryExecutionId": ...,
    }
```

```python title="Definition"
class GetQueryResultsInputGetQueryResultsPaginateTypeDef(TypedDict):
    QueryExecutionId: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## GetQueryResultsInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import GetQueryResultsInputRequestTypeDef

def get_value() -> GetQueryResultsInputRequestTypeDef:
    return {
        "QueryExecutionId": ...,
    }
```

```python title="Definition"
class GetQueryResultsInputRequestTypeDef(TypedDict):
    QueryExecutionId: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## GetQueryResultsOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import GetQueryResultsOutputTypeDef

def get_value() -> GetQueryResultsOutputTypeDef:
    return {
        "UpdateCount": ...,
        "ResultSet": ...,
        "NextToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetQueryResultsOutputTypeDef(TypedDict):
    UpdateCount: int,
    ResultSet: ResultSetTypeDef,  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: ResultSetTypeDef](./type_defs.md#resultsettypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetTableMetadataInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import GetTableMetadataInputRequestTypeDef

def get_value() -> GetTableMetadataInputRequestTypeDef:
    return {
        "CatalogName": ...,
        "DatabaseName": ...,
        "TableName": ...,
    }
```

```python title="Definition"
class GetTableMetadataInputRequestTypeDef(TypedDict):
    CatalogName: str,
    DatabaseName: str,
    TableName: str,
```

## GetTableMetadataOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import GetTableMetadataOutputTypeDef

def get_value() -> GetTableMetadataOutputTypeDef:
    return {
        "TableMetadata": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetTableMetadataOutputTypeDef(TypedDict):
    TableMetadata: TableMetadataTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableMetadataTypeDef](./type_defs.md#tablemetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## GetWorkGroupInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import GetWorkGroupInputRequestTypeDef

def get_value() -> GetWorkGroupInputRequestTypeDef:
    return {
        "WorkGroup": ...,
    }
```

```python title="Definition"
class GetWorkGroupInputRequestTypeDef(TypedDict):
    WorkGroup: str,
```

## GetWorkGroupOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import GetWorkGroupOutputTypeDef

def get_value() -> GetWorkGroupOutputTypeDef:
    return {
        "WorkGroup": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class GetWorkGroupOutputTypeDef(TypedDict):
    WorkGroup: WorkGroupTypeDef,  # (1)
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkGroupTypeDef](./type_defs.md#workgrouptypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDataCatalogsInputListDataCatalogsPaginateTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListDataCatalogsInputListDataCatalogsPaginateTypeDef

def get_value() -> ListDataCatalogsInputListDataCatalogsPaginateTypeDef:
    return {
        "PaginationConfig": ...,
    }
```

```python title="Definition"
class ListDataCatalogsInputListDataCatalogsPaginateTypeDef(TypedDict):
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDataCatalogsInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListDataCatalogsInputRequestTypeDef

def get_value() -> ListDataCatalogsInputRequestTypeDef:
    return {
        "NextToken": ...,
    }
```

```python title="Definition"
class ListDataCatalogsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDataCatalogsOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListDataCatalogsOutputTypeDef

def get_value() -> ListDataCatalogsOutputTypeDef:
    return {
        "DataCatalogsSummary": ...,
        "NextToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListDataCatalogsOutputTypeDef(TypedDict):
    DataCatalogsSummary: List[DataCatalogSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DataCatalogSummaryTypeDef](./type_defs.md#datacatalogsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListDatabasesInputListDatabasesPaginateTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListDatabasesInputListDatabasesPaginateTypeDef

def get_value() -> ListDatabasesInputListDatabasesPaginateTypeDef:
    return {
        "CatalogName": ...,
    }
```

```python title="Definition"
class ListDatabasesInputListDatabasesPaginateTypeDef(TypedDict):
    CatalogName: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListDatabasesInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListDatabasesInputRequestTypeDef

def get_value() -> ListDatabasesInputRequestTypeDef:
    return {
        "CatalogName": ...,
    }
```

```python title="Definition"
class ListDatabasesInputRequestTypeDef(TypedDict):
    CatalogName: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListDatabasesOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListDatabasesOutputTypeDef

def get_value() -> ListDatabasesOutputTypeDef:
    return {
        "DatabaseList": ...,
        "NextToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListDatabasesOutputTypeDef(TypedDict):
    DatabaseList: List[DatabaseTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: DatabaseTypeDef](./type_defs.md#databasetypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListEngineVersionsInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListEngineVersionsInputRequestTypeDef

def get_value() -> ListEngineVersionsInputRequestTypeDef:
    return {
        "NextToken": ...,
    }
```

```python title="Definition"
class ListEngineVersionsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListEngineVersionsOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListEngineVersionsOutputTypeDef

def get_value() -> ListEngineVersionsOutputTypeDef:
    return {
        "EngineVersions": ...,
        "NextToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListEngineVersionsOutputTypeDef(TypedDict):
    EngineVersions: List[EngineVersionTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: EngineVersionTypeDef](./type_defs.md#engineversiontypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListNamedQueriesInputListNamedQueriesPaginateTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListNamedQueriesInputListNamedQueriesPaginateTypeDef

def get_value() -> ListNamedQueriesInputListNamedQueriesPaginateTypeDef:
    return {
        "WorkGroup": ...,
    }
```

```python title="Definition"
class ListNamedQueriesInputListNamedQueriesPaginateTypeDef(TypedDict):
    WorkGroup: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListNamedQueriesInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListNamedQueriesInputRequestTypeDef

def get_value() -> ListNamedQueriesInputRequestTypeDef:
    return {
        "NextToken": ...,
    }
```

```python title="Definition"
class ListNamedQueriesInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    WorkGroup: NotRequired[str],
```

## ListNamedQueriesOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListNamedQueriesOutputTypeDef

def get_value() -> ListNamedQueriesOutputTypeDef:
    return {
        "NamedQueryIds": ...,
        "NextToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListNamedQueriesOutputTypeDef(TypedDict):
    NamedQueryIds: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListPreparedStatementsInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListPreparedStatementsInputRequestTypeDef

def get_value() -> ListPreparedStatementsInputRequestTypeDef:
    return {
        "WorkGroup": ...,
    }
```

```python title="Definition"
class ListPreparedStatementsInputRequestTypeDef(TypedDict):
    WorkGroup: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListPreparedStatementsOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListPreparedStatementsOutputTypeDef

def get_value() -> ListPreparedStatementsOutputTypeDef:
    return {
        "PreparedStatements": ...,
        "NextToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListPreparedStatementsOutputTypeDef(TypedDict):
    PreparedStatements: List[PreparedStatementSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: PreparedStatementSummaryTypeDef](./type_defs.md#preparedstatementsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef

def get_value() -> ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef:
    return {
        "WorkGroup": ...,
    }
```

```python title="Definition"
class ListQueryExecutionsInputListQueryExecutionsPaginateTypeDef(TypedDict):
    WorkGroup: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListQueryExecutionsInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListQueryExecutionsInputRequestTypeDef

def get_value() -> ListQueryExecutionsInputRequestTypeDef:
    return {
        "NextToken": ...,
    }
```

```python title="Definition"
class ListQueryExecutionsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
    WorkGroup: NotRequired[str],
```

## ListQueryExecutionsOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListQueryExecutionsOutputTypeDef

def get_value() -> ListQueryExecutionsOutputTypeDef:
    return {
        "QueryExecutionIds": ...,
        "NextToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListQueryExecutionsOutputTypeDef(TypedDict):
    QueryExecutionIds: List[str],
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTableMetadataInputListTableMetadataPaginateTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListTableMetadataInputListTableMetadataPaginateTypeDef

def get_value() -> ListTableMetadataInputListTableMetadataPaginateTypeDef:
    return {
        "CatalogName": ...,
        "DatabaseName": ...,
    }
```

```python title="Definition"
class ListTableMetadataInputListTableMetadataPaginateTypeDef(TypedDict):
    CatalogName: str,
    DatabaseName: str,
    Expression: NotRequired[str],
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTableMetadataInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListTableMetadataInputRequestTypeDef

def get_value() -> ListTableMetadataInputRequestTypeDef:
    return {
        "CatalogName": ...,
        "DatabaseName": ...,
    }
```

```python title="Definition"
class ListTableMetadataInputRequestTypeDef(TypedDict):
    CatalogName: str,
    DatabaseName: str,
    Expression: NotRequired[str],
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTableMetadataOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListTableMetadataOutputTypeDef

def get_value() -> ListTableMetadataOutputTypeDef:
    return {
        "TableMetadataList": ...,
        "NextToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListTableMetadataOutputTypeDef(TypedDict):
    TableMetadataList: List[TableMetadataTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TableMetadataTypeDef](./type_defs.md#tablemetadatatypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListTagsForResourceInputListTagsForResourcePaginateTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListTagsForResourceInputListTagsForResourcePaginateTypeDef

def get_value() -> ListTagsForResourceInputListTagsForResourcePaginateTypeDef:
    return {
        "ResourceARN": ...,
    }
```

```python title="Definition"
class ListTagsForResourceInputListTagsForResourcePaginateTypeDef(TypedDict):
    ResourceARN: str,
    PaginationConfig: NotRequired[PaginatorConfigTypeDef],  # (1)
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
## ListTagsForResourceInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListTagsForResourceInputRequestTypeDef

def get_value() -> ListTagsForResourceInputRequestTypeDef:
    return {
        "ResourceARN": ...,
    }
```

```python title="Definition"
class ListTagsForResourceInputRequestTypeDef(TypedDict):
    ResourceARN: str,
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListTagsForResourceOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListTagsForResourceOutputTypeDef

def get_value() -> ListTagsForResourceOutputTypeDef:
    return {
        "Tags": ...,
        "NextToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListTagsForResourceOutputTypeDef(TypedDict):
    Tags: List[TagTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## ListWorkGroupsInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListWorkGroupsInputRequestTypeDef

def get_value() -> ListWorkGroupsInputRequestTypeDef:
    return {
        "NextToken": ...,
    }
```

```python title="Definition"
class ListWorkGroupsInputRequestTypeDef(TypedDict):
    NextToken: NotRequired[str],
    MaxResults: NotRequired[int],
```

## ListWorkGroupsOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ListWorkGroupsOutputTypeDef

def get_value() -> ListWorkGroupsOutputTypeDef:
    return {
        "WorkGroups": ...,
        "NextToken": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class ListWorkGroupsOutputTypeDef(TypedDict):
    WorkGroups: List[WorkGroupSummaryTypeDef],  # (1)
    NextToken: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (2)
```

1. See [:material-code-braces: WorkGroupSummaryTypeDef](./type_defs.md#workgroupsummarytypedef) 
2. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## NamedQueryTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import NamedQueryTypeDef

def get_value() -> NamedQueryTypeDef:
    return {
        "Name": ...,
        "Database": ...,
        "QueryString": ...,
    }
```

```python title="Definition"
class NamedQueryTypeDef(TypedDict):
    Name: str,
    Database: str,
    QueryString: str,
    Description: NotRequired[str],
    NamedQueryId: NotRequired[str],
    WorkGroup: NotRequired[str],
```

## PaginatorConfigTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import PaginatorConfigTypeDef

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

## PreparedStatementSummaryTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import PreparedStatementSummaryTypeDef

def get_value() -> PreparedStatementSummaryTypeDef:
    return {
        "StatementName": ...,
    }
```

```python title="Definition"
class PreparedStatementSummaryTypeDef(TypedDict):
    StatementName: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
```

## PreparedStatementTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import PreparedStatementTypeDef

def get_value() -> PreparedStatementTypeDef:
    return {
        "StatementName": ...,
    }
```

```python title="Definition"
class PreparedStatementTypeDef(TypedDict):
    StatementName: NotRequired[str],
    QueryStatement: NotRequired[str],
    WorkGroupName: NotRequired[str],
    Description: NotRequired[str],
    LastModifiedTime: NotRequired[datetime],
```

## QueryExecutionContextTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import QueryExecutionContextTypeDef

def get_value() -> QueryExecutionContextTypeDef:
    return {
        "Database": ...,
    }
```

```python title="Definition"
class QueryExecutionContextTypeDef(TypedDict):
    Database: NotRequired[str],
    Catalog: NotRequired[str],
```

## QueryExecutionStatisticsTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import QueryExecutionStatisticsTypeDef

def get_value() -> QueryExecutionStatisticsTypeDef:
    return {
        "EngineExecutionTimeInMillis": ...,
    }
```

```python title="Definition"
class QueryExecutionStatisticsTypeDef(TypedDict):
    EngineExecutionTimeInMillis: NotRequired[int],
    DataScannedInBytes: NotRequired[int],
    DataManifestLocation: NotRequired[str],
    TotalExecutionTimeInMillis: NotRequired[int],
    QueryQueueTimeInMillis: NotRequired[int],
    QueryPlanningTimeInMillis: NotRequired[int],
    ServiceProcessingTimeInMillis: NotRequired[int],
```

## QueryExecutionStatusTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import QueryExecutionStatusTypeDef

def get_value() -> QueryExecutionStatusTypeDef:
    return {
        "State": ...,
    }
```

```python title="Definition"
class QueryExecutionStatusTypeDef(TypedDict):
    State: NotRequired[QueryExecutionStateType],  # (1)
    StateChangeReason: NotRequired[str],
    SubmissionDateTime: NotRequired[datetime],
    CompletionDateTime: NotRequired[datetime],
    AthenaError: NotRequired[AthenaErrorTypeDef],  # (2)
```

1. See [:material-code-brackets: QueryExecutionStateType](./literals.md#queryexecutionstatetype) 
2. See [:material-code-braces: AthenaErrorTypeDef](./type_defs.md#athenaerrortypedef) 
## QueryExecutionTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import QueryExecutionTypeDef

def get_value() -> QueryExecutionTypeDef:
    return {
        "QueryExecutionId": ...,
    }
```

```python title="Definition"
class QueryExecutionTypeDef(TypedDict):
    QueryExecutionId: NotRequired[str],
    Query: NotRequired[str],
    StatementType: NotRequired[StatementTypeType],  # (1)
    ResultConfiguration: NotRequired[ResultConfigurationTypeDef],  # (2)
    QueryExecutionContext: NotRequired[QueryExecutionContextTypeDef],  # (3)
    Status: NotRequired[QueryExecutionStatusTypeDef],  # (4)
    Statistics: NotRequired[QueryExecutionStatisticsTypeDef],  # (5)
    WorkGroup: NotRequired[str],
    EngineVersion: NotRequired[EngineVersionTypeDef],  # (6)
```

1. See [:material-code-brackets: StatementTypeType](./literals.md#statementtypetype) 
2. See [:material-code-braces: ResultConfigurationTypeDef](./type_defs.md#resultconfigurationtypedef) 
3. See [:material-code-braces: QueryExecutionContextTypeDef](./type_defs.md#queryexecutioncontexttypedef) 
4. See [:material-code-braces: QueryExecutionStatusTypeDef](./type_defs.md#queryexecutionstatustypedef) 
5. See [:material-code-braces: QueryExecutionStatisticsTypeDef](./type_defs.md#queryexecutionstatisticstypedef) 
6. See [:material-code-braces: EngineVersionTypeDef](./type_defs.md#engineversiontypedef) 
## ResponseMetadataTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ResponseMetadataTypeDef

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

## ResultConfigurationTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ResultConfigurationTypeDef

def get_value() -> ResultConfigurationTypeDef:
    return {
        "OutputLocation": ...,
    }
```

```python title="Definition"
class ResultConfigurationTypeDef(TypedDict):
    OutputLocation: NotRequired[str],
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (1)
    ExpectedBucketOwner: NotRequired[str],
    AclConfiguration: NotRequired[AclConfigurationTypeDef],  # (2)
```

1. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
2. See [:material-code-braces: AclConfigurationTypeDef](./type_defs.md#aclconfigurationtypedef) 
## ResultConfigurationUpdatesTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ResultConfigurationUpdatesTypeDef

def get_value() -> ResultConfigurationUpdatesTypeDef:
    return {
        "OutputLocation": ...,
    }
```

```python title="Definition"
class ResultConfigurationUpdatesTypeDef(TypedDict):
    OutputLocation: NotRequired[str],
    RemoveOutputLocation: NotRequired[bool],
    EncryptionConfiguration: NotRequired[EncryptionConfigurationTypeDef],  # (1)
    RemoveEncryptionConfiguration: NotRequired[bool],
    ExpectedBucketOwner: NotRequired[str],
    RemoveExpectedBucketOwner: NotRequired[bool],
    AclConfiguration: NotRequired[AclConfigurationTypeDef],  # (2)
    RemoveAclConfiguration: NotRequired[bool],
```

1. See [:material-code-braces: EncryptionConfigurationTypeDef](./type_defs.md#encryptionconfigurationtypedef) 
2. See [:material-code-braces: AclConfigurationTypeDef](./type_defs.md#aclconfigurationtypedef) 
## ResultSetMetadataTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ResultSetMetadataTypeDef

def get_value() -> ResultSetMetadataTypeDef:
    return {
        "ColumnInfo": ...,
    }
```

```python title="Definition"
class ResultSetMetadataTypeDef(TypedDict):
    ColumnInfo: NotRequired[List[ColumnInfoTypeDef]],  # (1)
```

1. See [:material-code-braces: ColumnInfoTypeDef](./type_defs.md#columninfotypedef) 
## ResultSetTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import ResultSetTypeDef

def get_value() -> ResultSetTypeDef:
    return {
        "Rows": ...,
    }
```

```python title="Definition"
class ResultSetTypeDef(TypedDict):
    Rows: NotRequired[List[RowTypeDef]],  # (1)
    ResultSetMetadata: NotRequired[ResultSetMetadataTypeDef],  # (2)
```

1. See [:material-code-braces: RowTypeDef](./type_defs.md#rowtypedef) 
2. See [:material-code-braces: ResultSetMetadataTypeDef](./type_defs.md#resultsetmetadatatypedef) 
## RowTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import RowTypeDef

def get_value() -> RowTypeDef:
    return {
        "Data": ...,
    }
```

```python title="Definition"
class RowTypeDef(TypedDict):
    Data: NotRequired[List[DatumTypeDef]],  # (1)
```

1. See [:material-code-braces: DatumTypeDef](./type_defs.md#datumtypedef) 
## StartQueryExecutionInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import StartQueryExecutionInputRequestTypeDef

def get_value() -> StartQueryExecutionInputRequestTypeDef:
    return {
        "QueryString": ...,
    }
```

```python title="Definition"
class StartQueryExecutionInputRequestTypeDef(TypedDict):
    QueryString: str,
    ClientRequestToken: NotRequired[str],
    QueryExecutionContext: NotRequired[QueryExecutionContextTypeDef],  # (1)
    ResultConfiguration: NotRequired[ResultConfigurationTypeDef],  # (2)
    WorkGroup: NotRequired[str],
```

1. See [:material-code-braces: QueryExecutionContextTypeDef](./type_defs.md#queryexecutioncontexttypedef) 
2. See [:material-code-braces: ResultConfigurationTypeDef](./type_defs.md#resultconfigurationtypedef) 
## StartQueryExecutionOutputTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import StartQueryExecutionOutputTypeDef

def get_value() -> StartQueryExecutionOutputTypeDef:
    return {
        "QueryExecutionId": ...,
        "ResponseMetadata": ...,
    }
```

```python title="Definition"
class StartQueryExecutionOutputTypeDef(TypedDict):
    QueryExecutionId: str,
    ResponseMetadata: ResponseMetadataTypeDef,  # (1)
```

1. See [:material-code-braces: ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef) 
## StopQueryExecutionInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import StopQueryExecutionInputRequestTypeDef

def get_value() -> StopQueryExecutionInputRequestTypeDef:
    return {
        "QueryExecutionId": ...,
    }
```

```python title="Definition"
class StopQueryExecutionInputRequestTypeDef(TypedDict):
    QueryExecutionId: str,
```

## TableMetadataTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import TableMetadataTypeDef

def get_value() -> TableMetadataTypeDef:
    return {
        "Name": ...,
    }
```

```python title="Definition"
class TableMetadataTypeDef(TypedDict):
    Name: str,
    CreateTime: NotRequired[datetime],
    LastAccessTime: NotRequired[datetime],
    TableType: NotRequired[str],
    Columns: NotRequired[List[ColumnTypeDef]],  # (1)
    PartitionKeys: NotRequired[List[ColumnTypeDef]],  # (1)
    Parameters: NotRequired[Dict[str, str]],
```

1. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) 
2. See [:material-code-braces: ColumnTypeDef](./type_defs.md#columntypedef) 
## TagResourceInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import TagResourceInputRequestTypeDef

def get_value() -> TagResourceInputRequestTypeDef:
    return {
        "ResourceARN": ...,
        "Tags": ...,
    }
```

```python title="Definition"
class TagResourceInputRequestTypeDef(TypedDict):
    ResourceARN: str,
    Tags: Sequence[TagTypeDef],  # (1)
```

1. See [:material-code-braces: TagTypeDef](./type_defs.md#tagtypedef) 
## TagTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import TagTypeDef

def get_value() -> TagTypeDef:
    return {
        "Key": ...,
    }
```

```python title="Definition"
class TagTypeDef(TypedDict):
    Key: NotRequired[str],
    Value: NotRequired[str],
```

## UnprocessedNamedQueryIdTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import UnprocessedNamedQueryIdTypeDef

def get_value() -> UnprocessedNamedQueryIdTypeDef:
    return {
        "NamedQueryId": ...,
    }
```

```python title="Definition"
class UnprocessedNamedQueryIdTypeDef(TypedDict):
    NamedQueryId: NotRequired[str],
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## UnprocessedQueryExecutionIdTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import UnprocessedQueryExecutionIdTypeDef

def get_value() -> UnprocessedQueryExecutionIdTypeDef:
    return {
        "QueryExecutionId": ...,
    }
```

```python title="Definition"
class UnprocessedQueryExecutionIdTypeDef(TypedDict):
    QueryExecutionId: NotRequired[str],
    ErrorCode: NotRequired[str],
    ErrorMessage: NotRequired[str],
```

## UntagResourceInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import UntagResourceInputRequestTypeDef

def get_value() -> UntagResourceInputRequestTypeDef:
    return {
        "ResourceARN": ...,
        "TagKeys": ...,
    }
```

```python title="Definition"
class UntagResourceInputRequestTypeDef(TypedDict):
    ResourceARN: str,
    TagKeys: Sequence[str],
```

## UpdateDataCatalogInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import UpdateDataCatalogInputRequestTypeDef

def get_value() -> UpdateDataCatalogInputRequestTypeDef:
    return {
        "Name": ...,
        "Type": ...,
    }
```

```python title="Definition"
class UpdateDataCatalogInputRequestTypeDef(TypedDict):
    Name: str,
    Type: DataCatalogTypeType,  # (1)
    Description: NotRequired[str],
    Parameters: NotRequired[Mapping[str, str]],
```

1. See [:material-code-brackets: DataCatalogTypeType](./literals.md#datacatalogtypetype) 
## UpdateNamedQueryInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import UpdateNamedQueryInputRequestTypeDef

def get_value() -> UpdateNamedQueryInputRequestTypeDef:
    return {
        "NamedQueryId": ...,
        "Name": ...,
        "QueryString": ...,
    }
```

```python title="Definition"
class UpdateNamedQueryInputRequestTypeDef(TypedDict):
    NamedQueryId: str,
    Name: str,
    QueryString: str,
    Description: NotRequired[str],
```

## UpdatePreparedStatementInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import UpdatePreparedStatementInputRequestTypeDef

def get_value() -> UpdatePreparedStatementInputRequestTypeDef:
    return {
        "StatementName": ...,
        "WorkGroup": ...,
        "QueryStatement": ...,
    }
```

```python title="Definition"
class UpdatePreparedStatementInputRequestTypeDef(TypedDict):
    StatementName: str,
    WorkGroup: str,
    QueryStatement: str,
    Description: NotRequired[str],
```

## UpdateWorkGroupInputRequestTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import UpdateWorkGroupInputRequestTypeDef

def get_value() -> UpdateWorkGroupInputRequestTypeDef:
    return {
        "WorkGroup": ...,
    }
```

```python title="Definition"
class UpdateWorkGroupInputRequestTypeDef(TypedDict):
    WorkGroup: str,
    Description: NotRequired[str],
    ConfigurationUpdates: NotRequired[WorkGroupConfigurationUpdatesTypeDef],  # (1)
    State: NotRequired[WorkGroupStateType],  # (2)
```

1. See [:material-code-braces: WorkGroupConfigurationUpdatesTypeDef](./type_defs.md#workgroupconfigurationupdatestypedef) 
2. See [:material-code-brackets: WorkGroupStateType](./literals.md#workgroupstatetype) 
## WorkGroupConfigurationTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import WorkGroupConfigurationTypeDef

def get_value() -> WorkGroupConfigurationTypeDef:
    return {
        "ResultConfiguration": ...,
    }
```

```python title="Definition"
class WorkGroupConfigurationTypeDef(TypedDict):
    ResultConfiguration: NotRequired[ResultConfigurationTypeDef],  # (1)
    EnforceWorkGroupConfiguration: NotRequired[bool],
    PublishCloudWatchMetricsEnabled: NotRequired[bool],
    BytesScannedCutoffPerQuery: NotRequired[int],
    RequesterPaysEnabled: NotRequired[bool],
    EngineVersion: NotRequired[EngineVersionTypeDef],  # (2)
```

1. See [:material-code-braces: ResultConfigurationTypeDef](./type_defs.md#resultconfigurationtypedef) 
2. See [:material-code-braces: EngineVersionTypeDef](./type_defs.md#engineversiontypedef) 
## WorkGroupConfigurationUpdatesTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import WorkGroupConfigurationUpdatesTypeDef

def get_value() -> WorkGroupConfigurationUpdatesTypeDef:
    return {
        "EnforceWorkGroupConfiguration": ...,
    }
```

```python title="Definition"
class WorkGroupConfigurationUpdatesTypeDef(TypedDict):
    EnforceWorkGroupConfiguration: NotRequired[bool],
    ResultConfigurationUpdates: NotRequired[ResultConfigurationUpdatesTypeDef],  # (1)
    PublishCloudWatchMetricsEnabled: NotRequired[bool],
    BytesScannedCutoffPerQuery: NotRequired[int],
    RemoveBytesScannedCutoffPerQuery: NotRequired[bool],
    RequesterPaysEnabled: NotRequired[bool],
    EngineVersion: NotRequired[EngineVersionTypeDef],  # (2)
```

1. See [:material-code-braces: ResultConfigurationUpdatesTypeDef](./type_defs.md#resultconfigurationupdatestypedef) 
2. See [:material-code-braces: EngineVersionTypeDef](./type_defs.md#engineversiontypedef) 
## WorkGroupSummaryTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import WorkGroupSummaryTypeDef

def get_value() -> WorkGroupSummaryTypeDef:
    return {
        "Name": ...,
    }
```

```python title="Definition"
class WorkGroupSummaryTypeDef(TypedDict):
    Name: NotRequired[str],
    State: NotRequired[WorkGroupStateType],  # (1)
    Description: NotRequired[str],
    CreationTime: NotRequired[datetime],
    EngineVersion: NotRequired[EngineVersionTypeDef],  # (2)
```

1. See [:material-code-brackets: WorkGroupStateType](./literals.md#workgroupstatetype) 
2. See [:material-code-braces: EngineVersionTypeDef](./type_defs.md#engineversiontypedef) 
## WorkGroupTypeDef

```python title="Usage Example"
from mypy_boto3_athena.type_defs import WorkGroupTypeDef

def get_value() -> WorkGroupTypeDef:
    return {
        "Name": ...,
    }
```

```python title="Definition"
class WorkGroupTypeDef(TypedDict):
    Name: str,
    State: NotRequired[WorkGroupStateType],  # (1)
    Configuration: NotRequired[WorkGroupConfigurationTypeDef],  # (2)
    Description: NotRequired[str],
    CreationTime: NotRequired[datetime],
```

1. See [:material-code-brackets: WorkGroupStateType](./literals.md#workgroupstatetype) 
2. See [:material-code-braces: WorkGroupConfigurationTypeDef](./type_defs.md#workgroupconfigurationtypedef) 
