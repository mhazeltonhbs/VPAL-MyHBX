# Form Submission Failed

### 


## Event Firing Instructions

<p><strong>Platform: myhbx</strong></p>
<p>Fire event when a form error occurs. This should be any 'friendly message' to the user.</p>


## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "form_error",
  "detailed_event": "Form Submission Failed",
    "event_data": {
        "error_message": "<error_message>",
        "name": "<name>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.error_message|string|Captures the form error code or message associated with form errors. Dynamic value. |Credit card declined, Required entries missing, EC3456, EC8976|||||||
|event_data.name|string|Captures the human-friendly name of the form. Dynamic value based on where the user is.|Payment Info|||||||

