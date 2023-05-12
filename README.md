# VPAL

<h1 id="overview"><strong>Overview</strong></h1>
<p>This repository contains the necessary specifications to add additional data layers for use with Google Tag Manager and Google Analytics 4.</p>
<p>All ecommerce definitions are defined in via the data layer code in this repo.</p>
<p>Additional documentation from Google for ecommerce definitions: <a href="https://developers.google.com/analytics/devguides/collection/ga4/ecommerce?client_type=gtm">https://developers.google.com/analytics/devguides/collection/ga4/ecommerce?client_type=gtm</a></p>
<p>&nbsp;</p>
<h2 id="data-layer">Data Layer</h2>
<p>Each file inside the events folder corresponds to a single use case or site event that needs to be implemented. These events are leveraged to trigger tracking rules in the tag management tool of choice and share data with the analytics reporting tool.</p>
<p>As the data layer is event-based, the order in which the events are fired is critical. In general, events should be pushed onto the data layer in the following sequence when a page load (virtual or otherwise) occurs:</p>
<p>Page Load Started &gt; <em>Other Page-level Events</em> &gt; Page Load Completed</p>
<p>If an Event is part of the page load sequence, it will be indicated in the corresponding event file.</p>
<p>Events that occur outside of the page load sequence should be pushed onto the data layer as they occur.</p>
