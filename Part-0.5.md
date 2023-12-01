sequenceDiagram
browser->>server: HTTP GET https://studies.cs.helsinki.fi/exampleapp/spa
server->>browser: return spa
server->>browser: return main.css
server->>browser: return spa.js
server-->browser: return data.json
browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
server->>browser: response header
Note right of browser: Object { content: "hello", date: "2023-11-28 14:25:37" }
