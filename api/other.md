# 其他

{% api-method method="get" host="https://www.deve.xiaopao69.com" path="/red-restful/other/gameStatus" %}
{% api-method-summary %}
获取游戏开启状态
{% endapi-method-summary %}

{% api-method-description %}
游戏开启状态；若返回的是false则不显示「游戏」以及相关菜单  
  
服务端实现则比较简单，读取sys\_config表 设置一个字段，若该字段不存在则返回true。
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-headers %}
{% api-method-parameter name="Authentication" type="string" required=true %}
Authentication token to track down who is emptying our stocks.
{% endapi-method-parameter %}
{% endapi-method-headers %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```javascript
true
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



