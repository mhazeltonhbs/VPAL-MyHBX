# User Registered

### 

## Event Firing Instructions

<p><strong>Platform: myhbx</strong></p>
<p>This event should fire when the user creates an account (just account creation, not validation step)</p>
<p>Fire on this page: https://account.myhbx.org/SignUpConfirmation </p>

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "sign_up",
  "detailed_event": "User Registered",
    "event_data": {
        "method": ""
    },
    "user_data": {
        "user_id": "<user_id>",
        "user_type": ""
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.method|string|Left blank for future use.||||||||
|user_data.user_id|string|The id of the user currently logged in to the site, if the site offers authentication and the user is authenticated.|123456, abc123|||||||
|user_data.user_type|string|Left blank for future use.||||||||



