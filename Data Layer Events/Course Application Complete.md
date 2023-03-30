# Course Application Complete

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "course_application_complete",
  "detailed_event": "Course Application Complete",
    "event_data": {
        "course_application_step": "<course_application_step>",
        "course_availabilty": "<course_availabilty>",
        "course_certificate_price": "<course_certificate_price>",
        "course_difficulty": "<course_difficulty>",
        "course_language": "<course_language>",
        "course_modality": "<course_modality>",
        "course_pace": "<course_pace>",
        "course_platform": "<course_platform>",
        "course_price": "<course_price>",
        "course_school": "<course_school>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.course_application_step|string|Datasource for Application Step Name||||||||
|event_data.course_availabilty|string|Datasource for Course Availability||||||||
|event_data.course_certificate_price|string|Datasource for Course Certificate Price||||||||
|event_data.course_difficulty|string|Datasource for Course Difficulty||||||||
|event_data.course_language|string|Datasource for Course Language||||||||
|event_data.course_modality|string|Datasource for Course Modality||||||||
|event_data.course_pace|string|Datasource for Course Pace||||||||
|event_data.course_platform|string|Datasource for Course Platform||||||||
|event_data.course_price|string|Datasource for Course Price||||||||
|event_data.course_school|string|Datasource for Course School||||||||




