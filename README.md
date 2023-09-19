# react-note-taking-app
#### Video Demo: https://youtu.be/ZSft6AEBUJc
#### Live App: https://doganiwho-notes.netlify.app/

### Overview
This documentation provides an overview of a React-based note-taking application. The application allows users to create, edit, and manage notes with tags. It uses various React libraries, including React Router for navigation and React Bootstrap for styling.

### Table of Contents
1. **Dependencies**
2. **File Structure**
3. **Data Structures**
4. **Main Application Components**
5. **Functions and Handlers**
6. **Routes and Routing**
7. **Usage**

--- 

#### 1. Dependencies
- `bootstrap/dist/css/bootstrap.min.css`: CSS styles for Bootstrap.
- `react-bootstrap`: React components for Bootstrap.
- `react-router-dom`: Routing and navigation for React applications.
- `uuid`: A library for generating UUIDs.
- `useLocalStorage`: Custom hook for managing data in local storage.

#### 2. File Structure
- `NewNote.tsx`: Component for creating a new note.
- `useLocalStorage.ts`: Custom hook for managing data in local storage.
- `NoteList.tsx`: Component for displaying a list of notes.
- `NoteLayout.tsx`: Component for displaying a note layout.
- `Note.tsx`: Component for displaying a single note.
- `EditNote.tsx`: Component for editing a note.
- `App.tsx`: Main application file containing the root component.

#### 3. Data Structures
- `Note`: Represents a note with additional data properties.
- `RawNote`: Represents a raw note data structure.
- `RawNoteData`: Contains raw note data including title, markdown, and tag IDs.
- `NoteData`: Contains processed note data including title, markdown, and tags.
- `Tag`: Represents a tag with an ID and a label.

#### 4. Main Application Components
`App`: The root component of the application. It manages the overall structure of the app and handles note creation, updating, and deletion.

#### 5. Functions and Handlers
- `onCreateNote({ tags, ...data }: NoteData)`: Creates a new note and adds it to the list of notes.
- `onUpdateNote(id: string, { tags, ...data }`: NoteData): Updates an existing note.
- `onDeleteNote(id: string)`: Deletes a note by its ID.
- `addTag(tag: Tag)`: Adds a new tag to the list of tags.
- `updateTag(id: string, label: string)`: Updates the label of an existing tag.
- `deleteTag(id: string)`: Deletes a tag by its ID.

#### 6. Routes and Routing
- `/`: Displays the list of notes with associated tags and allows editing and deletion.
- `/new`: Provides a form to create a new note, including the ability to add tags.
- `/:id`: Displays a single note with options to edit and delete.
- `/edit`: Allows editing the content of the note and tags.

#### 7. Usage
To use this application, follow these steps:

1. Clone this repo and run `npm i`.
