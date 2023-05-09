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
        "user_cohort": "<user_cohort>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.user_cohort|string|The date\/price selected from the available cohort list during the initial application process.|May 10, 2023 - Fee: $1600|||||||

## Attached Notes

<p><strong>Platform: myhbx</strong></p>
<p>This event fires when a a user selects and suscessfully submits a 'cohort' (date) in the course application flow. (step1)</p>
<p>Fires on: https://account.myhbx.org/SelectWave</p>

