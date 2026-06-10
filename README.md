# To-Do List Application

A modern, feature-rich to-do list web application with local storage functionality. This application allows users to manage their tasks efficiently with a clean and intuitive user interface.

## Features

✨ **Core Features:**
- ✅ Add new tasks
- ✅ Mark tasks as complete/incomplete
- ✅ Delete tasks
- ✅ Filter tasks (All, Active, Completed)
- ✅ Clear all completed tasks at once
- ✅ Task statistics (total and completed count)

💾 **Local Storage:**
- Tasks are automatically saved to browser's local storage
- All data persists even after closing the browser
- No backend server required

🎨 **User Interface:**
- Modern, responsive design
- Gradient background
- Smooth animations and transitions
- Mobile-friendly layout
- Priority badges for tasks
- Clean and intuitive controls

## Project Structure

```
tributario-co/
├── index.html      # HTML structure and layout
├── styles.css      # Styling and responsive design
├── script.js       # JavaScript functionality and local storage
└── README.md       # Project documentation
```

## Files Description

### index.html
Contains the HTML markup for the application:
- Input field for adding new tasks
- Button to add tasks
- Filter buttons (All, Active, Completed)
- Task list container
- Statistics display
- Clear completed button

### styles.css
Provides complete styling with:
- Gradient background
- Card-based layout
- Smooth animations
- Responsive grid system
- Custom scrollbar styling
- Mobile breakpoints

### script.js
Implements the TodoApp class with:
- Task management (add, delete, toggle)
- Local storage save/load functionality
- Filter functionality
- DOM rendering and updates
- Event listeners
- Error handling

## How to Use

1. **Open the Application**
   - Open `index.html` in your web browser

2. **Add a Task**
   - Type your task in the input field
   - Press Enter or click "Add Task" button

3. **Manage Tasks**
   - Click the checkbox to mark a task as complete
   - Click "Delete" to remove a task
   - Tasks are automatically saved to local storage

4. **Filter Tasks**
   - Click "All" to see all tasks
   - Click "Active" to see incomplete tasks
   - Click "Completed" to see completed tasks

5. **Clear Completed**
   - Click "Clear Completed" to delete all completed tasks at once

## Local Storage Implementation

The application uses the browser's `localStorage` API to persist data:

```javascript
// Save to local storage
localStorage.setItem(this.STORAGE_KEY, JSON.stringify(this.todos));

// Load from local storage
const data = localStorage.getItem(this.STORAGE_KEY);
this.todos = JSON.parse(data);
```

**Storage Key:** `todoApp_tasks`

**Data Structure:**
```json
[
  {
    "id": 1623425600000,
    "text": "Sample task",
    "completed": false,
    "priority": "medium",
    "createdAt": "6/10/2026, 3:40:00 AM"
  }
]
```

## Browser Compatibility

- Chrome/Chromium (latest)
- Firefox (latest)
- Safari (latest)
- Edge (latest)
- Any modern browser with ES6 and localStorage support

## Local Storage Limits

- Most browsers allow ~5-10MB of localStorage per domain
- Current application uses minimal storage space
- Storage is domain-specific and cleared with browser cache

## Technology Stack

- **HTML5:** Semantic markup
- **CSS3:** Styling with gradients, flexbox, and animations
- **JavaScript (ES6+):** Object-oriented programming with classes
- **Browser APIs:** localStorage, DOM API

## Future Enhancements

Potential features for future versions:
- [ ] Task editing capability
- [ ] Due dates for tasks
- [ ] Task categories/tags
- [ ] Dark mode theme
- [ ] Export/import functionality
- [ ] Cloud synchronization
- [ ] Notifications/reminders
- [ ] Task prioritization system

## Performance Considerations

- Lightweight: No external dependencies
- Fast load time
- Minimal DOM manipulation
- Efficient local storage operations
- Smooth animations with CSS transitions

## Accessibility

- Semantic HTML structure
- Keyboard navigation support
- Focus indicators on interactive elements
- Color contrast compliance
- Proper ARIA labels consideration

## License

This project is open source and available for personal and educational use.

## Author

Created with ❤️ for efficient task management

---

**Last Updated:** June 10, 2026
