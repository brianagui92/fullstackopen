New note in single page app diagram

```mermaid

sequenceDiagram
    participant browser
    participant server

    Note right of browser: The browser starts executing the JavaScript code that adds the note to the list, redraws the list and sends the note to the server

    browser->>server: GET https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: note created
    deactivate server
```