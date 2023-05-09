# Course Application

### 

## Event Firing Instructions

<p><strong>Platform: myhbx</strong></p>
<p>This event fires when the user starts the 'personal information' application flow step. This event should only be fire once per page request. (step2)</p>
<p>Fires on page load: https://account.myhbx.org/MyApplication </p>

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "course_application",
  "detailed_event": "Course Application",
    "event_data": {
        "user_cohort": "<user_cohort>",
        "course_application_step": "Step 2",
        "name": "Personal Information"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.user_cohort|string|The date\/price selected from the available cohort list during the initial application process. Dynamic value. |May 10, 2023 - Fee: $1600|||||||
|event_data.course_application_step|string|Datasource for Application Step Name. Static Value.|Step 2|||||||
|event_data.name|string|Captures the human-friendly name of the form. Static Value.|Personal Information|||||||



