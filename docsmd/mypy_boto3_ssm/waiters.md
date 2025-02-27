# Waiters

> [Index](../README.md) > [SSM](./README.md) > Waiters

!!! note ""

    Auto-generated documentation for [SSM](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM)
    type annotations stubs module [mypy-boto3-ssm](https://pypi.org/project/mypy-boto3-ssm/).

## CommandExecutedWaiter

Type annotations and code completion for `#!python boto3.client("ssm").get_waiter("command_executed")`.
[:material-aws: boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/ssm.html#SSM.Waiter.CommandExecuted)

```python title="Usage example"
from boto3.session import Session

from mypy_boto3_ssm.waiter import CommandExecutedWaiter

def get_command_executed_waiter() -> CommandExecutedWaiter:
    return Session().client("ssm").get_waiter("command_executed")
```


### wait

Type annotations and code completion for `#!python CommandExecutedWaiter.wait` method.

```python title="Method definition"
def wait(
    self,
    *,
    CommandId: str,
    InstanceId: str,
    PluginName: str = ...,
    WaiterConfig: WaiterConfigTypeDef = ...,  # (1)
) -> None:
    ...
```

1. See [:material-code-braces: WaiterConfigTypeDef](./type_defs.md#waiterconfigtypedef) 


```python title="Usage example with kwargs"
kwargs: GetCommandInvocationRequestCommandExecutedWaitTypeDef = {  # (1)
    "CommandId": ...,
    "InstanceId": ...,
}

parent.wait(**kwargs)
```

1. See [:material-code-braces: GetCommandInvocationRequestCommandExecutedWaitTypeDef](./type_defs.md#getcommandinvocationrequestcommandexecutedwaittypedef) 
