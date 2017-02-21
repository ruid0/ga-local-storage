# ga-local-storage
Google Analytics for Electron app

Modified version of [GALocalstorage](https://github.com/ggendre/GALocalStorage)

## Installation

```bash
npm install ga-local-storage@1.0.0 --save 
```

## How to use

```js
<script>
  const gaStorage = require('ga-local-storage');
  gaStorage.setAccount('UA-XXXXXXXX-1'); //Replace with your own
  gaStorage.trackPageView('/index.html');
</script>
```
Then in your renderer you can track page view and events

```js
  gaStorage.trackPageView('/login', 'optional title');
  gaStorage.trackEvent('category', 'action', 'label', 'value');
```