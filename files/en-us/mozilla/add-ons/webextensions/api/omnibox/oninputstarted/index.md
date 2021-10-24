---
title: omnibox.onInputStarted
slug: Mozilla/Add-ons/WebExtensions/API/omnibox/onInputStarted
tags:
  - API
  - Add-ons
  - Event
  - Extensions
  - Reference
  - WebExtensions
  - omnibox
  - onInputStarted
browser-compat: webextensions.api.omnibox.onInputStarted
---
<div>{{AddonSidebar()}}</div>

<p>Fired when the user starts interacting with your extension by entering its keyword in the address bar and then pressing the space key.</p>

<p>This will be sent before any {{WebExtAPIRef("omnibox.onInputChanged")}} events.</p>

<h2 id="Syntax">Syntax</h2>

<pre class="brush:js">browser.omnibox.onInputStarted.addListener(listener)
browser.omnibox.onInputStarted.removeListener(listener)
browser.omnibox.onInputStarted.hasListener(listener)
</pre>

<p>Events have three functions:</p>

<dl>
 <dt><code>addListener(callback)</code></dt>
 <dd>Adds a listener to this event.</dd>
 <dt><code>removeListener(listener)</code></dt>
 <dd>Stop listening to this event. The <code>listener</code> argument is the listener to remove.</dd>
 <dt><code>hasListener(listener)</code></dt>
 <dd>Check whether <code>listener</code> is registered for this event. Returns <code>true</code> if it is listening, <code>false</code> otherwise.</dd>
</dl>

<h2 id="addListener_syntax">addListener syntax</h2>

<h3 id="Parameters">Parameters</h3>

<dl>
 <dt><code>callback</code></dt>
 <dd>
 <p>Function that will be called when this event occurs. The function will be passed no arguments.</p>
 </dd>
</dl>

<h2 id="Browser_compatibility">Browser compatibility</h2>

<p>{{Compat}}</p>

<h2 id="Examples">Examples</h2>

<pre class="brush: js">browser.omnibox.onInputStarted.addListener(() =&gt; {
  console.log("User has started interacting with me.")
});
</pre>

<p>{{WebExtExamples}}</p>


<div class="note"><p><strong>Note:</strong> This API is based on Chromium's <a href="https://developer.chrome.com/extensions/omnibox"><code>chrome.omnibox</code></a> API.</p>

<p>Microsoft Edge compatibility data is supplied by Microsoft Corporation and is included here under the Creative Commons Attribution 3.0 United States License.</p>
</div>