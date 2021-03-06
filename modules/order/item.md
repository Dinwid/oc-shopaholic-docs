{% extends 'docs/modules/item-default.md' %}

{% block fields %}
{{ parent() }}

### Position total price fields

|  Name | Type | Description |
|-------|------|--------|
|position_total_price|string|Formatted position total price string (**"120,05"**)|
|position_total_price_value|float|Float position total price value (**120.05**)|
|old_position_total_price|string|Formatted position total old price string (**"125,05"**)|
|old_position_total_price_value|float|Float position total old price value (**125.05**)|
|discount_position_total_price|string|Formatted position total discount price string (**"5,00"**)|
|discount_position_total_price_value|float|Float position total discount price value (**5**)|
|position_total_price_data|[TotalPriceContainer](modules/price-container/home.md#TotalPriceContainer)|

### Shipping price fields

|  Name | Type | Description |
|-------|------|--------|
|shipping_price|string|Formatted shipping price string (**"10,50"**)|
|shipping_price_value|float|Float shipping price value (**10.5**)|
|old_shipping_price|string|Formatted old shipping price string (**"12,50"**)|
|old_shipping_price_value|float|Float old shipping price value (**12.5**)|
|discount_shipping_price|string|Formatted shipping discount price string (**"2,00"**)|
|discount_shipping_price_value|float|Float shipping discount price value (**2**)|
|shipping_price_data|[ItemPriceContainer](modules/price-container/home.md#ItemPriceContainer)|

### Total price fields

|  Name | Type | Description |
|-------|------|--------|
|total_price|string|Formatted order total price string (**"130,55"**)|
|total_price_value|float|Float order total price value (**130.55**)|
|old_total_price|string|Formatted order total old price string (**"137,55"**)|
|old_total_price_value|float|Float order total old price value (**137.55**)|
|discount_total_price|string|Formatted order total discount price string (**"7,00"**)|
|discount_total_price_value|float|Float order total discount price value (**7**)|
|total_price_data|[ItemPriceContainer](modules/price-container/home.md#ItemPriceContainer)|

{% endblock %}

{% block method_list %}{% endblock %}