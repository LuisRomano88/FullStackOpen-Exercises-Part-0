```mermaid
sequenceDiagram
browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_notes
server-->>browser: return HTTP 302
browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/notes
server->>browser: return https://studies.cs.helsinki.fi/main.css
server->>browser: return https://studies.cs.helsinki.fi/main.js
server->>browser: return https://studies.cs.helsinki.fi/data.json
browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note
Note right of server: crea un nuevo objeto
Note right of server: Object { content: "hello", date: "2023-11-28 14:25:37" }
```

