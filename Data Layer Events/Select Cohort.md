# Select Cohort

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "select_cohort",
  "detailed_event": "Select Cohort",
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

<p><span style="font-weight: 400;"><strong>Platform: harvardonline</strong></span></p>
<p><span style="font-weight: 400;">Trigger this event when a user has successfully selected a cohort.</span></p>
<p><span style="font-weight: 400;">Example page: </span><a href="https://account.myhbx.org/SelectWave"><span style="font-weight: 400;">https://account.myhbx.org/SelectWave</span></a><span style="font-weight: 400;">&nbsp;</span></p>
