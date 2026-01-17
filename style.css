const API_URL = "http://localhost:8080/api/notes";

function loadNotes() {
    fetch(API_URL)
        .then(res => res.json())
        .then(notes => {
            const notesDiv = document.getElementById("notes");
            notesDiv.innerHTML = "";

            notes.forEach(note => {
                const div = document.createElement("div");
                div.className = "note";
               div.innerHTML = `
                   <div class="note-header">
                       <h3>${note.title}</h3>
                       <button class="delete-btn" onclick="deleteNote(${note.id})">✕</button>
                   </div>
                   <p class="note-content">${note.content}</p>
               `;

                notesDiv.appendChild(div);
            });
        });
}

function addNote() {
    const title = document.getElementById("title").value;
    const content = document.getElementById("content").value;

    fetch(API_URL, {
        method: "POST",
        headers: { "Content-Type": "application/json" },
        body: JSON.stringify({ title, content })
    }).then(() => {
        document.getElementById("title").value = "";
        document.getElementById("content").value = "";
        loadNotes();
    });
}

function deleteNote(id) {
    fetch(`${API_URL}/${id}`, { method: "DELETE" })
        .then(() => loadNotes());
}

loadNotes();
