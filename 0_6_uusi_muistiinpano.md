sequenceDiagram
    participant browser
    participant server
    
    Note right of browser: The browser starts executing the JavaScript code that fetches the JSON from the server
    
    browser->>server: POST  {content:"juu u", date: "2023-22-08T14:39:09.923Z"} https://studies.cs.helsinki.fi/exampleapp/new_note_spa
    activate server
    browser-->>server: {"message":"note created"}
    deactivate server    

    Note right of browser: The browser executes the callback function that renders the notes 
