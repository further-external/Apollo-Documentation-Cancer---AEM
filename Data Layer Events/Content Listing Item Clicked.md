# Content Listing Item Clicked

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  event: 'select_content',
  detailed_event: "Content Listing Item Clicked",
  event_data: {
    identifier: "<identifier>", // REQUIRED | string | ex. 12345abcde12345
    name: "<name>", // recommended | string | ex.  What Is Cancer?	
    content_list_name: "<content_list_name>", // recommended | string | ex.  Cancer A-Z	
    index: "<index>", // recommended | integer | ex. 1 | min. lgth. 1 | min. 1
    target_index: "<target_index>" // recommended | integer | ex. 2 | min. lgth. 1 | min. 1 
  }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|identifier|string|required|The computer-readable machine name of the carousel. Use UUID provided by the component|12345abcde12345|
|name|string|recommended|The human-readable name of the carousel. If user does not input one, populate with numerical index of which carousel this is on the page (1-indexed)| What Is Cancer?|
|name|string|recommended|The human-readable name of the content list. If user does not input one, populate with numerical index of which list this is on the page (1-indexed)| Cancer A-Z|
|index|integer|recommended|The slide # the carousel is on at time of interaction (1-indexed)|1||1||1
|target_index|integer|recommended|The slide # of the target slide (1-indexed)|2||1||1|




