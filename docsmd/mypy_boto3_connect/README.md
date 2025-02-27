#  Connect module

> [Index](../README.md) > Connect

!!! note ""

    Auto-generated documentation for [Connect](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect)
    type annotations stubs module [mypy-boto3-connect](https://pypi.org/project/mypy-boto3-connect/).

## How to install

### VSCode extension

Add [AWS Boto3](https://marketplace.visualstudio.com/items?itemName=Boto3typed.boto3-ide)
extension to your VSCode and run `AWS boto3: Quick Start` command.

Click `Modify` and select `boto3 common` and `Connect`.

### From PyPI with pip

Install `boto3-stubs` for `Connect` service.

```bash
# install with boto3 type annotations
python -m pip install 'boto3-stubs[connect]'


# Lite version does not provide session.client/resource overloads
# it is more RAM-friendly, but requires explicit type annotations
python -m pip install 'boto3-stubs-lite[connect]'


# standalone installation
python -m pip install mypy-boto3-connect
```



## How to uninstall

```bash
python -m pip uninstall -y mypy-boto3-connect
```

## Usage

Code samples can be found in [Examples](./usage.md).

## ConnectClient

Type annotations and code completion for  `#!python boto3.client("connect")` as [ConnectClient](./client.md)
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/connect.html#Connect.Client)

```python title="Usage example"
from boto3.session import Session

from mypy_boto3_connect.client import ConnectClient

def get_client() -> ConnectClient:
    return Session().cleint("connect")
```


## Paginators

Type annotations and code completion for [paginators](./paginators.md)
from `#!python boto3.client("connect").get_paginator("...")`.

```python title="Usage example"
from boto3.session import Session

from mypy_boto3_connect.paginator import GetMetricDataPaginator

def get_get_metric_data_paginator() -> GetMetricDataPaginator:
    return Session().client("connect").get_paginator("get_metric_data"))
```

- [GetMetricDataPaginator](./paginators.md#getmetricdatapaginator)
- [ListAgentStatusesPaginator](./paginators.md#listagentstatusespaginator)
- [ListApprovedOriginsPaginator](./paginators.md#listapprovedoriginspaginator)
- [ListBotsPaginator](./paginators.md#listbotspaginator)
- [ListContactFlowModulesPaginator](./paginators.md#listcontactflowmodulespaginator)
- [ListContactFlowsPaginator](./paginators.md#listcontactflowspaginator)
- [ListContactReferencesPaginator](./paginators.md#listcontactreferencespaginator)
- [ListDefaultVocabulariesPaginator](./paginators.md#listdefaultvocabulariespaginator)
- [ListHoursOfOperationsPaginator](./paginators.md#listhoursofoperationspaginator)
- [ListInstanceAttributesPaginator](./paginators.md#listinstanceattributespaginator)
- [ListInstanceStorageConfigsPaginator](./paginators.md#listinstancestorageconfigspaginator)
- [ListInstancesPaginator](./paginators.md#listinstancespaginator)
- [ListIntegrationAssociationsPaginator](./paginators.md#listintegrationassociationspaginator)
- [ListLambdaFunctionsPaginator](./paginators.md#listlambdafunctionspaginator)
- [ListLexBotsPaginator](./paginators.md#listlexbotspaginator)
- [ListPhoneNumbersPaginator](./paginators.md#listphonenumberspaginator)
- [ListPromptsPaginator](./paginators.md#listpromptspaginator)
- [ListQueueQuickConnectsPaginator](./paginators.md#listqueuequickconnectspaginator)
- [ListQueuesPaginator](./paginators.md#listqueuespaginator)
- [ListQuickConnectsPaginator](./paginators.md#listquickconnectspaginator)
- [ListRoutingProfileQueuesPaginator](./paginators.md#listroutingprofilequeuespaginator)
- [ListRoutingProfilesPaginator](./paginators.md#listroutingprofilespaginator)
- [ListSecurityKeysPaginator](./paginators.md#listsecuritykeyspaginator)
- [ListSecurityProfilePermissionsPaginator](./paginators.md#listsecurityprofilepermissionspaginator)
- [ListSecurityProfilesPaginator](./paginators.md#listsecurityprofilespaginator)
- [ListUseCasesPaginator](./paginators.md#listusecasespaginator)
- [ListUserHierarchyGroupsPaginator](./paginators.md#listuserhierarchygroupspaginator)
- [ListUsersPaginator](./paginators.md#listuserspaginator)
- [SearchVocabulariesPaginator](./paginators.md#searchvocabulariespaginator)









## Literals

Type annotations for [literals](./literals.md) used in methods and schemas.

```python title="Usage example"
from mypy_boto3_connect.literals import AgentStatusStateType

def get_value() -> AgentStatusStateType:
    return "DISABLED"
```

- [AgentStatusStateType](./literals.md#agentstatusstatetype)
- [AgentStatusTypeType](./literals.md#agentstatustypetype)
- [ChannelType](./literals.md#channeltype)
- [ComparisonType](./literals.md#comparisontype)
- [ContactFlowModuleStateType](./literals.md#contactflowmodulestatetype)
- [ContactFlowModuleStatusType](./literals.md#contactflowmodulestatustype)
- [ContactFlowStateType](./literals.md#contactflowstatetype)
- [ContactFlowTypeType](./literals.md#contactflowtypetype)
- [ContactInitiationMethodType](./literals.md#contactinitiationmethodtype)
- [CurrentMetricNameType](./literals.md#currentmetricnametype)
- [DirectoryTypeType](./literals.md#directorytypetype)
- [EncryptionTypeType](./literals.md#encryptiontypetype)
- [GetMetricDataPaginatorName](./literals.md#getmetricdatapaginatorname)
- [GroupingType](./literals.md#groupingtype)
- [HistoricalMetricNameType](./literals.md#historicalmetricnametype)
- [HoursOfOperationDaysType](./literals.md#hoursofoperationdaystype)
- [InstanceAttributeTypeType](./literals.md#instanceattributetypetype)
- [InstanceStatusType](./literals.md#instancestatustype)
- [InstanceStorageResourceTypeType](./literals.md#instancestorageresourcetypetype)
- [IntegrationTypeType](./literals.md#integrationtypetype)
- [LexVersionType](./literals.md#lexversiontype)
- [ListAgentStatusesPaginatorName](./literals.md#listagentstatusespaginatorname)
- [ListApprovedOriginsPaginatorName](./literals.md#listapprovedoriginspaginatorname)
- [ListBotsPaginatorName](./literals.md#listbotspaginatorname)
- [ListContactFlowModulesPaginatorName](./literals.md#listcontactflowmodulespaginatorname)
- [ListContactFlowsPaginatorName](./literals.md#listcontactflowspaginatorname)
- [ListContactReferencesPaginatorName](./literals.md#listcontactreferencespaginatorname)
- [ListDefaultVocabulariesPaginatorName](./literals.md#listdefaultvocabulariespaginatorname)
- [ListHoursOfOperationsPaginatorName](./literals.md#listhoursofoperationspaginatorname)
- [ListInstanceAttributesPaginatorName](./literals.md#listinstanceattributespaginatorname)
- [ListInstanceStorageConfigsPaginatorName](./literals.md#listinstancestorageconfigspaginatorname)
- [ListInstancesPaginatorName](./literals.md#listinstancespaginatorname)
- [ListIntegrationAssociationsPaginatorName](./literals.md#listintegrationassociationspaginatorname)
- [ListLambdaFunctionsPaginatorName](./literals.md#listlambdafunctionspaginatorname)
- [ListLexBotsPaginatorName](./literals.md#listlexbotspaginatorname)
- [ListPhoneNumbersPaginatorName](./literals.md#listphonenumberspaginatorname)
- [ListPromptsPaginatorName](./literals.md#listpromptspaginatorname)
- [ListQueueQuickConnectsPaginatorName](./literals.md#listqueuequickconnectspaginatorname)
- [ListQueuesPaginatorName](./literals.md#listqueuespaginatorname)
- [ListQuickConnectsPaginatorName](./literals.md#listquickconnectspaginatorname)
- [ListRoutingProfileQueuesPaginatorName](./literals.md#listroutingprofilequeuespaginatorname)
- [ListRoutingProfilesPaginatorName](./literals.md#listroutingprofilespaginatorname)
- [ListSecurityKeysPaginatorName](./literals.md#listsecuritykeyspaginatorname)
- [ListSecurityProfilePermissionsPaginatorName](./literals.md#listsecurityprofilepermissionspaginatorname)
- [ListSecurityProfilesPaginatorName](./literals.md#listsecurityprofilespaginatorname)
- [ListUseCasesPaginatorName](./literals.md#listusecasespaginatorname)
- [ListUserHierarchyGroupsPaginatorName](./literals.md#listuserhierarchygroupspaginatorname)
- [ListUsersPaginatorName](./literals.md#listuserspaginatorname)
- [PhoneNumberCountryCodeType](./literals.md#phonenumbercountrycodetype)
- [PhoneNumberTypeType](./literals.md#phonenumbertypetype)
- [PhoneTypeType](./literals.md#phonetypetype)
- [QueueStatusType](./literals.md#queuestatustype)
- [QueueTypeType](./literals.md#queuetypetype)
- [QuickConnectTypeType](./literals.md#quickconnecttypetype)
- [ReferenceStatusType](./literals.md#referencestatustype)
- [ReferenceTypeType](./literals.md#referencetypetype)
- [SearchVocabulariesPaginatorName](./literals.md#searchvocabulariespaginatorname)
- [SourceTypeType](./literals.md#sourcetypetype)
- [StatisticType](./literals.md#statistictype)
- [StorageTypeType](./literals.md#storagetypetype)
- [TrafficTypeType](./literals.md#traffictypetype)
- [UnitType](./literals.md#unittype)
- [UseCaseTypeType](./literals.md#usecasetypetype)
- [VocabularyLanguageCodeType](./literals.md#vocabularylanguagecodetype)
- [VocabularyStateType](./literals.md#vocabularystatetype)
- [VoiceRecordingTrackType](./literals.md#voicerecordingtracktype)
- [ConnectServiceName](./literals.md#connectservicename)
- [ServiceName](./literals.md#servicename)
- [ResourceServiceName](./literals.md#resourceservicename)
- [PaginatorName](./literals.md#paginatorname)
- [RegionName](./literals.md#regionname)




## Typed dictionaries

Type annotations for [typed dictionaries](./type_defs.md) used in methods and schema.

```python title="Usage example"
from mypy_boto3_connect.type_defs import AgentInfoTypeDef

def get_value() -> AgentInfoTypeDef:
    return {
        "Id": ...,
    }
```

- [AgentInfoTypeDef](./type_defs.md#agentinfotypedef)
- [AgentStatusSummaryTypeDef](./type_defs.md#agentstatussummarytypedef)
- [AgentStatusTypeDef](./type_defs.md#agentstatustypedef)
- [AnswerMachineDetectionConfigTypeDef](./type_defs.md#answermachinedetectionconfigtypedef)
- [AssociateApprovedOriginRequestRequestTypeDef](./type_defs.md#associateapprovedoriginrequestrequesttypedef)
- [AssociateBotRequestRequestTypeDef](./type_defs.md#associatebotrequestrequesttypedef)
- [AssociateDefaultVocabularyRequestRequestTypeDef](./type_defs.md#associatedefaultvocabularyrequestrequesttypedef)
- [AssociateInstanceStorageConfigRequestRequestTypeDef](./type_defs.md#associateinstancestorageconfigrequestrequesttypedef)
- [AssociateInstanceStorageConfigResponseTypeDef](./type_defs.md#associateinstancestorageconfigresponsetypedef)
- [AssociateLambdaFunctionRequestRequestTypeDef](./type_defs.md#associatelambdafunctionrequestrequesttypedef)
- [AssociateLexBotRequestRequestTypeDef](./type_defs.md#associatelexbotrequestrequesttypedef)
- [AssociateQueueQuickConnectsRequestRequestTypeDef](./type_defs.md#associatequeuequickconnectsrequestrequesttypedef)
- [AssociateRoutingProfileQueuesRequestRequestTypeDef](./type_defs.md#associateroutingprofilequeuesrequestrequesttypedef)
- [AssociateSecurityKeyRequestRequestTypeDef](./type_defs.md#associatesecuritykeyrequestrequesttypedef)
- [AssociateSecurityKeyResponseTypeDef](./type_defs.md#associatesecuritykeyresponsetypedef)
- [AttachmentReferenceTypeDef](./type_defs.md#attachmentreferencetypedef)
- [AttributeTypeDef](./type_defs.md#attributetypedef)
- [ChatMessageTypeDef](./type_defs.md#chatmessagetypedef)
- [ChatStreamingConfigurationTypeDef](./type_defs.md#chatstreamingconfigurationtypedef)
- [ContactFlowModuleSummaryTypeDef](./type_defs.md#contactflowmodulesummarytypedef)
- [ContactFlowModuleTypeDef](./type_defs.md#contactflowmoduletypedef)
- [ContactFlowSummaryTypeDef](./type_defs.md#contactflowsummarytypedef)
- [ContactFlowTypeDef](./type_defs.md#contactflowtypedef)
- [ContactTypeDef](./type_defs.md#contacttypedef)
- [CreateAgentStatusRequestRequestTypeDef](./type_defs.md#createagentstatusrequestrequesttypedef)
- [CreateAgentStatusResponseTypeDef](./type_defs.md#createagentstatusresponsetypedef)
- [CreateContactFlowModuleRequestRequestTypeDef](./type_defs.md#createcontactflowmodulerequestrequesttypedef)
- [CreateContactFlowModuleResponseTypeDef](./type_defs.md#createcontactflowmoduleresponsetypedef)
- [CreateContactFlowRequestRequestTypeDef](./type_defs.md#createcontactflowrequestrequesttypedef)
- [CreateContactFlowResponseTypeDef](./type_defs.md#createcontactflowresponsetypedef)
- [CreateHoursOfOperationRequestRequestTypeDef](./type_defs.md#createhoursofoperationrequestrequesttypedef)
- [CreateHoursOfOperationResponseTypeDef](./type_defs.md#createhoursofoperationresponsetypedef)
- [CreateInstanceRequestRequestTypeDef](./type_defs.md#createinstancerequestrequesttypedef)
- [CreateInstanceResponseTypeDef](./type_defs.md#createinstanceresponsetypedef)
- [CreateIntegrationAssociationRequestRequestTypeDef](./type_defs.md#createintegrationassociationrequestrequesttypedef)
- [CreateIntegrationAssociationResponseTypeDef](./type_defs.md#createintegrationassociationresponsetypedef)
- [CreateQueueRequestRequestTypeDef](./type_defs.md#createqueuerequestrequesttypedef)
- [CreateQueueResponseTypeDef](./type_defs.md#createqueueresponsetypedef)
- [CreateQuickConnectRequestRequestTypeDef](./type_defs.md#createquickconnectrequestrequesttypedef)
- [CreateQuickConnectResponseTypeDef](./type_defs.md#createquickconnectresponsetypedef)
- [CreateRoutingProfileRequestRequestTypeDef](./type_defs.md#createroutingprofilerequestrequesttypedef)
- [CreateRoutingProfileResponseTypeDef](./type_defs.md#createroutingprofileresponsetypedef)
- [CreateSecurityProfileRequestRequestTypeDef](./type_defs.md#createsecurityprofilerequestrequesttypedef)
- [CreateSecurityProfileResponseTypeDef](./type_defs.md#createsecurityprofileresponsetypedef)
- [CreateUseCaseRequestRequestTypeDef](./type_defs.md#createusecaserequestrequesttypedef)
- [CreateUseCaseResponseTypeDef](./type_defs.md#createusecaseresponsetypedef)
- [CreateUserHierarchyGroupRequestRequestTypeDef](./type_defs.md#createuserhierarchygrouprequestrequesttypedef)
- [CreateUserHierarchyGroupResponseTypeDef](./type_defs.md#createuserhierarchygroupresponsetypedef)
- [CreateUserRequestRequestTypeDef](./type_defs.md#createuserrequestrequesttypedef)
- [CreateUserResponseTypeDef](./type_defs.md#createuserresponsetypedef)
- [CreateVocabularyRequestRequestTypeDef](./type_defs.md#createvocabularyrequestrequesttypedef)
- [CreateVocabularyResponseTypeDef](./type_defs.md#createvocabularyresponsetypedef)
- [CredentialsTypeDef](./type_defs.md#credentialstypedef)
- [CurrentMetricDataTypeDef](./type_defs.md#currentmetricdatatypedef)
- [CurrentMetricResultTypeDef](./type_defs.md#currentmetricresulttypedef)
- [CurrentMetricTypeDef](./type_defs.md#currentmetrictypedef)
- [DefaultVocabularyTypeDef](./type_defs.md#defaultvocabularytypedef)
- [DeleteContactFlowModuleRequestRequestTypeDef](./type_defs.md#deletecontactflowmodulerequestrequesttypedef)
- [DeleteContactFlowRequestRequestTypeDef](./type_defs.md#deletecontactflowrequestrequesttypedef)
- [DeleteHoursOfOperationRequestRequestTypeDef](./type_defs.md#deletehoursofoperationrequestrequesttypedef)
- [DeleteInstanceRequestRequestTypeDef](./type_defs.md#deleteinstancerequestrequesttypedef)
- [DeleteIntegrationAssociationRequestRequestTypeDef](./type_defs.md#deleteintegrationassociationrequestrequesttypedef)
- [DeleteQuickConnectRequestRequestTypeDef](./type_defs.md#deletequickconnectrequestrequesttypedef)
- [DeleteSecurityProfileRequestRequestTypeDef](./type_defs.md#deletesecurityprofilerequestrequesttypedef)
- [DeleteUseCaseRequestRequestTypeDef](./type_defs.md#deleteusecaserequestrequesttypedef)
- [DeleteUserHierarchyGroupRequestRequestTypeDef](./type_defs.md#deleteuserhierarchygrouprequestrequesttypedef)
- [DeleteUserRequestRequestTypeDef](./type_defs.md#deleteuserrequestrequesttypedef)
- [DeleteVocabularyRequestRequestTypeDef](./type_defs.md#deletevocabularyrequestrequesttypedef)
- [DeleteVocabularyResponseTypeDef](./type_defs.md#deletevocabularyresponsetypedef)
- [DescribeAgentStatusRequestRequestTypeDef](./type_defs.md#describeagentstatusrequestrequesttypedef)
- [DescribeAgentStatusResponseTypeDef](./type_defs.md#describeagentstatusresponsetypedef)
- [DescribeContactFlowModuleRequestRequestTypeDef](./type_defs.md#describecontactflowmodulerequestrequesttypedef)
- [DescribeContactFlowModuleResponseTypeDef](./type_defs.md#describecontactflowmoduleresponsetypedef)
- [DescribeContactFlowRequestRequestTypeDef](./type_defs.md#describecontactflowrequestrequesttypedef)
- [DescribeContactFlowResponseTypeDef](./type_defs.md#describecontactflowresponsetypedef)
- [DescribeContactRequestRequestTypeDef](./type_defs.md#describecontactrequestrequesttypedef)
- [DescribeContactResponseTypeDef](./type_defs.md#describecontactresponsetypedef)
- [DescribeHoursOfOperationRequestRequestTypeDef](./type_defs.md#describehoursofoperationrequestrequesttypedef)
- [DescribeHoursOfOperationResponseTypeDef](./type_defs.md#describehoursofoperationresponsetypedef)
- [DescribeInstanceAttributeRequestRequestTypeDef](./type_defs.md#describeinstanceattributerequestrequesttypedef)
- [DescribeInstanceAttributeResponseTypeDef](./type_defs.md#describeinstanceattributeresponsetypedef)
- [DescribeInstanceRequestRequestTypeDef](./type_defs.md#describeinstancerequestrequesttypedef)
- [DescribeInstanceResponseTypeDef](./type_defs.md#describeinstanceresponsetypedef)
- [DescribeInstanceStorageConfigRequestRequestTypeDef](./type_defs.md#describeinstancestorageconfigrequestrequesttypedef)
- [DescribeInstanceStorageConfigResponseTypeDef](./type_defs.md#describeinstancestorageconfigresponsetypedef)
- [DescribeQueueRequestRequestTypeDef](./type_defs.md#describequeuerequestrequesttypedef)
- [DescribeQueueResponseTypeDef](./type_defs.md#describequeueresponsetypedef)
- [DescribeQuickConnectRequestRequestTypeDef](./type_defs.md#describequickconnectrequestrequesttypedef)
- [DescribeQuickConnectResponseTypeDef](./type_defs.md#describequickconnectresponsetypedef)
- [DescribeRoutingProfileRequestRequestTypeDef](./type_defs.md#describeroutingprofilerequestrequesttypedef)
- [DescribeRoutingProfileResponseTypeDef](./type_defs.md#describeroutingprofileresponsetypedef)
- [DescribeSecurityProfileRequestRequestTypeDef](./type_defs.md#describesecurityprofilerequestrequesttypedef)
- [DescribeSecurityProfileResponseTypeDef](./type_defs.md#describesecurityprofileresponsetypedef)
- [DescribeUserHierarchyGroupRequestRequestTypeDef](./type_defs.md#describeuserhierarchygrouprequestrequesttypedef)
- [DescribeUserHierarchyGroupResponseTypeDef](./type_defs.md#describeuserhierarchygroupresponsetypedef)
- [DescribeUserHierarchyStructureRequestRequestTypeDef](./type_defs.md#describeuserhierarchystructurerequestrequesttypedef)
- [DescribeUserHierarchyStructureResponseTypeDef](./type_defs.md#describeuserhierarchystructureresponsetypedef)
- [DescribeUserRequestRequestTypeDef](./type_defs.md#describeuserrequestrequesttypedef)
- [DescribeUserResponseTypeDef](./type_defs.md#describeuserresponsetypedef)
- [DescribeVocabularyRequestRequestTypeDef](./type_defs.md#describevocabularyrequestrequesttypedef)
- [DescribeVocabularyResponseTypeDef](./type_defs.md#describevocabularyresponsetypedef)
- [DimensionsTypeDef](./type_defs.md#dimensionstypedef)
- [DisassociateApprovedOriginRequestRequestTypeDef](./type_defs.md#disassociateapprovedoriginrequestrequesttypedef)
- [DisassociateBotRequestRequestTypeDef](./type_defs.md#disassociatebotrequestrequesttypedef)
- [DisassociateInstanceStorageConfigRequestRequestTypeDef](./type_defs.md#disassociateinstancestorageconfigrequestrequesttypedef)
- [DisassociateLambdaFunctionRequestRequestTypeDef](./type_defs.md#disassociatelambdafunctionrequestrequesttypedef)
- [DisassociateLexBotRequestRequestTypeDef](./type_defs.md#disassociatelexbotrequestrequesttypedef)
- [DisassociateQueueQuickConnectsRequestRequestTypeDef](./type_defs.md#disassociatequeuequickconnectsrequestrequesttypedef)
- [DisassociateRoutingProfileQueuesRequestRequestTypeDef](./type_defs.md#disassociateroutingprofilequeuesrequestrequesttypedef)
- [DisassociateSecurityKeyRequestRequestTypeDef](./type_defs.md#disassociatesecuritykeyrequestrequesttypedef)
- [EncryptionConfigTypeDef](./type_defs.md#encryptionconfigtypedef)
- [FiltersTypeDef](./type_defs.md#filterstypedef)
- [GetContactAttributesRequestRequestTypeDef](./type_defs.md#getcontactattributesrequestrequesttypedef)
- [GetContactAttributesResponseTypeDef](./type_defs.md#getcontactattributesresponsetypedef)
- [GetCurrentMetricDataRequestRequestTypeDef](./type_defs.md#getcurrentmetricdatarequestrequesttypedef)
- [GetCurrentMetricDataResponseTypeDef](./type_defs.md#getcurrentmetricdataresponsetypedef)
- [GetFederationTokenRequestRequestTypeDef](./type_defs.md#getfederationtokenrequestrequesttypedef)
- [GetFederationTokenResponseTypeDef](./type_defs.md#getfederationtokenresponsetypedef)
- [GetMetricDataRequestGetMetricDataPaginateTypeDef](./type_defs.md#getmetricdatarequestgetmetricdatapaginatetypedef)
- [GetMetricDataRequestRequestTypeDef](./type_defs.md#getmetricdatarequestrequesttypedef)
- [GetMetricDataResponseTypeDef](./type_defs.md#getmetricdataresponsetypedef)
- [HierarchyGroupSummaryTypeDef](./type_defs.md#hierarchygroupsummarytypedef)
- [HierarchyGroupTypeDef](./type_defs.md#hierarchygrouptypedef)
- [HierarchyLevelTypeDef](./type_defs.md#hierarchyleveltypedef)
- [HierarchyLevelUpdateTypeDef](./type_defs.md#hierarchylevelupdatetypedef)
- [HierarchyPathTypeDef](./type_defs.md#hierarchypathtypedef)
- [HierarchyStructureTypeDef](./type_defs.md#hierarchystructuretypedef)
- [HierarchyStructureUpdateTypeDef](./type_defs.md#hierarchystructureupdatetypedef)
- [HistoricalMetricDataTypeDef](./type_defs.md#historicalmetricdatatypedef)
- [HistoricalMetricResultTypeDef](./type_defs.md#historicalmetricresulttypedef)
- [HistoricalMetricTypeDef](./type_defs.md#historicalmetrictypedef)
- [HoursOfOperationConfigTypeDef](./type_defs.md#hoursofoperationconfigtypedef)
- [HoursOfOperationSummaryTypeDef](./type_defs.md#hoursofoperationsummarytypedef)
- [HoursOfOperationTimeSliceTypeDef](./type_defs.md#hoursofoperationtimeslicetypedef)
- [HoursOfOperationTypeDef](./type_defs.md#hoursofoperationtypedef)
- [InstanceStatusReasonTypeDef](./type_defs.md#instancestatusreasontypedef)
- [InstanceStorageConfigTypeDef](./type_defs.md#instancestorageconfigtypedef)
- [InstanceSummaryTypeDef](./type_defs.md#instancesummarytypedef)
- [InstanceTypeDef](./type_defs.md#instancetypedef)
- [IntegrationAssociationSummaryTypeDef](./type_defs.md#integrationassociationsummarytypedef)
- [KinesisFirehoseConfigTypeDef](./type_defs.md#kinesisfirehoseconfigtypedef)
- [KinesisStreamConfigTypeDef](./type_defs.md#kinesisstreamconfigtypedef)
- [KinesisVideoStreamConfigTypeDef](./type_defs.md#kinesisvideostreamconfigtypedef)
- [LexBotConfigTypeDef](./type_defs.md#lexbotconfigtypedef)
- [LexBotTypeDef](./type_defs.md#lexbottypedef)
- [LexV2BotTypeDef](./type_defs.md#lexv2bottypedef)
- [ListAgentStatusRequestListAgentStatusesPaginateTypeDef](./type_defs.md#listagentstatusrequestlistagentstatusespaginatetypedef)
- [ListAgentStatusRequestRequestTypeDef](./type_defs.md#listagentstatusrequestrequesttypedef)
- [ListAgentStatusResponseTypeDef](./type_defs.md#listagentstatusresponsetypedef)
- [ListApprovedOriginsRequestListApprovedOriginsPaginateTypeDef](./type_defs.md#listapprovedoriginsrequestlistapprovedoriginspaginatetypedef)
- [ListApprovedOriginsRequestRequestTypeDef](./type_defs.md#listapprovedoriginsrequestrequesttypedef)
- [ListApprovedOriginsResponseTypeDef](./type_defs.md#listapprovedoriginsresponsetypedef)
- [ListBotsRequestListBotsPaginateTypeDef](./type_defs.md#listbotsrequestlistbotspaginatetypedef)
- [ListBotsRequestRequestTypeDef](./type_defs.md#listbotsrequestrequesttypedef)
- [ListBotsResponseTypeDef](./type_defs.md#listbotsresponsetypedef)
- [ListContactFlowModulesRequestListContactFlowModulesPaginateTypeDef](./type_defs.md#listcontactflowmodulesrequestlistcontactflowmodulespaginatetypedef)
- [ListContactFlowModulesRequestRequestTypeDef](./type_defs.md#listcontactflowmodulesrequestrequesttypedef)
- [ListContactFlowModulesResponseTypeDef](./type_defs.md#listcontactflowmodulesresponsetypedef)
- [ListContactFlowsRequestListContactFlowsPaginateTypeDef](./type_defs.md#listcontactflowsrequestlistcontactflowspaginatetypedef)
- [ListContactFlowsRequestRequestTypeDef](./type_defs.md#listcontactflowsrequestrequesttypedef)
- [ListContactFlowsResponseTypeDef](./type_defs.md#listcontactflowsresponsetypedef)
- [ListContactReferencesRequestListContactReferencesPaginateTypeDef](./type_defs.md#listcontactreferencesrequestlistcontactreferencespaginatetypedef)
- [ListContactReferencesRequestRequestTypeDef](./type_defs.md#listcontactreferencesrequestrequesttypedef)
- [ListContactReferencesResponseTypeDef](./type_defs.md#listcontactreferencesresponsetypedef)
- [ListDefaultVocabulariesRequestListDefaultVocabulariesPaginateTypeDef](./type_defs.md#listdefaultvocabulariesrequestlistdefaultvocabulariespaginatetypedef)
- [ListDefaultVocabulariesRequestRequestTypeDef](./type_defs.md#listdefaultvocabulariesrequestrequesttypedef)
- [ListDefaultVocabulariesResponseTypeDef](./type_defs.md#listdefaultvocabulariesresponsetypedef)
- [ListHoursOfOperationsRequestListHoursOfOperationsPaginateTypeDef](./type_defs.md#listhoursofoperationsrequestlisthoursofoperationspaginatetypedef)
- [ListHoursOfOperationsRequestRequestTypeDef](./type_defs.md#listhoursofoperationsrequestrequesttypedef)
- [ListHoursOfOperationsResponseTypeDef](./type_defs.md#listhoursofoperationsresponsetypedef)
- [ListInstanceAttributesRequestListInstanceAttributesPaginateTypeDef](./type_defs.md#listinstanceattributesrequestlistinstanceattributespaginatetypedef)
- [ListInstanceAttributesRequestRequestTypeDef](./type_defs.md#listinstanceattributesrequestrequesttypedef)
- [ListInstanceAttributesResponseTypeDef](./type_defs.md#listinstanceattributesresponsetypedef)
- [ListInstanceStorageConfigsRequestListInstanceStorageConfigsPaginateTypeDef](./type_defs.md#listinstancestorageconfigsrequestlistinstancestorageconfigspaginatetypedef)
- [ListInstanceStorageConfigsRequestRequestTypeDef](./type_defs.md#listinstancestorageconfigsrequestrequesttypedef)
- [ListInstanceStorageConfigsResponseTypeDef](./type_defs.md#listinstancestorageconfigsresponsetypedef)
- [ListInstancesRequestListInstancesPaginateTypeDef](./type_defs.md#listinstancesrequestlistinstancespaginatetypedef)
- [ListInstancesRequestRequestTypeDef](./type_defs.md#listinstancesrequestrequesttypedef)
- [ListInstancesResponseTypeDef](./type_defs.md#listinstancesresponsetypedef)
- [ListIntegrationAssociationsRequestListIntegrationAssociationsPaginateTypeDef](./type_defs.md#listintegrationassociationsrequestlistintegrationassociationspaginatetypedef)
- [ListIntegrationAssociationsRequestRequestTypeDef](./type_defs.md#listintegrationassociationsrequestrequesttypedef)
- [ListIntegrationAssociationsResponseTypeDef](./type_defs.md#listintegrationassociationsresponsetypedef)
- [ListLambdaFunctionsRequestListLambdaFunctionsPaginateTypeDef](./type_defs.md#listlambdafunctionsrequestlistlambdafunctionspaginatetypedef)
- [ListLambdaFunctionsRequestRequestTypeDef](./type_defs.md#listlambdafunctionsrequestrequesttypedef)
- [ListLambdaFunctionsResponseTypeDef](./type_defs.md#listlambdafunctionsresponsetypedef)
- [ListLexBotsRequestListLexBotsPaginateTypeDef](./type_defs.md#listlexbotsrequestlistlexbotspaginatetypedef)
- [ListLexBotsRequestRequestTypeDef](./type_defs.md#listlexbotsrequestrequesttypedef)
- [ListLexBotsResponseTypeDef](./type_defs.md#listlexbotsresponsetypedef)
- [ListPhoneNumbersRequestListPhoneNumbersPaginateTypeDef](./type_defs.md#listphonenumbersrequestlistphonenumberspaginatetypedef)
- [ListPhoneNumbersRequestRequestTypeDef](./type_defs.md#listphonenumbersrequestrequesttypedef)
- [ListPhoneNumbersResponseTypeDef](./type_defs.md#listphonenumbersresponsetypedef)
- [ListPromptsRequestListPromptsPaginateTypeDef](./type_defs.md#listpromptsrequestlistpromptspaginatetypedef)
- [ListPromptsRequestRequestTypeDef](./type_defs.md#listpromptsrequestrequesttypedef)
- [ListPromptsResponseTypeDef](./type_defs.md#listpromptsresponsetypedef)
- [ListQueueQuickConnectsRequestListQueueQuickConnectsPaginateTypeDef](./type_defs.md#listqueuequickconnectsrequestlistqueuequickconnectspaginatetypedef)
- [ListQueueQuickConnectsRequestRequestTypeDef](./type_defs.md#listqueuequickconnectsrequestrequesttypedef)
- [ListQueueQuickConnectsResponseTypeDef](./type_defs.md#listqueuequickconnectsresponsetypedef)
- [ListQueuesRequestListQueuesPaginateTypeDef](./type_defs.md#listqueuesrequestlistqueuespaginatetypedef)
- [ListQueuesRequestRequestTypeDef](./type_defs.md#listqueuesrequestrequesttypedef)
- [ListQueuesResponseTypeDef](./type_defs.md#listqueuesresponsetypedef)
- [ListQuickConnectsRequestListQuickConnectsPaginateTypeDef](./type_defs.md#listquickconnectsrequestlistquickconnectspaginatetypedef)
- [ListQuickConnectsRequestRequestTypeDef](./type_defs.md#listquickconnectsrequestrequesttypedef)
- [ListQuickConnectsResponseTypeDef](./type_defs.md#listquickconnectsresponsetypedef)
- [ListRoutingProfileQueuesRequestListRoutingProfileQueuesPaginateTypeDef](./type_defs.md#listroutingprofilequeuesrequestlistroutingprofilequeuespaginatetypedef)
- [ListRoutingProfileQueuesRequestRequestTypeDef](./type_defs.md#listroutingprofilequeuesrequestrequesttypedef)
- [ListRoutingProfileQueuesResponseTypeDef](./type_defs.md#listroutingprofilequeuesresponsetypedef)
- [ListRoutingProfilesRequestListRoutingProfilesPaginateTypeDef](./type_defs.md#listroutingprofilesrequestlistroutingprofilespaginatetypedef)
- [ListRoutingProfilesRequestRequestTypeDef](./type_defs.md#listroutingprofilesrequestrequesttypedef)
- [ListRoutingProfilesResponseTypeDef](./type_defs.md#listroutingprofilesresponsetypedef)
- [ListSecurityKeysRequestListSecurityKeysPaginateTypeDef](./type_defs.md#listsecuritykeysrequestlistsecuritykeyspaginatetypedef)
- [ListSecurityKeysRequestRequestTypeDef](./type_defs.md#listsecuritykeysrequestrequesttypedef)
- [ListSecurityKeysResponseTypeDef](./type_defs.md#listsecuritykeysresponsetypedef)
- [ListSecurityProfilePermissionsRequestListSecurityProfilePermissionsPaginateTypeDef](./type_defs.md#listsecurityprofilepermissionsrequestlistsecurityprofilepermissionspaginatetypedef)
- [ListSecurityProfilePermissionsRequestRequestTypeDef](./type_defs.md#listsecurityprofilepermissionsrequestrequesttypedef)
- [ListSecurityProfilePermissionsResponseTypeDef](./type_defs.md#listsecurityprofilepermissionsresponsetypedef)
- [ListSecurityProfilesRequestListSecurityProfilesPaginateTypeDef](./type_defs.md#listsecurityprofilesrequestlistsecurityprofilespaginatetypedef)
- [ListSecurityProfilesRequestRequestTypeDef](./type_defs.md#listsecurityprofilesrequestrequesttypedef)
- [ListSecurityProfilesResponseTypeDef](./type_defs.md#listsecurityprofilesresponsetypedef)
- [ListTagsForResourceRequestRequestTypeDef](./type_defs.md#listtagsforresourcerequestrequesttypedef)
- [ListTagsForResourceResponseTypeDef](./type_defs.md#listtagsforresourceresponsetypedef)
- [ListUseCasesRequestListUseCasesPaginateTypeDef](./type_defs.md#listusecasesrequestlistusecasespaginatetypedef)
- [ListUseCasesRequestRequestTypeDef](./type_defs.md#listusecasesrequestrequesttypedef)
- [ListUseCasesResponseTypeDef](./type_defs.md#listusecasesresponsetypedef)
- [ListUserHierarchyGroupsRequestListUserHierarchyGroupsPaginateTypeDef](./type_defs.md#listuserhierarchygroupsrequestlistuserhierarchygroupspaginatetypedef)
- [ListUserHierarchyGroupsRequestRequestTypeDef](./type_defs.md#listuserhierarchygroupsrequestrequesttypedef)
- [ListUserHierarchyGroupsResponseTypeDef](./type_defs.md#listuserhierarchygroupsresponsetypedef)
- [ListUsersRequestListUsersPaginateTypeDef](./type_defs.md#listusersrequestlistuserspaginatetypedef)
- [ListUsersRequestRequestTypeDef](./type_defs.md#listusersrequestrequesttypedef)
- [ListUsersResponseTypeDef](./type_defs.md#listusersresponsetypedef)
- [MediaConcurrencyTypeDef](./type_defs.md#mediaconcurrencytypedef)
- [OutboundCallerConfigTypeDef](./type_defs.md#outboundcallerconfigtypedef)
- [PaginatorConfigTypeDef](./type_defs.md#paginatorconfigtypedef)
- [ParticipantDetailsTypeDef](./type_defs.md#participantdetailstypedef)
- [PhoneNumberQuickConnectConfigTypeDef](./type_defs.md#phonenumberquickconnectconfigtypedef)
- [PhoneNumberSummaryTypeDef](./type_defs.md#phonenumbersummarytypedef)
- [PromptSummaryTypeDef](./type_defs.md#promptsummarytypedef)
- [QueueInfoTypeDef](./type_defs.md#queueinfotypedef)
- [QueueQuickConnectConfigTypeDef](./type_defs.md#queuequickconnectconfigtypedef)
- [QueueReferenceTypeDef](./type_defs.md#queuereferencetypedef)
- [QueueSummaryTypeDef](./type_defs.md#queuesummarytypedef)
- [QueueTypeDef](./type_defs.md#queuetypedef)
- [QuickConnectConfigTypeDef](./type_defs.md#quickconnectconfigtypedef)
- [QuickConnectSummaryTypeDef](./type_defs.md#quickconnectsummarytypedef)
- [QuickConnectTypeDef](./type_defs.md#quickconnecttypedef)
- [ReferenceSummaryTypeDef](./type_defs.md#referencesummarytypedef)
- [ReferenceTypeDef](./type_defs.md#referencetypedef)
- [ResponseMetadataTypeDef](./type_defs.md#responsemetadatatypedef)
- [ResumeContactRecordingRequestRequestTypeDef](./type_defs.md#resumecontactrecordingrequestrequesttypedef)
- [RoutingProfileQueueConfigSummaryTypeDef](./type_defs.md#routingprofilequeueconfigsummarytypedef)
- [RoutingProfileQueueConfigTypeDef](./type_defs.md#routingprofilequeueconfigtypedef)
- [RoutingProfileQueueReferenceTypeDef](./type_defs.md#routingprofilequeuereferencetypedef)
- [RoutingProfileSummaryTypeDef](./type_defs.md#routingprofilesummarytypedef)
- [RoutingProfileTypeDef](./type_defs.md#routingprofiletypedef)
- [S3ConfigTypeDef](./type_defs.md#s3configtypedef)
- [SearchVocabulariesRequestRequestTypeDef](./type_defs.md#searchvocabulariesrequestrequesttypedef)
- [SearchVocabulariesRequestSearchVocabulariesPaginateTypeDef](./type_defs.md#searchvocabulariesrequestsearchvocabulariespaginatetypedef)
- [SearchVocabulariesResponseTypeDef](./type_defs.md#searchvocabulariesresponsetypedef)
- [SecurityKeyTypeDef](./type_defs.md#securitykeytypedef)
- [SecurityProfileSummaryTypeDef](./type_defs.md#securityprofilesummarytypedef)
- [SecurityProfileTypeDef](./type_defs.md#securityprofiletypedef)
- [StartChatContactRequestRequestTypeDef](./type_defs.md#startchatcontactrequestrequesttypedef)
- [StartChatContactResponseTypeDef](./type_defs.md#startchatcontactresponsetypedef)
- [StartContactRecordingRequestRequestTypeDef](./type_defs.md#startcontactrecordingrequestrequesttypedef)
- [StartContactStreamingRequestRequestTypeDef](./type_defs.md#startcontactstreamingrequestrequesttypedef)
- [StartContactStreamingResponseTypeDef](./type_defs.md#startcontactstreamingresponsetypedef)
- [StartOutboundVoiceContactRequestRequestTypeDef](./type_defs.md#startoutboundvoicecontactrequestrequesttypedef)
- [StartOutboundVoiceContactResponseTypeDef](./type_defs.md#startoutboundvoicecontactresponsetypedef)
- [StartTaskContactRequestRequestTypeDef](./type_defs.md#starttaskcontactrequestrequesttypedef)
- [StartTaskContactResponseTypeDef](./type_defs.md#starttaskcontactresponsetypedef)
- [StopContactRecordingRequestRequestTypeDef](./type_defs.md#stopcontactrecordingrequestrequesttypedef)
- [StopContactRequestRequestTypeDef](./type_defs.md#stopcontactrequestrequesttypedef)
- [StopContactStreamingRequestRequestTypeDef](./type_defs.md#stopcontactstreamingrequestrequesttypedef)
- [SuspendContactRecordingRequestRequestTypeDef](./type_defs.md#suspendcontactrecordingrequestrequesttypedef)
- [TagResourceRequestRequestTypeDef](./type_defs.md#tagresourcerequestrequesttypedef)
- [ThresholdTypeDef](./type_defs.md#thresholdtypedef)
- [UntagResourceRequestRequestTypeDef](./type_defs.md#untagresourcerequestrequesttypedef)
- [UpdateAgentStatusRequestRequestTypeDef](./type_defs.md#updateagentstatusrequestrequesttypedef)
- [UpdateContactAttributesRequestRequestTypeDef](./type_defs.md#updatecontactattributesrequestrequesttypedef)
- [UpdateContactFlowContentRequestRequestTypeDef](./type_defs.md#updatecontactflowcontentrequestrequesttypedef)
- [UpdateContactFlowMetadataRequestRequestTypeDef](./type_defs.md#updatecontactflowmetadatarequestrequesttypedef)
- [UpdateContactFlowModuleContentRequestRequestTypeDef](./type_defs.md#updatecontactflowmodulecontentrequestrequesttypedef)
- [UpdateContactFlowModuleMetadataRequestRequestTypeDef](./type_defs.md#updatecontactflowmodulemetadatarequestrequesttypedef)
- [UpdateContactFlowNameRequestRequestTypeDef](./type_defs.md#updatecontactflownamerequestrequesttypedef)
- [UpdateContactRequestRequestTypeDef](./type_defs.md#updatecontactrequestrequesttypedef)
- [UpdateContactScheduleRequestRequestTypeDef](./type_defs.md#updatecontactschedulerequestrequesttypedef)
- [UpdateHoursOfOperationRequestRequestTypeDef](./type_defs.md#updatehoursofoperationrequestrequesttypedef)
- [UpdateInstanceAttributeRequestRequestTypeDef](./type_defs.md#updateinstanceattributerequestrequesttypedef)
- [UpdateInstanceStorageConfigRequestRequestTypeDef](./type_defs.md#updateinstancestorageconfigrequestrequesttypedef)
- [UpdateQueueHoursOfOperationRequestRequestTypeDef](./type_defs.md#updatequeuehoursofoperationrequestrequesttypedef)
- [UpdateQueueMaxContactsRequestRequestTypeDef](./type_defs.md#updatequeuemaxcontactsrequestrequesttypedef)
- [UpdateQueueNameRequestRequestTypeDef](./type_defs.md#updatequeuenamerequestrequesttypedef)
- [UpdateQueueOutboundCallerConfigRequestRequestTypeDef](./type_defs.md#updatequeueoutboundcallerconfigrequestrequesttypedef)
- [UpdateQueueStatusRequestRequestTypeDef](./type_defs.md#updatequeuestatusrequestrequesttypedef)
- [UpdateQuickConnectConfigRequestRequestTypeDef](./type_defs.md#updatequickconnectconfigrequestrequesttypedef)
- [UpdateQuickConnectNameRequestRequestTypeDef](./type_defs.md#updatequickconnectnamerequestrequesttypedef)
- [UpdateRoutingProfileConcurrencyRequestRequestTypeDef](./type_defs.md#updateroutingprofileconcurrencyrequestrequesttypedef)
- [UpdateRoutingProfileDefaultOutboundQueueRequestRequestTypeDef](./type_defs.md#updateroutingprofiledefaultoutboundqueuerequestrequesttypedef)
- [UpdateRoutingProfileNameRequestRequestTypeDef](./type_defs.md#updateroutingprofilenamerequestrequesttypedef)
- [UpdateRoutingProfileQueuesRequestRequestTypeDef](./type_defs.md#updateroutingprofilequeuesrequestrequesttypedef)
- [UpdateSecurityProfileRequestRequestTypeDef](./type_defs.md#updatesecurityprofilerequestrequesttypedef)
- [UpdateUserHierarchyGroupNameRequestRequestTypeDef](./type_defs.md#updateuserhierarchygroupnamerequestrequesttypedef)
- [UpdateUserHierarchyRequestRequestTypeDef](./type_defs.md#updateuserhierarchyrequestrequesttypedef)
- [UpdateUserHierarchyStructureRequestRequestTypeDef](./type_defs.md#updateuserhierarchystructurerequestrequesttypedef)
- [UpdateUserIdentityInfoRequestRequestTypeDef](./type_defs.md#updateuseridentityinforequestrequesttypedef)
- [UpdateUserPhoneConfigRequestRequestTypeDef](./type_defs.md#updateuserphoneconfigrequestrequesttypedef)
- [UpdateUserRoutingProfileRequestRequestTypeDef](./type_defs.md#updateuserroutingprofilerequestrequesttypedef)
- [UpdateUserSecurityProfilesRequestRequestTypeDef](./type_defs.md#updateusersecurityprofilesrequestrequesttypedef)
- [UrlReferenceTypeDef](./type_defs.md#urlreferencetypedef)
- [UseCaseTypeDef](./type_defs.md#usecasetypedef)
- [UserIdentityInfoTypeDef](./type_defs.md#useridentityinfotypedef)
- [UserPhoneConfigTypeDef](./type_defs.md#userphoneconfigtypedef)
- [UserQuickConnectConfigTypeDef](./type_defs.md#userquickconnectconfigtypedef)
- [UserSummaryTypeDef](./type_defs.md#usersummarytypedef)
- [UserTypeDef](./type_defs.md#usertypedef)
- [VocabularySummaryTypeDef](./type_defs.md#vocabularysummarytypedef)
- [VocabularyTypeDef](./type_defs.md#vocabularytypedef)
- [VoiceRecordingConfigurationTypeDef](./type_defs.md#voicerecordingconfigurationtypedef)

