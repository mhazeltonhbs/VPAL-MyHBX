# Course Application - Select Cohort

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "course_application_select_cohort",
  "detailed_event": "Course Application - Select Cohort",
    "event_data": {
        "user_cohort": "<user_cohort>",
        "course_application_step": "Step 1",
        "name": "Select Wave"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.user_cohort|string|The date\/price selected from the available cohort list during the initial application process. Dynamic value. |May 10, 2023 - Fee: $1600|||||||
|event_data.course_application_step|string|Datasource for Application Step Name. Static value. |Step 1|||||||
|event_data.name|string|Captures the human-friendly name of the form. Static value.|Select Wave|||||||

## Attached Notes

<p><strong>Platform: myhbx</strong></p>
<p>This event fires when a a user selects and suscessfully submits a 'cohort' (date) in the course application flow. (step1)</p>
<p>Fires on: https://account.myhbx.org/SelectWave</p>

