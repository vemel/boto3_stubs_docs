# Structures for boto3 QLDBSession module

> [Index](../index.md) > [QLDBSession](./index.md) > Structures

Auto-generated documentation for [QLDBSession](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/qldb-session.html#QLDBSession)
type annotations stubs module [mypy_boto3_qldb_session](https://pypi.org/project/mypy-boto3-qldb-session/).

- [Structures for boto3 QLDBSession module](#structures-for-boto3-qldbsession-module)
  - [AbortTransactionResultTypeDef](#aborttransactionresulttypedef)
  - [CommitTransactionRequestTypeDef](#committransactionrequesttypedef)
  - [CommitTransactionResultTypeDef](#committransactionresulttypedef)
  - [EndSessionResultTypeDef](#endsessionresulttypedef)
  - [ExecuteStatementRequestTypeDef](#executestatementrequesttypedef)
  - [ExecuteStatementResultTypeDef](#executestatementresulttypedef)
  - [FetchPageRequestTypeDef](#fetchpagerequesttypedef)
  - [FetchPageResultTypeDef](#fetchpageresulttypedef)
  - [IOUsageTypeDef](#iousagetypedef)
  - [PageTypeDef](#pagetypedef)
  - [SendCommandResultTypeDef](#sendcommandresulttypedef)
  - [StartSessionRequestTypeDef](#startsessionrequesttypedef)
  - [StartSessionResultTypeDef](#startsessionresulttypedef)
  - [StartTransactionResultTypeDef](#starttransactionresulttypedef)
  - [TimingInformationTypeDef](#timinginformationtypedef)
  - [ValueHolderTypeDef](#valueholdertypedef)

## AbortTransactionResultTypeDef

```python
from mypy_boto3_qldb_session.type_defs import AbortTransactionResultTypeDef
```




Optional fields:
- `TimingInformation`: `"TimingInformationTypeDef"`


## CommitTransactionRequestTypeDef

```python
from mypy_boto3_qldb_session.type_defs import CommitTransactionRequestTypeDef
```


Required fields:
- `TransactionId`: `str`
- `CommitDigest`: `Union[bytes, IO[bytes]]`




## CommitTransactionResultTypeDef

```python
from mypy_boto3_qldb_session.type_defs import CommitTransactionResultTypeDef
```




Optional fields:
- `TransactionId`: `str`
- `CommitDigest`: `Union[bytes, IO[bytes]]`
- `TimingInformation`: `"TimingInformationTypeDef"`
- `ConsumedIOs`: `"IOUsageTypeDef"`


## EndSessionResultTypeDef

```python
from mypy_boto3_qldb_session.type_defs import EndSessionResultTypeDef
```




Optional fields:
- `TimingInformation`: `"TimingInformationTypeDef"`


## ExecuteStatementRequestTypeDef

```python
from mypy_boto3_qldb_session.type_defs import ExecuteStatementRequestTypeDef
```


Required fields:
- `TransactionId`: `str`
- `Statement`: `str`



Optional fields:
- `Parameters`: `List["ValueHolderTypeDef"]`


## ExecuteStatementResultTypeDef

```python
from mypy_boto3_qldb_session.type_defs import ExecuteStatementResultTypeDef
```




Optional fields:
- `FirstPage`: `"PageTypeDef"`
- `TimingInformation`: `"TimingInformationTypeDef"`
- `ConsumedIOs`: `"IOUsageTypeDef"`


## FetchPageRequestTypeDef

```python
from mypy_boto3_qldb_session.type_defs import FetchPageRequestTypeDef
```


Required fields:
- `TransactionId`: `str`
- `NextPageToken`: `str`




## FetchPageResultTypeDef

```python
from mypy_boto3_qldb_session.type_defs import FetchPageResultTypeDef
```




Optional fields:
- `Page`: `"PageTypeDef"`
- `TimingInformation`: `"TimingInformationTypeDef"`
- `ConsumedIOs`: `"IOUsageTypeDef"`


## IOUsageTypeDef

```python
from mypy_boto3_qldb_session.type_defs import IOUsageTypeDef
```




Optional fields:
- `ReadIOs`: `int`
- `WriteIOs`: `int`


## PageTypeDef

```python
from mypy_boto3_qldb_session.type_defs import PageTypeDef
```




Optional fields:
- `Values`: `List["ValueHolderTypeDef"]`
- `NextPageToken`: `str`


## SendCommandResultTypeDef

```python
from mypy_boto3_qldb_session.type_defs import SendCommandResultTypeDef
```




Optional fields:
- `StartSession`: `"StartSessionResultTypeDef"`
- `StartTransaction`: `"StartTransactionResultTypeDef"`
- `EndSession`: `"EndSessionResultTypeDef"`
- `CommitTransaction`: `"CommitTransactionResultTypeDef"`
- `AbortTransaction`: `"AbortTransactionResultTypeDef"`
- `ExecuteStatement`: `"ExecuteStatementResultTypeDef"`
- `FetchPage`: `"FetchPageResultTypeDef"`


## StartSessionRequestTypeDef

```python
from mypy_boto3_qldb_session.type_defs import StartSessionRequestTypeDef
```


Required fields:
- `LedgerName`: `str`




## StartSessionResultTypeDef

```python
from mypy_boto3_qldb_session.type_defs import StartSessionResultTypeDef
```




Optional fields:
- `SessionToken`: `str`
- `TimingInformation`: `"TimingInformationTypeDef"`


## StartTransactionResultTypeDef

```python
from mypy_boto3_qldb_session.type_defs import StartTransactionResultTypeDef
```




Optional fields:
- `TransactionId`: `str`
- `TimingInformation`: `"TimingInformationTypeDef"`


## TimingInformationTypeDef

```python
from mypy_boto3_qldb_session.type_defs import TimingInformationTypeDef
```




Optional fields:
- `ProcessingTimeMilliseconds`: `int`


## ValueHolderTypeDef

```python
from mypy_boto3_qldb_session.type_defs import ValueHolderTypeDef
```




Optional fields:
- `IonBinary`: `Union[bytes, IO[bytes]]`
- `IonText`: `str`

