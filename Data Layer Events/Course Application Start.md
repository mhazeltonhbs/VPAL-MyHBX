# Course Application Start

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "course_application_start",
  "detailed_event": "Course Application Start",
    "event_data": {
        "course_application_step": "<course_application_step>",
        "course_availabilty": "<course_availabilty>",
        "course_difficulty": "<course_difficulty>",
        "course_language": "<course_language>",
        "course_length": "<course_length>",
        "course_modality": "<course_modality>",
        "course_platform": "<course_platform>",
        "course_school": "<course_school>",
        "course_transcript_language": "<course_transcript_language>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.course_application_step|string|Datasource for Application Step Name||||||||
|event_data.course_availabilty|string|Datasource for Course Availability||||||||
|event_data.course_difficulty|string|Datasource for Course Difficulty||||||||
|event_data.course_language|string|Datasource for Course Language||||||||
|event_data.course_length|string|Datasource for Course Length||||||||
|event_data.course_modality|string|Datasource for Course Modality||||||||
|event_data.course_platform|string|Datasource for Course Platform||||||||
|event_data.course_school|string|Datasource for Course School||||||||
|event_data.course_transcript_language|string|Datasource for Course Transcript Language||||||||




