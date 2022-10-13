# Donation Completed

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  "event": "purchase",
  "detailed_event": "Donation Completed",
    "ecommerce": {
        "currency": "<currency>",
        "items": [
            {
                "affiliation": "<affiliation>",
                "currency": "<currency>",
                "item_id": "<item_id>",
                "item_name": "<item_name>"
            }
        ],
        "payment_frequency": "<payment_frequency>",
        "payment_method": "<payment_method>",
        "postal_code": "<postal_code>",
        "state_province": "<state_province>",
        "transaction_id": "<transaction_id>",
        "type": "<type>",
        "value": <value>
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|ecommerce.currency|string|The currency, in 3-letter ISO 4217 format.||||||||
|ecommerce.items[n].affiliation|string|A product affiliation to designate a supplying company or brick and mortar store location.|Google Store|||||||
|ecommerce.items[n].currency|string|The currency, in 3-letter ISO 4217 format.|USD|||||||
|ecommerce.items[n].item_id|string|Item ID \(context-specific\).The product primary ID \(SKU or UPC\)|SKU\_12345|||||||
|ecommerce.items[n].item_name|string|Item Name \(context-specific\).|jeggings|||||||
|ecommerce.payment_frequency|string|Captures the recurring frequency of donation \(i.e. one-time, monthly\).|One Time, Monthly|||||||
|ecommerce.payment_method|string|Captures the payment methods used for a transaction \(i.e. credit card, Visa, MasterCard, Amex, Paypal, purchase order, etc\).|Credit Card, PayPal, Mastercard, Visa, Amex, Discover|||||||
|ecommerce.postal_code|string|Captures the postal code associated with a transaction \(i.e. order, booking, dontation, etc.\).|53533, 30381, M1R 0E9, M3C 0C1|||||||
|ecommerce.state_province|string|Captures the state or province associated with payments used for a transaction \(i.e. order, booking, dontation, etc.\).|WI, GA, NB, ON|||||||
|ecommerce.transaction_id|string|The unique identifier of a transaction.|T\_12345, 19283j2nm9jdjs|^[a-zA-Z0-9]{6,20}$|6|20||||
|ecommerce.type|string|Captures the type of donation made \(i.e. general, tribute\).|Tribute, General, Fundraiser|||||||
|ecommerce.value|number|The monetary value of the event.|7.77, 239.55, 659|||||||




