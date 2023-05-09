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
        "course_application_step": "Step 3",
        "name": "Application Submission"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.course_application_step|string|Datasource for Application Step Name. Static value.| Step 3|||||||
|event_data.name|string|Captures the human-friendly name of the form. Static value.|Application Submission|||||||

## Attached Notes

<p><strong>Platform: myhbx</strong></p>
<p>This event fires when the course application is successfully submitted. (step3)</p>
