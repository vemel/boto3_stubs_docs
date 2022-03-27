# Paginators

> [Index](../README.md) > [LexModelBuildingService](./README.md) > Paginators

!!! note ""

    Auto-generated documentation for [LexModelBuildingService](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService)
    type annotations stubs module [mypy-boto3-lex-models](https://pypi.org/project/mypy-boto3-lex-models/).

## GetBotAliasesPaginator

Type annotations and code completion for `#!python boto3.client("lex-models").get_paginator("get_bot_aliases")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotAliases)

```python title="Usage example"
from boto3.session import Session

from mypy_boto3_lex_models.paginator import GetBotAliasesPaginator

def get_get_bot_aliases_paginator() -> GetBotAliasesPaginator:
    return Session().client("lex-models").get_paginator("get_bot_aliases")
```


### paginate

Type annotations and code completion for `#!python GetBotAliasesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    botName: str,
    nameContains: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> _PageIterator[GetBotAliasesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetBotAliasesResponseTypeDef](./type_defs.md#getbotaliasesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetBotAliasesRequestGetBotAliasesPaginateTypeDef = {  # (1)
    "botName": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetBotAliasesRequestGetBotAliasesPaginateTypeDef](./type_defs.md#getbotaliasesrequestgetbotaliasespaginatetypedef) 
## GetBotChannelAssociationsPaginator

Type annotations and code completion for `#!python boto3.client("lex-models").get_paginator("get_bot_channel_associations")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotChannelAssociations)

```python title="Usage example"
from boto3.session import Session

from mypy_boto3_lex_models.paginator import GetBotChannelAssociationsPaginator

def get_get_bot_channel_associations_paginator() -> GetBotChannelAssociationsPaginator:
    return Session().client("lex-models").get_paginator("get_bot_channel_associations")
```


### paginate

Type annotations and code completion for `#!python GetBotChannelAssociationsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    botName: str,
    botAlias: str,
    nameContains: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> _PageIterator[GetBotChannelAssociationsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetBotChannelAssociationsResponseTypeDef](./type_defs.md#getbotchannelassociationsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef = {  # (1)
    "botName": ...,
    "botAlias": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetBotChannelAssociationsRequestGetBotChannelAssociationsPaginateTypeDef](./type_defs.md#getbotchannelassociationsrequestgetbotchannelassociationspaginatetypedef) 
## GetBotVersionsPaginator

Type annotations and code completion for `#!python boto3.client("lex-models").get_paginator("get_bot_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBotVersions)

```python title="Usage example"
from boto3.session import Session

from mypy_boto3_lex_models.paginator import GetBotVersionsPaginator

def get_get_bot_versions_paginator() -> GetBotVersionsPaginator:
    return Session().client("lex-models").get_paginator("get_bot_versions")
```


### paginate

Type annotations and code completion for `#!python GetBotVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> _PageIterator[GetBotVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetBotVersionsResponseTypeDef](./type_defs.md#getbotversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetBotVersionsRequestGetBotVersionsPaginateTypeDef = {  # (1)
    "name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetBotVersionsRequestGetBotVersionsPaginateTypeDef](./type_defs.md#getbotversionsrequestgetbotversionspaginatetypedef) 
## GetBotsPaginator

Type annotations and code completion for `#!python boto3.client("lex-models").get_paginator("get_bots")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBots)

```python title="Usage example"
from boto3.session import Session

from mypy_boto3_lex_models.paginator import GetBotsPaginator

def get_get_bots_paginator() -> GetBotsPaginator:
    return Session().client("lex-models").get_paginator("get_bots")
```


### paginate

Type annotations and code completion for `#!python GetBotsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    nameContains: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> _PageIterator[GetBotsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetBotsResponseTypeDef](./type_defs.md#getbotsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetBotsRequestGetBotsPaginateTypeDef = {  # (1)
    "nameContains": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetBotsRequestGetBotsPaginateTypeDef](./type_defs.md#getbotsrequestgetbotspaginatetypedef) 
## GetBuiltinIntentsPaginator

Type annotations and code completion for `#!python boto3.client("lex-models").get_paginator("get_builtin_intents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinIntents)

```python title="Usage example"
from boto3.session import Session

from mypy_boto3_lex_models.paginator import GetBuiltinIntentsPaginator

def get_get_builtin_intents_paginator() -> GetBuiltinIntentsPaginator:
    return Session().client("lex-models").get_paginator("get_builtin_intents")
```


### paginate

Type annotations and code completion for `#!python GetBuiltinIntentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    locale: LocaleType = ...,  # (1)
    signatureContains: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> _PageIterator[GetBuiltinIntentsResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetBuiltinIntentsResponseTypeDef](./type_defs.md#getbuiltinintentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef = {  # (1)
    "locale": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetBuiltinIntentsRequestGetBuiltinIntentsPaginateTypeDef](./type_defs.md#getbuiltinintentsrequestgetbuiltinintentspaginatetypedef) 
## GetBuiltinSlotTypesPaginator

Type annotations and code completion for `#!python boto3.client("lex-models").get_paginator("get_builtin_slot_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetBuiltinSlotTypes)

```python title="Usage example"
from boto3.session import Session

from mypy_boto3_lex_models.paginator import GetBuiltinSlotTypesPaginator

def get_get_builtin_slot_types_paginator() -> GetBuiltinSlotTypesPaginator:
    return Session().client("lex-models").get_paginator("get_builtin_slot_types")
```


### paginate

Type annotations and code completion for `#!python GetBuiltinSlotTypesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    locale: LocaleType = ...,  # (1)
    signatureContains: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (2)
) -> _PageIterator[GetBuiltinSlotTypesResponseTypeDef]:  # (3)
    ...
```

1. See [:material-code-brackets: LocaleType](./literals.md#localetype) 
2. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
3. See [:material-code-braces: GetBuiltinSlotTypesResponseTypeDef](./type_defs.md#getbuiltinslottypesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef = {  # (1)
    "locale": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetBuiltinSlotTypesRequestGetBuiltinSlotTypesPaginateTypeDef](./type_defs.md#getbuiltinslottypesrequestgetbuiltinslottypespaginatetypedef) 
## GetIntentVersionsPaginator

Type annotations and code completion for `#!python boto3.client("lex-models").get_paginator("get_intent_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntentVersions)

```python title="Usage example"
from boto3.session import Session

from mypy_boto3_lex_models.paginator import GetIntentVersionsPaginator

def get_get_intent_versions_paginator() -> GetIntentVersionsPaginator:
    return Session().client("lex-models").get_paginator("get_intent_versions")
```


### paginate

Type annotations and code completion for `#!python GetIntentVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> _PageIterator[GetIntentVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetIntentVersionsResponseTypeDef](./type_defs.md#getintentversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef = {  # (1)
    "name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetIntentVersionsRequestGetIntentVersionsPaginateTypeDef](./type_defs.md#getintentversionsrequestgetintentversionspaginatetypedef) 
## GetIntentsPaginator

Type annotations and code completion for `#!python boto3.client("lex-models").get_paginator("get_intents")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetIntents)

```python title="Usage example"
from boto3.session import Session

from mypy_boto3_lex_models.paginator import GetIntentsPaginator

def get_get_intents_paginator() -> GetIntentsPaginator:
    return Session().client("lex-models").get_paginator("get_intents")
```


### paginate

Type annotations and code completion for `#!python GetIntentsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    nameContains: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> _PageIterator[GetIntentsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetIntentsResponseTypeDef](./type_defs.md#getintentsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetIntentsRequestGetIntentsPaginateTypeDef = {  # (1)
    "nameContains": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetIntentsRequestGetIntentsPaginateTypeDef](./type_defs.md#getintentsrequestgetintentspaginatetypedef) 
## GetSlotTypeVersionsPaginator

Type annotations and code completion for `#!python boto3.client("lex-models").get_paginator("get_slot_type_versions")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypeVersions)

```python title="Usage example"
from boto3.session import Session

from mypy_boto3_lex_models.paginator import GetSlotTypeVersionsPaginator

def get_get_slot_type_versions_paginator() -> GetSlotTypeVersionsPaginator:
    return Session().client("lex-models").get_paginator("get_slot_type_versions")
```


### paginate

Type annotations and code completion for `#!python GetSlotTypeVersionsPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    name: str,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> _PageIterator[GetSlotTypeVersionsResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetSlotTypeVersionsResponseTypeDef](./type_defs.md#getslottypeversionsresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef = {  # (1)
    "name": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetSlotTypeVersionsRequestGetSlotTypeVersionsPaginateTypeDef](./type_defs.md#getslottypeversionsrequestgetslottypeversionspaginatetypedef) 
## GetSlotTypesPaginator

Type annotations and code completion for `#!python boto3.client("lex-models").get_paginator("get_slot_types")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/lex-models.html#LexModelBuildingService.Paginator.GetSlotTypes)

```python title="Usage example"
from boto3.session import Session

from mypy_boto3_lex_models.paginator import GetSlotTypesPaginator

def get_get_slot_types_paginator() -> GetSlotTypesPaginator:
    return Session().client("lex-models").get_paginator("get_slot_types")
```


### paginate

Type annotations and code completion for `#!python GetSlotTypesPaginator.paginate` method.

```python title="Method definition"
def paginate(
    self,
    *,
    nameContains: str = ...,
    PaginationConfig: PaginatorConfigTypeDef = ...,  # (1)
) -> _PageIterator[GetSlotTypesResponseTypeDef]:  # (2)
    ...
```

1. See [:material-code-braces: PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef) 
2. See [:material-code-braces: GetSlotTypesResponseTypeDef](./type_defs.md#getslottypesresponsetypedef) 


```python title="Usage example with kwargs"
kwargs: GetSlotTypesRequestGetSlotTypesPaginateTypeDef = {  # (1)
    "nameContains": ...,
}

parent.paginate(**kwargs)
```

1. See [:material-code-braces: GetSlotTypesRequestGetSlotTypesPaginateTypeDef](./type_defs.md#getslottypesrequestgetslottypespaginatetypedef) 
