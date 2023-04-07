# Page Load Completed

### Page Load Completed is part of the page load sequence, including virtual page loads in the case of single page apps, and must be the last event pushed in the page load event sequence.

## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({
  "event": "page_view",
  "detailed_event": "Page Load Completed"
});
```





## Attached Notes

<p><span style="font-weight: 400;"><strong>Platform: BOTH</strong></span></p>
<p><span style="font-weight: 400;">Trigger this event when data from the data layer has completely propagated and the payload is ready to deploy. This helps prevent race conditions that could occur when using data from multiple events that load on a single page load (see the </span><em><span style="font-weight: 400;">Article Loaded</span></em><span style="font-weight: 400;"> event).</span></p>
<p><span style="font-weight: 400;">Example page:</span></p>
<p><a href="https://www.harvardonline.harvard.edu/series/harvard-on-digital"><span style="font-weight: 400;">https://www.harvardonline.harvard.edu</span></a></p>
