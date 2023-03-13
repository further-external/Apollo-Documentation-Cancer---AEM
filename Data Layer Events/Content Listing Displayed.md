# Content Listing Displayed

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  event: 'view_content_list',
  detailed_event: "Content Listing Displayed",
  event_data: {
    identifier: "<identifier>", // REQUIRED | string | ex. 12345abcde12345
    name: "<name>", // recommended | string | ex. Most Popular Blog Posts, 2	
  }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|identifier|string|required|The computer-readable machine name of the carousel. Use UUID provided by the component|12345abcde12345|
|name|string|recommended|The human-readable name of the carousel. If user does not input one, populate with numerical index of which carousel this is on the page (1-indexed)|Cancer A-Z|




