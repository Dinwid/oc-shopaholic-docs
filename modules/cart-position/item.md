{% extends 'docs/modules/item-default.md' %}

{% block fields %}
{{ parent() }}

### Price fields

|  Name | Type | Description |
|-------|------|--------|
|price|string|Formatted price string|
|price_value|float|Float price value|
|price_with_tax|string|Formatted price with tax string|
|price_with_tax_value|float|Float price with tax value|
|price_without_tax|string|Formatted price without tax string|
|price_without_tax_value|float|Float price without tax value|
|tax_price|string|Formatted tax price string|
|tax_price_value|float|Float tax price value|

### Old price fields

|  Name | Type | Description |
|-------|------|--------|
|old_price|string|Formatted old price string|
|old_price_value|float|Float old price value|
|old_price_with_tax|string|Formatted old price with tax string|
|old_price_with_tax_value|float|Float old price with tax value|
|old_price_without_tax|string|Formatted old price without tax string|
|old_price_without_tax_value|float|Float old price without tax value|
|tax_old_price|string|Formatted tax old price string|
|tax_old_price_value|float|Float tax old price value|

### Discount price fields

|  Name | Type | Description |
|-------|------|--------|
|discount_price|string|Formatted discount price string|
|discount_price_value|float|Float discount price value|
|discount_price_with_tax|string|Formatted discount price with tax string|
|discount_price_with_tax_value|float|Float discount price with tax value|
|discount_price_without_tax|string|Formatted discount price without tax string|
|discount_price_without_tax_value|float|Float discount price without tax value|
|tax_discount_price|string|Formatted tax discount price string|
|tax_discount_price_value|float|Float tax discount price value|

### Price per unit fields

|  Name | Type | Description |
|-------|------|--------|
|price_per_unit|string|Formatted price per unit string|
|price_per_unit_value|float|Float price per unit value|
|price_per_unit_with_tax|string|Formatted price per unit with tax string|
|price_per_unit_with_tax_value|float|Float price per unit with tax value|
|price_per_unit_without_tax|string|Formatted price per unit without tax string|
|price_per_unit_without_tax_value|float|Float price per unit without tax value|
|tax_price_per_unit|string|Formatted tax price per unit string|
|tax_price_per_unit_value|float|Float tax price per unit value|

### Old price per unit fields

|  Name | Type | Description |
|-------|------|--------|
|old_price_per_unit|string|Formatted old price per unit string|
|old_price_per_unit_value|float|Float old price per unit value|
|old_price_per_unit_with_tax|string|Formatted old price per unit with tax string|
|old_price_per_unit_with_tax_value|float|Float old price per unit with tax value|
|old_price_per_unit_without_tax|string|Formatted old price per unit without tax string|
|old_price_per_unit_without_tax_value|float|Float old price per unit without tax value|
|tax_old_price_per_unit|string|Formatted tax old price per unit string|
|tax_old_price_per_unit_value|float|Float tax old price per unit value|

### Discount price per unit fields

|  Name | Type | Description |
|-------|------|--------|
|discount_price_per_unit|string|Formatted discount price per unit string|
|discount_price_per_unit_value|float|Float discount price per unit value|
|discount_price_per_unit_with_tax|string|Formatted discount price per unit with tax string|
|discount_price_per_unit_with_tax_value|float|Float discount price per unit with tax value|
|discount_price_per_unit_without_tax|string|Formatted discount price per unit without tax string|
|discount_price_per_unit_without_tax_value|float|Float discount price per unit without tax value|
|tax_discount_price_per_unit|string|Formatted tax discount price per unit string|
|tax_discount_price_per_unit_value|float|Float tax discount price per unit value|
{% endblock %}

{% block method_list %}{% endblock %}