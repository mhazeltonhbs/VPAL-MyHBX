# Article Loaded 2

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "article_loaded",
  "detailed_event": "Article Loaded 2",
    "event_data": {
        "article_length": <article_length>,
        "article_photo_content": <article_photo_content>,
        "article_video_content": <article_video_content>,
        "author_name": "<author_name>",
        "content_title": "<content_title>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.article_length|number|Datasource for Article Length||||||||
|event_data.article_photo_content|boolean|Datasource for Article Photo Content|true \| false|||||||
|event_data.article_video_content|boolean|Datasource for Article Video Content|true \| false|||||||
|event_data.author_name|string|Datasource for Author Name|john doe|||||||
|event_data.content_title|string|Datasource for Content Title||||||||




