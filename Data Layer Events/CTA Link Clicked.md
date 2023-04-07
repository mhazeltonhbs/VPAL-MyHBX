# CTA Link Clicked

### 

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({ event_data: null });  // Clear the previous event_data object.
dataLayer.push({
  "event": "click",
  "detailed_event": "CTA Link Clicked",
    "event_data": {
        "identifier": "<identifier>",
        "region_ancestry": "<region_ancestry>"
    }
});
```

## Variable Definitions

|Path|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|event_data.identifier|string|Captures the ID associated with CTA links used.|act now, cancel, ok, 3456, 8765|||||||
|event_data.region_ancestry|string|Captures the name or ID of the region within which CTA links are used.|Top Nav, Footer Nav, Hero, Recommended, Also Shopped, Also Bought|||||||

## Attached Notes

<p><span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;https://vpal.harvard.edu/make-a-course\nclicks on CTAs or Nav Clicks to either Make a course OR Courses list&quot;}" data-sheets-userformat="{&quot;2&quot;:1049345,&quot;3&quot;:{&quot;1&quot;:0},&quot;11&quot;:4,&quot;12&quot;:0,&quot;23&quot;:1}" data-sheets-textstyleruns="{&quot;1&quot;:0,&quot;2&quot;:{&quot;2&quot;:{&quot;1&quot;:2,&quot;2&quot;:1136076},&quot;9&quot;:1}}{&quot;1&quot;:39}" data-sheets-hyperlinkruns="{&quot;1&quot;:0,&quot;2&quot;:&quot;https://vpal.harvard.edu/make-a-course&quot;}{&quot;1&quot;:39}"><strong>Platform: harvardonline</strong></span></p>
<p><span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;https://vpal.harvard.edu/make-a-course\nclicks on CTAs or Nav Clicks to either Make a course OR Courses list&quot;}" data-sheets-userformat="{&quot;2&quot;:1049345,&quot;3&quot;:{&quot;1&quot;:0},&quot;11&quot;:4,&quot;12&quot;:0,&quot;23&quot;:1}" data-sheets-textstyleruns="{&quot;1&quot;:0,&quot;2&quot;:{&quot;2&quot;:{&quot;1&quot;:2,&quot;2&quot;:1136076},&quot;9&quot;:1}}{&quot;1&quot;:39}" data-sheets-hyperlinkruns="{&quot;1&quot;:0,&quot;2&quot;:&quot;https://vpal.harvard.edu/make-a-course&quot;}{&quot;1&quot;:39}">Fire this event when a user clicks on a specific navigation or CTA link to ether 'Make a Course' page or a 'List of Courses'</span></p>
<p><span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;https://vpal.harvard.edu/make-a-course\nclicks on CTAs or Nav Clicks to either Make a course OR Courses list&quot;}" data-sheets-userformat="{&quot;2&quot;:1049345,&quot;3&quot;:{&quot;1&quot;:0},&quot;11&quot;:4,&quot;12&quot;:0,&quot;23&quot;:1}" data-sheets-textstyleruns="{&quot;1&quot;:0,&quot;2&quot;:{&quot;2&quot;:{&quot;1&quot;:2,&quot;2&quot;:1136076},&quot;9&quot;:1}}{&quot;1&quot;:39}" data-sheets-hyperlinkruns="{&quot;1&quot;:0,&quot;2&quot;:&quot;https://vpal.harvard.edu/make-a-course&quot;}{&quot;1&quot;:39}">Example Page: (any link cta or nav to -&gt;) </span><span data-sheets-value="{&quot;1&quot;:2,&quot;2&quot;:&quot;https://vpal.harvard.edu/make-a-course\nclicks on CTAs or Nav Clicks to either Make a course OR Courses list&quot;}" data-sheets-userformat="{&quot;2&quot;:1049345,&quot;3&quot;:{&quot;1&quot;:0},&quot;11&quot;:4,&quot;12&quot;:0,&quot;23&quot;:1}" data-sheets-textstyleruns="{&quot;1&quot;:0,&quot;2&quot;:{&quot;2&quot;:{&quot;1&quot;:2,&quot;2&quot;:1136076},&quot;9&quot;:1}}{&quot;1&quot;:39}" data-sheets-hyperlinkruns="{&quot;1&quot;:0,&quot;2&quot;:&quot;https://vpal.harvard.edu/make-a-course&quot;}{&quot;1&quot;:39}"><a class="in-cell-link" href="https://vpal.harvard.edu/make-a-course" target="_blank" rel="noopener">https://vpal.harvard.edu/make-a-course<br /></a><br /></span></p>
