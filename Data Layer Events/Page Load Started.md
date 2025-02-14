# Page Load Started

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ page_data: null });  // Clear the previous page_data object.
dataLayer.push({
  "event": "page_load_started",
  "detailed_event": "Page Load Started",
    "page_data": {
        "breadcrumb": "<breadcrumb>",
        "country": "<country>",
        "language": "<language>",
        "name": "<name>",
        "page_location": "<page_location>",
        "page_path": "<page_path>",
        "release_version": "<release_version>",
        "site_name": "<site_name>",
        "site_section": "<site_section>",
        "site_section2": "<site_section2>",
        "site_variant": "<site_variant>",
        "type": "<type>",
        "system_environment": "<system_environment>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|page_data.breadcrumb|string|A delimited list of hierarchical sections that describe the current page's location within the navigation of the site.|Home&gt;Women&gt;Tops&gt;Sweaters, Mens - Tops - Sweaters - Supmina, Wool, Rayon, Checkout &gt; Order Thank You|||||||
|page_data.country|string|The country the site is associated with.||||||||
|page_data.language|string|The language of the current page, usually pulled from the &lt;html&gt; tag lang attribute.||||||||
|page_data.name|string|Captures the name of the page the user is on|product - XYZ123, Mens - Tops - Sweaters, Order Confirmation|||||||
|page_data.page_location|string|The url of the page currently being viewed.||||||||
|page_data.page_path|string|Captures the path portion of the page URL.||||||||
|page_data.release_version|string|Captures the version number of the release active on the site||||||||
|page_data.site_name|string|Common language used within the business to refer to the website. May be specific County Sites.|Prospecting-EU, Prospecting-US, Member Portal, Shop-CA, Shop-US, Shop-EU|||||||
|page_data.site_section|string|The section of the site that the current page resides in. site\_section2 through site\_section5can also be used if the site has many sections.||||||||
|page_data.site_section2|string|Captures the sub-section of the site where the page being viewed is located|Shop &gt; Kids, Shop &gt; Mens, Shop &gt; Womens|||||||
|page_data.site_variant|string|Describes the version of the site that is being shown|Responsive, Mobile, Desktop|||||||
|page_data.type|string|The type of page currently viewed.|home, pdp, article|||||||
|page_data.system_environment|string|The environment type of the site, is used to distinguish between product and non-production activity.|production, non-production|||||||





