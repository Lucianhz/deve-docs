# 群信息相关

{% api-method method="get" host="http://app.deve.xiaopao69.com" path="/plugins/restapi/v1/chatrooms/findUsers/:name" %}
{% api-method-summary %}
获取群成员\(旧API\)
{% endapi-method-summary %}

{% api-method-description %}
获取特定群的所有成员。
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="name" type="string" required=true %}
群名称，由用户名加数字构成比如：xp8888\_1112112
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authentication" type="string" required=true %}
你们懂得
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
成功获取到成员信息
{% endapi-method-response-example-description %}

```javascript
{
    "code": "0",// 你没看错 是字符串！
    "msg": "success",
    "data": [
    {
        // 略过一大堆属性
        "owner": true,// 是否为群主
        "manager": true,// 是否为管理员
    }
    ]
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



