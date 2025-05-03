```mermaid 
sequenceDiagram 
participant browser 
participant server 

browser->>server: POST https://studies.cs.helsinki.fi/exampleapp/new_note_spa<br>with JSON payload 
activate server 
server-->>browser: Response 201 Created 
deactivate server 

Note right of browser: JavaScript updates the notes list on the page<br>without reloading 
```