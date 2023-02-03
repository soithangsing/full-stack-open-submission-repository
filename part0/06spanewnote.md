```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    browser->>server: {"content": "new note ","date": "2023-02-03T14:24:52.993Z"}
    Note right of browser: content-type: application/json

    activate server
    server-->>browser: Status Code: 🟢 201 Created
    deactivate server sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    browser->>server: {"content": "new note ","date": "2023-02-03T14:24:52.993Z"}
    Note right of browser: content-type: application/json

    activate server
    server-->>browser: Status Code: 🟢 201 Created
    deactivate server
```
