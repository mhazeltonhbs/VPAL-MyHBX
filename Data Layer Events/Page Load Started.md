# Page Load Started

### 

## Event Firing Instructions

<p dir="auto"><span style="font-weight: 400;"><strong>Platform: myHBX</strong></span></p>
<p dir="auto">Fire whenever a user loads in a new page, whether that is done synchronously or asynchronously.</p>
<p dir="auto">This event should be the first pushed into the data layer on each page. Given many 3rd party scripts push events to the data layer, this event push should be placed in the page&nbsp;<code>&lt;head&gt;</code>&nbsp;and should be the first&nbsp;<code>&lt;script&gt;</code>&nbsp;tag on the page to ensure it is the first event.</p>
<p dir="auto">There is no longer a concept of virtual page view, so this event should be fired whenever a virtual page view would have been fired in the past, such as when a new screen is loaded asyncronously within an angular, react, or vue app/embed.</p>


## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ page_data: null });  // Clear the previous page_data object.
dataLayer.push({
  "event": "page_load_started",
  "detailed_event": "Page Load Started",
    "page_data": {
        "page_location": "<page_location>",
        "page_title": "<page_title>"
    },
    "user_data": {
        "user_id": "<user_id>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|page_data.page_location|string|The URL of the page currently being viewed. This value will include the full, unaltered URL of the page\/screen the user is currently viewing, including query parameters, fragments, etc., Dynamic value.|https:\/\/account.myhbx.org\/MyDashboard?qs=WGv%2FaZjTzzPGEvkiut1CsBhX8d%2BXHx0NHS0TLxw1ErE%3D|||||||
|page_data.page_title|string|The title of the page currently being viewed, generally available in &lt;title&gt;. Dynamic value.|HBS Online - My Dashboard|||||||
|user_data.user_id|string|The id of the user currently logged in to the site, if the site offers authentication and the user is authenticated. Dynamic value.|123456|||||||

