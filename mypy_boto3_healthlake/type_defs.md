# Structures for boto3 HealthLake module

> [Index](../index.md) > [HealthLake](./index.md) > Structures

Auto-generated documentation for [HealthLake](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/healthlake.html#HealthLake)
type annotations stubs module [mypy_boto3_healthlake](https://pypi.org/project/mypy-boto3-healthlake/).

- [Structures for boto3 HealthLake module](#structures-for-boto3-healthlake-module)
  - [CreateFHIRDatastoreResponseTypeDef](#createfhirdatastoreresponsetypedef)
  - [DatastoreFilterTypeDef](#datastorefiltertypedef)
  - [DatastorePropertiesTypeDef](#datastorepropertiestypedef)
  - [DeleteFHIRDatastoreResponseTypeDef](#deletefhirdatastoreresponsetypedef)
  - [DescribeFHIRDatastoreResponseTypeDef](#describefhirdatastoreresponsetypedef)
  - [DescribeFHIRExportJobResponseTypeDef](#describefhirexportjobresponsetypedef)
  - [DescribeFHIRImportJobResponseTypeDef](#describefhirimportjobresponsetypedef)
  - [ExportJobPropertiesTypeDef](#exportjobpropertiestypedef)
  - [ImportJobPropertiesTypeDef](#importjobpropertiestypedef)
  - [InputDataConfigTypeDef](#inputdataconfigtypedef)
  - [ListFHIRDatastoresResponseTypeDef](#listfhirdatastoresresponsetypedef)
  - [OutputDataConfigTypeDef](#outputdataconfigtypedef)
  - [PreloadDataConfigTypeDef](#preloaddataconfigtypedef)
  - [StartFHIRExportJobResponseTypeDef](#startfhirexportjobresponsetypedef)
  - [StartFHIRImportJobResponseTypeDef](#startfhirimportjobresponsetypedef)

## CreateFHIRDatastoreResponseTypeDef

```python
from mypy_boto3_healthlake.type_defs import CreateFHIRDatastoreResponseTypeDef
```


Required fields:
- `DatastoreId`: `str`
- `DatastoreArn`: `str`
- `DatastoreStatus`: `DatastoreStatus`
- `DatastoreEndpoint`: `str`




## DatastoreFilterTypeDef

```python
from mypy_boto3_healthlake.type_defs import DatastoreFilterTypeDef
```




Optional fields:
- `DatastoreName`: `str`
- `DatastoreStatus`: `DatastoreStatus`
- `CreatedBefore`: `datetime`
- `CreatedAfter`: `datetime`


## DatastorePropertiesTypeDef

```python
from mypy_boto3_healthlake.type_defs import DatastorePropertiesTypeDef
```


Required fields:
- `DatastoreId`: `str`
- `DatastoreArn`: `str`
- `DatastoreStatus`: `DatastoreStatus`
- `DatastoreTypeVersion`: `Literal['R4']`
- `DatastoreEndpoint`: `str`



Optional fields:
- `DatastoreName`: `str`
- `CreatedAt`: `datetime`
- `PreloadDataConfig`: `"PreloadDataConfigTypeDef"`


## DeleteFHIRDatastoreResponseTypeDef

```python
from mypy_boto3_healthlake.type_defs import DeleteFHIRDatastoreResponseTypeDef
```


Required fields:
- `DatastoreId`: `str`
- `DatastoreArn`: `str`
- `DatastoreStatus`: `DatastoreStatus`
- `DatastoreEndpoint`: `str`




## DescribeFHIRDatastoreResponseTypeDef

```python
from mypy_boto3_healthlake.type_defs import DescribeFHIRDatastoreResponseTypeDef
```


Required fields:
- `DatastoreProperties`: `"DatastorePropertiesTypeDef"`




## DescribeFHIRExportJobResponseTypeDef

```python
from mypy_boto3_healthlake.type_defs import DescribeFHIRExportJobResponseTypeDef
```


Required fields:
- `ExportJobProperties`: `"ExportJobPropertiesTypeDef"`




## DescribeFHIRImportJobResponseTypeDef

```python
from mypy_boto3_healthlake.type_defs import DescribeFHIRImportJobResponseTypeDef
```


Required fields:
- `ImportJobProperties`: `"ImportJobPropertiesTypeDef"`




## ExportJobPropertiesTypeDef

```python
from mypy_boto3_healthlake.type_defs import ExportJobPropertiesTypeDef
```


Required fields:
- `JobId`: `str`
- `JobStatus`: `JobStatus`
- `SubmitTime`: `datetime`
- `DatastoreId`: `str`
- `OutputDataConfig`: `"OutputDataConfigTypeDef"`



Optional fields:
- `JobName`: `str`
- `EndTime`: `datetime`
- `DataAccessRoleArn`: `str`
- `Message`: `str`


## ImportJobPropertiesTypeDef

```python
from mypy_boto3_healthlake.type_defs import ImportJobPropertiesTypeDef
```


Required fields:
- `JobId`: `str`
- `JobStatus`: `JobStatus`
- `SubmitTime`: `datetime`
- `DatastoreId`: `str`
- `InputDataConfig`: `"InputDataConfigTypeDef"`



Optional fields:
- `JobName`: `str`
- `EndTime`: `datetime`
- `DataAccessRoleArn`: `str`
- `Message`: `str`


## InputDataConfigTypeDef

```python
from mypy_boto3_healthlake.type_defs import InputDataConfigTypeDef
```




Optional fields:
- `S3Uri`: `str`


## ListFHIRDatastoresResponseTypeDef

```python
from mypy_boto3_healthlake.type_defs import ListFHIRDatastoresResponseTypeDef
```


Required fields:
- `DatastorePropertiesList`: `List["DatastorePropertiesTypeDef"]`



Optional fields:
- `NextToken`: `str`


## OutputDataConfigTypeDef

```python
from mypy_boto3_healthlake.type_defs import OutputDataConfigTypeDef
```




Optional fields:
- `S3Uri`: `str`


## PreloadDataConfigTypeDef

```python
from mypy_boto3_healthlake.type_defs import PreloadDataConfigTypeDef
```


Required fields:
- `PreloadDataType`: `Literal['SYNTHEA']`




## StartFHIRExportJobResponseTypeDef

```python
from mypy_boto3_healthlake.type_defs import StartFHIRExportJobResponseTypeDef
```


Required fields:
- `JobId`: `str`
- `JobStatus`: `JobStatus`



Optional fields:
- `DatastoreId`: `str`


## StartFHIRImportJobResponseTypeDef

```python
from mypy_boto3_healthlake.type_defs import StartFHIRImportJobResponseTypeDef
```


Required fields:
- `JobId`: `str`
- `JobStatus`: `JobStatus`



Optional fields:
- `DatastoreId`: `str`

