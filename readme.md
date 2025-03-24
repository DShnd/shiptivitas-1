# Kanban Board Implementation

## Overview
This project enhances the **Shiptivitas frontend** by adding a **Kanban board** for managing shipping requests. The board allows users to **drag and drop** shipping requests between different statuses.

## Features Implemented
✅ **Three Swimlanes:** Backlog, In Progress, Complete  
✅ **Drag-and-Drop Functionality:** Move shipping requests between lanes  
✅ **Dynamic Styling:** Cards change color based on their status  
✅ **Frontend-Only Changes:** No backend modifications required  

## File Modifications

### 1. `board.js`
- Manages the **Kanban board** structure.
- Categorizes shipping requests into different **swimlanes**.
- Integrates **Dragula** for drag-and-drop functionality.

### 2. `board.css`
- Defines styles for the **Kanban board layout**.

### 3. `swimlane.js`
- Defines the **Swimlane component** that holds the shipping request cards.
- Accepts a `dragulaRef` to enable **drag-and-drop** within swimlanes.

### 4. `swimlane.css`
- Styles the **swimlane columns**, ensuring proper spacing.

### 5. `card.js`
- Defines the **Card component** representing individual shipping requests.
- Assigns a class dynamically based on status:
  - **Backlog:** Grey  
  - **In Progress:** Blue  
  - **Complete:** Green  

### 6. `card.css`
- Defines styles for cards, including **status-based colors**.

## Drag-and-Drop Implementation
- **Dragula** is used to enable drag-and-drop functionality.
- **Containers (swimlanes)** are passed as references to Dragula.
- When a card is moved to a new swimlane:
  - **Its status is updated**.
  - **Its color is changed** to match the new status.

## Next Steps
🚀 **Backend Integration:** Persist task statuses in a database.  
🚀 **Animations:** Smooth transitions for card movements.  
🚀 **User Authentication:** Personalized task management.  

## Notes
This implementation follows the **acceptance criteria** provided and aims to improve **task management usability** by making it **more intuitive**.

---
### 📌 Developed for Shiptivitas Frontend  
