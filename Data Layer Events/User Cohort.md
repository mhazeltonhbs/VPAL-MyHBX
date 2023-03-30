# User Cohort

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "user_cohort",
  "detailed_event": "User Cohort",
    "event_data": {
        "user_cohort": "<user_cohort>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.user_cohort|string|Datasource for User Cohort type||||||||




