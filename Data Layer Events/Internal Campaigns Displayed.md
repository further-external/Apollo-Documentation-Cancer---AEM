# Internal Campaigns Displayed

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ ecommerce: null });  // Clear the previous ecommerce object.
dataLayer.push({
  "event": "view_promotion",
  "detailed_event": "Internal Campaigns Displayed",
    "ecommerce": {
        "creative_name": "<creative_name>",
        "creative_slot": "<creative_slot>",
        "items": [
            {
                "item_id": "<item_id>",
                "item_name": "<item_name>",
                "location_id": "<location_id>"
            }
        ],
        "promotion_name": "<promotion_name>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|ecommerce.creative_name|string|Captures the internal campaign creative associated with internal campaigns. Used for internal campaign impressions and clicks only.|Girl with bike, Mountain Top, River Cruise Danube|||||||
|ecommerce.creative_slot|string|Captures the position of an internal campaign on a website page or mobile app screen. Used for internal campaign impressions and clicks only.|1, 5, 78, 3||||1|||
|ecommerce.items[n].item_id|string|Item ID \(context-specific\).The product primary ID \(SKU or UPC\)|SKU\_12345|||||||
|ecommerce.items[n].item_name|string|Item Name \(context-specific\).|jeggings|||||||
|ecommerce.items[n].location_id|string|Captures a unique ID of a physical location such as a store, banking branch, atm, hotel, office, or other.|155, 65588, 987764448|||||||
|ecommerce.promotion_name|string|Captures the name associated with internal campaigns. Used for internal campaign impressions and clicks only.|Trek bikes for kids, REI Spring Sale 2019, Viking Cruise Fall Specials|||||||




