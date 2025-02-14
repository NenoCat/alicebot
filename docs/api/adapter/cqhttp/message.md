# alicebot.adapter.cqhttp.message

CQHTTP 适配器消息。

## _class_ `CQHTTPMessage` {#CQHTTPMessage}

Bases: `alicebot.message.Message`

CQHTTP 消息。

### _method_ `__init__(self, *messages)` {#Message.\_\_init\_\_}

初始化。

- **Arguments**

  - **\*messages** (_Union\[List\[~MessageSegmentT\], ~MessageSegmentT, str, Mapping\[str, Any\]\]_) - 可以被转化为消息的数据。

- **Returns**

  Type: _None_

### _method_ `get_segment_class()` {#CQHTTPMessage.get\_segment\_class}

获取消息字段类。

- **Returns**

  Type: _Type\[CQHTTPMessageSegment\]_

  消息字段类。

## _class_ `CQHTTPMessageSegment` {#CQHTTPMessageSegment}

Bases: `alicebot.message.MessageSegment[CQHTTPMessage]`

CQHTTP 消息字段。

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

### _method_ `anonymous(ignore = None)` {#CQHTTPMessageSegment.anonymous}

匿名发消息

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `at(qq)` {#CQHTTPMessageSegment.at}

@某人

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `contact(type_, id_)` {#CQHTTPMessageSegment.contact}

推荐好友/推荐群

- **Arguments**

  - **id\_** (_int_)

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `contact_friend(id_)` {#CQHTTPMessageSegment.contact\_friend}

推荐好友

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `contact_group(id_)` {#CQHTTPMessageSegment.contact\_group}

推荐好友

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `dice()` {#CQHTTPMessageSegment.dice}

掷骰子魔法表情

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `face(id_)` {#CQHTTPMessageSegment.face}

QQ 表情

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `from_str(msg)` {#CQHTTPMessageSegment.from\_str}

用于将 `str` 转换为消息字段。

- **Returns**

  Type: _typing\_extensions.Self_

  由 `str` 转换的消息字段。

### _method_ `get_cqcode(self)` {#CQHTTPMessageSegment.get\_cqcode}

获取此消息字段的 CQ 码形式。

- **Returns**

  Type: _str_

  此消息字段的 CQ 码形式。

### _method_ `get_message_class()` {#CQHTTPMessageSegment.get\_message\_class}

获取消息类。

- **Returns**

  Type: _Type\[alicebot.adapter.cqhttp.message.CQHTTPMessage\]_

  消息类。

### _method_ `image(file, type_ = None, cache = True, proxy = True, timeout = None)` {#CQHTTPMessageSegment.image}

图片

- **Arguments**

  - **type\_** (_Optional\[Literal\['flash'\]\]_)

  - **cache** (_bool_)

  - **proxy** (_bool_)

  - **timeout** (_Optional\[int\]_)

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `json_message(data)` {#CQHTTPMessageSegment.json\_message}

JSON 消息

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `location(lat, lon, title, content = None)` {#CQHTTPMessageSegment.location}

位置

- **Arguments**

  - **lon** (_float_)

  - **title** (_Optional\[str\]_)

  - **content** (_Optional\[str\]_)

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `music(type_, id_)` {#CQHTTPMessageSegment.music}

音乐分享

- **Arguments**

  - **id\_** (_int_)

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `music_custom(url, audio, title, content = None, image = None)` {#CQHTTPMessageSegment.music\_custom}

音乐自定义分享

- **Arguments**

  - **audio** (_str_)

  - **title** (_str_)

  - **content** (_Optional\[str\]_)

  - **image** (_Optional\[str\]_)

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `node(id_)` {#CQHTTPMessageSegment.node}

合并转发节点

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `node_custom(user_id, nickname, content)` {#CQHTTPMessageSegment.node\_custom}

合并转发自定义节点

- **Arguments**

  - **nickname** (_str_)

  - **content** (_CQHTTPMessage_)

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `poke(type_, id_)` {#CQHTTPMessageSegment.poke}

戳一戳

- **Arguments**

  - **id\_** (_int_)

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `record(file, magic = False, cache = True, proxy = True, timeout = None)` {#CQHTTPMessageSegment.record}

语音

- **Arguments**

  - **magic** (_bool_)

  - **cache** (_bool_)

  - **proxy** (_bool_)

  - **timeout** (_Optional\[int\]_)

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `reply(id_)` {#CQHTTPMessageSegment.reply}

回复

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `rps()` {#CQHTTPMessageSegment.rps}

猜拳魔法表情

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `shake()` {#CQHTTPMessageSegment.shake}

窗口抖动 (戳一戳)

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `share(url, title, content = None, image = None)` {#CQHTTPMessageSegment.share}

链接分享

- **Arguments**

  - **title** (_str_)

  - **content** (_Optional\[str\]_)

  - **image** (_Optional\[str\]_)

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `text(text)` {#CQHTTPMessageSegment.text}

纯文本

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `video(file, cache = True, proxy = True, timeout = None)` {#CQHTTPMessageSegment.video}

短视频

- **Arguments**

  - **cache** (_bool_)

  - **proxy** (_bool_)

  - **timeout** (_Optional\[int\]_)

- **Returns**

  Type: _typing\_extensions.Self_

### _method_ `xml_message(data)` {#CQHTTPMessageSegment.xml\_message}

XML 消息

- **Returns**

  Type: _typing\_extensions.Self_

## _function_ `escape(string, *, escape_comma = True)` {#escape}

对 CQ 码中的特殊字符进行转义。

- **Arguments**

  - **string** (_str_) - 待转义的字符串。

  - **escape\_comma** (_bool_) - 是否转义 `,`。

- **Returns**

  Type: _str_

  转义后的字符串。
