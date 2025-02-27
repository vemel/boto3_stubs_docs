#  CodeStarconnections module

> [Index](../README.md) > CodeStarconnections

!!! note ""

    Auto-generated documentation for [CodeStarconnections](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections)
    type annotations stubs module [mypy-boto3-codestar-connections](https://pypi.org/project/mypy-boto3-codestar-connections/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `CodeStarconnections`.

### From PyPI with pip

Install `boto3-stubs` for `CodeStarconnections` service.

```bash
# install with boto3 type annotations
python -m pip install 'boto3-stubs[codestar-connections]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'boto3-stubs-lite[codestar-connections]'


# standalone installation
python -m pip install mypy-boto3-codestar-connections
```



## How to uninstall

```bash
python -m pip uninstall -y mypy-boto3-codestar-connections
```

## Usage

Code samples can be found in [Examples](./usage.md).

## CodeStarconnectionsClient

Type annotations and code completion for  `#!python boto3.client("codestar-connections")` as [CodeStarconnectionsClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/codestar-connections.html#CodeStarconnections.Client)

```python title="Usage example"
from boto3.session import Session

from mypy_boto3_codestar_connections.client import CodeStarconnectionsClient

def get_client() -> CodeStarconnectionsClient:
    return Session().cleint("codestar-connections")
```









## Literals

Type annotations for [literals](./literals.md) used in methods and schemas.

```python title="Usage example"
from mypy_boto3_codestar_connections.literals import ConnectionStatusType

def get_value() -> ConnectionStatusType:
    return "AVAILABLE"
```

- [ConnectionStatusType](./literals.md#connectionstatustype)
- [ProviderTypeType](./literals.md#providertypetype)
- [CodeStarconnectionsServiceName](./literals.md#codestarconnectionsservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from mypy_boto3_codestar_connections.type_defs import ConnectionTypeDef

def get_value() -> ConnectionTypeDef:
    return {
        "ConnectionName": ...,
    }
```

- [ConnectionTypeDef](./type_defs.md#connectiontypedef)
- [CreateConnectionInputRequestTypeDef](./type_defs.md#createconnectioninputrequesttypedef)
- [CreateConnectionOutputTypeDef](./type_defs.md#createconnectionoutputtypedef)
- [CreateHostInputRequestTypeDef](./type_defs.md#createhostinputrequesttypedef)
- [CreateHostOutputTypeDef](./type_defs.md#createhostoutputtypedef)
- [DeleteConnectionInputRequestTypeDef](./type_defs.md#deleteconnectioninputrequesttypedef)
- [DeleteHostInputRequestTypeDef](./type_defs.md#deletehostinputrequesttypedef)
- [GetConnectionInputRequestTypeDef](./type_defs.md#getconnectioninputrequesttypedef)
- [GetConnectionOutputTypeDef](./type_defs.md#getconnectionoutputtypedef)
- [GetHostInputRequestTypeDef](./type_defs.md#gethostinputrequesttypedef)
- [GetHostOutputTypeDef](./type_defs.md#gethostoutputtypedef)
- [HostTypeDef](./type_defs.md#hosttypedef)
- [ListConnectionsInputRequestTypeDef](./type_defs.md#listconnectionsinputrequesttypedef)
- [ListConnectionsOutputTypeDef](./type_defs.md#listconnectionsoutputtypedef)
- [ListHostsInputRequestTypeDef](./type_defs.md#listhostsinputrequesttypedef)
- [ListHostsOutputTypeDef](./type_defs.md#listhostsoutputtypedef)
- [ListTagsForResourceInputRequestTypeDef](./type_defs.md#listtagsforresourceinputrequesttypedef)
- [ListTagsForResourceOutputTypeDef](./type_defs.md#listtagsforresourceoutputtypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [TagResourceInputRequestTypeDef](./type_defs.md#tagresourceinputrequesttypedef)
- [TagTypeDef](./type_defs.md#tagtypedef)
- [UntagResourceInputRequestTypeDef](./type_defs.md#untagresourceinputrequesttypedef)
- [UpdateHostInputRequestTypeDef](./type_defs.md#updatehostinputrequesttypedef)
- [VpcConfigurationTypeDef](./type_defs.md#vpcconfigurationtypedef)

