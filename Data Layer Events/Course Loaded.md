# Course Loaded

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "course_loaded",
  "detailed_event": "Course Loaded",
    "event_data": {
        "course_availabilty": "<course_availabilty>",
        "course_certificate_price": "<course_certificate_price>",
        "course_difficulty": "<course_difficulty>",
        "course_language": "<course_language>",
        "course_length": "<course_length>",
        "course_modality": "<course_modality>",
        "course_name": "<course_name>",
        "course_pace": "<course_pace>",
        "course_platform": "<course_platform>",
        "course_price": "<course_price>",
        "course_promo_name": "<course_promo_name>",
        "course_school": "<course_school>",
        "course_transcript_language": "<course_transcript_language>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.course_availabilty|string|Datasource for Course Availability||||||||
|event_data.course_certificate_price|string|Datasource for Course Certificate Price||||||||
|event_data.course_difficulty|string|Datasource for Course Difficulty||||||||
|event_data.course_language|string|Datasource for Course Language||||||||
|event_data.course_length|string|Datasource for Course Length||||||||
|event_data.course_modality|string|Datasource for Course Modality||||||||
|event_data.course_name|string|Datasource for Course Name||||||||
|event_data.course_pace|string|Datasource for Course Pace||||||||
|event_data.course_platform|string|Datasource for Course Platform||||||||
|event_data.course_price|string|Datasource for Course Price||||||||
|event_data.course_promo_name|string|Datasource for Course Promotion Name||||||||
|event_data.course_school|string|Datasource for Course School||||||||
|event_data.course_transcript_language|string|Datasource for Course Transcript Language||||||||




