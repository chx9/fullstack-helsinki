```mermaid
sequenceDiagram
    participant browser
    participant server

    Note right of browser: add to notes array and re-render page
    
    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server

    Note left of server: The server add note to it's notes array

    server-->>browser: successful message
    deactivate server

```