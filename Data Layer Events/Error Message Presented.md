# Error Message Presented

### 

## Event Firing Instructions

<p><strong>Platform: myhbx</strong></p>
<p>Fire when an error message is displayed on MyHBX, such as form validation errors. This should be any 'friendly message' to the user.</p>

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({
  "event": "site_error",
  "detailed_event": "Error Message Presented",
  "event_data": {
        "error_message": "<error_message>",
        "name": "<name>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.error_message|string|Captures the error message associated with any on-page errors. Dynamic value. |First Name is required|||||||
|event_data.name|string|Captures the human-friendly name of the form. Dynamic value based on where the user is.|Application Submission|||||||






