# alicebot.adapter.mirai.event.mate

默认不会被传播的特殊事件。

## _class_ `MateEvent` {#MateEvent}

Bases: `alicebot.adapter.mirai.event.base.MiraiEvent`

默认不会被传播的特殊事件

### _method_ `__init__(__pydantic_self__, **data)` {#BaseModel.\_\_init\_\_}

Create a new model by parsing and validating input data from keyword arguments.

Raises [`ValidationError`][pydantic_core.ValidationError] if the input data cannot be
validated to form a valid model.

`__init__` uses `__pydantic_self__` instead of the more common `self` for the first arg to
allow `self` as a field name.

- **Arguments**

  - **data** (_Any_)

- **Returns**

  Type: _None_

## _class_ `BotEvent` {#BotEvent}

Bases: `alicebot.adapter.mirai.event.mate.MateEvent`

Bot 自身事件

- **Attributes**

  - **qq** (_int_)

### _method_ `__init__(__pydantic_self__, **data)` {#BaseModel.\_\_init\_\_}

Create a new model by parsing and validating input data from keyword arguments.

Raises [`ValidationError`][pydantic_core.ValidationError] if the input data cannot be
validated to form a valid model.

`__init__` uses `__pydantic_self__` instead of the more common `self` for the first arg to
allow `self` as a field name.

- **Arguments**

  - **data** (_Any_)

- **Returns**

  Type: _None_

## _class_ `BotOnlineEvent` {#BotOnlineEvent}

Bases: `alicebot.adapter.mirai.event.mate.BotEvent`

Bot 登录成功

- **Attributes**

  - **type** (_Literal\['BotOnlineEvent'\]_)

### _method_ `__init__(__pydantic_self__, **data)` {#BaseModel.\_\_init\_\_}

Create a new model by parsing and validating input data from keyword arguments.

Raises [`ValidationError`][pydantic_core.ValidationError] if the input data cannot be
validated to form a valid model.

`__init__` uses `__pydantic_self__` instead of the more common `self` for the first arg to
allow `self` as a field name.

- **Arguments**

  - **data** (_Any_)

- **Returns**

  Type: _None_

## _class_ `BotOfflineEventActive` {#BotOfflineEventActive}

Bases: `alicebot.adapter.mirai.event.mate.BotEvent`

Bot 主动离线

- **Attributes**

  - **type** (_Literal\['BotOfflineEventActive'\]_)

### _method_ `__init__(__pydantic_self__, **data)` {#BaseModel.\_\_init\_\_}

Create a new model by parsing and validating input data from keyword arguments.

Raises [`ValidationError`][pydantic_core.ValidationError] if the input data cannot be
validated to form a valid model.

`__init__` uses `__pydantic_self__` instead of the more common `self` for the first arg to
allow `self` as a field name.

- **Arguments**

  - **data** (_Any_)

- **Returns**

  Type: _None_

## _class_ `BotOfflineEventForce` {#BotOfflineEventForce}

Bases: `alicebot.adapter.mirai.event.mate.BotEvent`

Bot 被挤下线

- **Attributes**

  - **type** (_Literal\['BotOfflineEventForce'\]_)

### _method_ `__init__(__pydantic_self__, **data)` {#BaseModel.\_\_init\_\_}

Create a new model by parsing and validating input data from keyword arguments.

Raises [`ValidationError`][pydantic_core.ValidationError] if the input data cannot be
validated to form a valid model.

`__init__` uses `__pydantic_self__` instead of the more common `self` for the first arg to
allow `self` as a field name.

- **Arguments**

  - **data** (_Any_)

- **Returns**

  Type: _None_

## _class_ `BotOfflineEventDropped` {#BotOfflineEventDropped}

Bases: `alicebot.adapter.mirai.event.mate.BotEvent`

Bot 被服务器断开或因网络问题而掉线

- **Attributes**

  - **type** (_Literal\['BotOfflineEventDropped'\]_)

### _method_ `__init__(__pydantic_self__, **data)` {#BaseModel.\_\_init\_\_}

Create a new model by parsing and validating input data from keyword arguments.

Raises [`ValidationError`][pydantic_core.ValidationError] if the input data cannot be
validated to form a valid model.

`__init__` uses `__pydantic_self__` instead of the more common `self` for the first arg to
allow `self` as a field name.

- **Arguments**

  - **data** (_Any_)

- **Returns**

  Type: _None_

## _class_ `BotReloginEvent` {#BotReloginEvent}

Bases: `alicebot.adapter.mirai.event.mate.BotEvent`

Bot 主动重新登录

- **Attributes**

  - **type** (_Literal\['BotReloginEvent'\]_)

### _method_ `__init__(__pydantic_self__, **data)` {#BaseModel.\_\_init\_\_}

Create a new model by parsing and validating input data from keyword arguments.

Raises [`ValidationError`][pydantic_core.ValidationError] if the input data cannot be
validated to form a valid model.

`__init__` uses `__pydantic_self__` instead of the more common `self` for the first arg to
allow `self` as a field name.

- **Arguments**

  - **data** (_Any_)

- **Returns**

  Type: _None_

## _class_ `CommandExecutedEvent` {#CommandExecutedEvent}

Bases: `alicebot.adapter.mirai.event.mate.MateEvent`

命令被执行

- **Attributes**

  - **type** (_Literal\['CommandExecutedEvent'\]_)

  - **name** (_str_)

  - **friend** (_Optional\[alicebot.adapter.mirai.event.base.FriendInfo\]_)

  - **member** (_Optional\[alicebot.adapter.mirai.event.base.GroupMemberInfo\]_)

  - **args** (_List\[Any\]_)

### _method_ `__init__(__pydantic_self__, **data)` {#BaseModel.\_\_init\_\_}

Create a new model by parsing and validating input data from keyword arguments.

Raises [`ValidationError`][pydantic_core.ValidationError] if the input data cannot be
validated to form a valid model.

`__init__` uses `__pydantic_self__` instead of the more common `self` for the first arg to
allow `self` as a field name.

- **Arguments**

  - **data** (_Any_)

- **Returns**

  Type: _None_
