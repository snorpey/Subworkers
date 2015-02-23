# Subworkers
WebWorkers are awesome! Unfortionately, Google Chrome doesn't support creating subworkers,
[here's the Chromium issue for it](https://code.google.com/p/chromium/issues/detail?id=31666).

This polyfill provides this functionality to Chrome and any other browser that supports WebWorkers,
but now subworkers.

## Usage
Using this is easy!

1. Download [`subworkers.js`](https://raw.githubusercontent.com/dmihal/Subworkers/master/subworkers.js)
2. In the document hosting the WebWorkers, include the `subworkers.js` script before

   ``` html
   <script src="subworkers.js"></script>
   ```

3. In the code for any WebWorker that will have a subworker, you also need to include `subworkers.js`

   ``` javascript
   importScripts("subworkers.js");
   ```

That's it! WebWorkers now work the way you would expect!

