# Course List Displayed

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "course_listing",
  "detailed_event": "Course List Displayed",
    "event_data": {
        "course_list_category": "<course_list_category>",
        "course_list_name": "<course_list_name>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.course_list_category|string|Datasource of Category \(course list\)||||||||
|event_data.course_list_name|string|Datasource. for Course List Name||||||||




