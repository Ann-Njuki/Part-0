```mermaid
sequenceDiagram
  participant browser as browser
  participant server as server

  browser->>server:GET https://studies.cs.helsinki.fi/exampleapp/spa
  activate server
  server-->>browser:The HTML Document of spa
  deactivate server

  browser->>server:GET https://studies.cs.helsinki.fi/exampleapp/spa
  activate server
  server-->>browser: The CSS file of spa
  deactivate server

  browser->>server:GET https://studies.cs.helsinki.fi/exampleapp/spa.js
  activate server
  server-->>browser: The javascript file of spa
  deactivate server

```
