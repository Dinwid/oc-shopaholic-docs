{% extends 'docs/modules/examples-default.md' %}

{% block content %}
##  Example 1: Accessories on product page

### 1.1 Task

Create simple product page and render block with 5 random accessories.

> Block with accessories can look like any block with product list.
Block can be simple (for example: slider with 5 random accessories).
Block can be complicated (contain searching, filtering, sorting, pagination).

### 1.2 How can i do it?

!> Module {{ module.available|available_with|lcfirst }}

```plantuml
@startuml
:Create simple product page;
:Get ProductItem object
from ProductPage component;
:Get ProductCollection object
with accessories from
ProductItem object;
:Apply filter by "active" field
to ProductCollection object;
:Get array with 5 random products
from ProductCollection object;
:Render block with accessories;
@enduml
```

### 1.3 Source code

Simple example of product page.

File: **pages/product.htm**
{% verbatim %}
```twig
title = "Product page"
url = "/product/:slug"
layout = "main"
is_hidden = 0

[ProductPage]
slug = "{{ :slug }}"
slug_required = 1
smart_url_check = 1
skip_error = 0
==

{# Get product item #}
{% set obProduct = ProductPage.get() %}

<div data-id="{{ obProduct.id }}" itemscope itemtype="http://schema.org/Product">
    <h1 itemprop="name">{{ obProduct.name }}</h1>
</div>

{# Get accessories + apply filder by "active" field #}
{% set obProductList = obProduct.accessory.active() %}
{% set arProductList = obProductList.random(5) %}
{% if arProductList is not empty %}
<div>
    <span>Accessories</span>
    {# Render product list #}
    <ul>
        {% for obProduct in arProductList %}
            <li>{% partial 'product/product-card/product-card' obProduct=obProduct %}</li>
        {% endfor %}
    </ul>
</div>
{% endif %}
```
{% endverbatim %}
{% endblock %}