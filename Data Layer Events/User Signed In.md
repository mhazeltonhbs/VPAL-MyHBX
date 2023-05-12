# User Signed In

### 

## Event Firing Instructions

<p><strong>Platform: myhbx</strong></p>
<p>Trigger this event when a user has successfully signed into their account.</p>
<p>Example page:<br />https://login.myhbx.org/login?service=https%3A%2F%2Fadmin.myhbx.org%2Fsso&amp;PC=DSRY&amp;hbssrc=vpal&amp;_ga=2.173678115.1213328162.1680195742-1854174576.1669999120&amp;bsrc=https%3A%2F%2Fwww.harvardonline.harvard.edu%2F&nbsp;</p>

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ page_data: null });  // Clear the previous page_data object.
dataLayer.push({
  "event": "login",
  "detailed_event": "User Signed In",
    "page_data": {
        "user_login_state": "signed_in"
    },
    "user_data": {
        "user_id": "<user_id>",
        "user_type": "Customer"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|page_data.user_login_state|string|Captures the current sign in status for the user - static value for MyHBX|signed_in|||||||
|user_data.user_id|string|The id of the user currently logged in to the site, if the site offers authentication and the user is authenticated. Dynamic value. |123456, abc123|||||||
|user_data.user_type|string|Captures the type associated with the user. Static value.|Customer|||||||


