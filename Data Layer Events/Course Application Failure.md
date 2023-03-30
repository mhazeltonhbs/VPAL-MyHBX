# Course Application Failure

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "course_application_error",
  "detailed_event": "Course Application Failure",
    "event_data": {
        "course_name": "<course_name>",
        "error_message": "<error_message>",
        "name": "<name>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.course_name|string|Datasource for Course Name||||||||
|event_data.error_message|string|Captures the form error code or message associated with form errors.|Credit card declined, Required entries missing, EC3456, EC8976|||||||
|event_data.name|string|Captures the human-friendly name of the form.|Payment Info, Mailing Address, Payment Address, Contact Us|||||||




