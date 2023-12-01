```mermaid
sequenceDiagram
browser->>server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/spa
server->>browser: return spa
server->>browser: return main.css
server->>browser: return spa.js
server-->browser: return data.json
```
