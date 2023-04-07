# Form Submission Failed

### 

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
|event_data.error_message|string|Captures the form error code or message associated with form errors.|Credit card declined, Required entries missing, EC3456, EC8976|||||||
|event_data.name|string|Captures the human-friendly name of the form.|Payment Info, Mailing Address, Payment Address, Contact Us|||||||

## Attached Notes

<p><span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;https://vpal.harvard.edu/make-a-course\nclicks on CTAs or Nav Clicks to either Make a course OR Courses list&quot;}" data-sheets-userformat="{&quot;2&quot;:1049345,&quot;3&quot;:{&quot;1&quot;:0},&quot;11&quot;:4,&quot;12&quot;:0,&quot;23&quot;:1}" data-sheets-textstyleruns="{&quot;1&quot;:0,&quot;2&quot;:{&quot;2&quot;:{&quot;1&quot;:2,&quot;2&quot;:1136076},&quot;9&quot;:1}}{&quot;1&quot;:39}" data-sheets-hyperlinkruns="{&quot;1&quot;:0,&quot;2&quot;:&quot;https://vpal.harvard.edu/make-a-course&quot;}{&quot;1&quot;:39}"><strong>Platform: both</strong></span></p>
<p>Fire event when a form error occurs. This should be any 'friendly message' to the user.</p>
