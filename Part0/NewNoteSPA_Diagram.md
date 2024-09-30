```mermaid
sequenceDiagram
    participant browser
    participant server

    browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    server-->>browser: Note Content
    deactivate server

     Note right of browser: There is more that happens on the browser. 
     Note right of browser:  Such as adding the note locally and rerendering the page. I did not show that here.

```