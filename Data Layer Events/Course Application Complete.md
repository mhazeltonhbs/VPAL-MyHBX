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
        "user_cohort": "<user_cohort>",
        "course_application_step": "Step 3",
        "name": "Application Submission"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.user_cohort|string|The date\/price selected from the available cohort list during the initial application process. Dynamic value. |May 10, 2023 - Fee: $1600|||||||
|event_data.course_application_step|string|Datasource for Application Step Name. Static value.| Step 3|||||||
|event_data.name|string|Captures the human-friendly name of the form. Static value.|Application Submission|||||||

## Attached Notes

<p><strong>Platform: myhbx</strong></p>
<p>This event fires when the course application is successfully submitted. (step3)</p>
