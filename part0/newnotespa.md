note over browser:
user submits new note
end note

browser->server: HTTP POST https://fullstack-exampleapp.herokuapp.com/new_note_spa
server-->browser: HTTP code 201 created
note over server:
server receives JSON object
event handler creates a new note,
adds it to the notes list with the command notes.push(note),
re-renders the note list on the page
and sends the new note to the server.
end note
