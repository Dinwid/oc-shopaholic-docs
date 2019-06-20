# Event list: Offer

## **shopaholic.sorting.offer.get.list**

Event allows you to quickly add custom sorting for list of offers ([OfferCollection](modules/offer/collection/collection.md) class, sort() method)

For example:
```php
Event::listen('shopaholic.sorting.offer.get.list', function($sSorting) {
    if ($sSorting != 'my_custom_sorting') {
        return null;
    }
    
    //Get array with offer ID list for your custom sorting
    $arElementIDList = ...;
    
    return $arElementIDList;
});
```

!> You need to add cache clearing for your custom sorting
```php
\Lovata\Shopaholic\Classes\Store\OfferListStore->sorting->clear('my_custom_sorting');
```