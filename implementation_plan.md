# Vasuki 2.0 Implementation Plan

## Goal Description
Build a professional-grade, responsive, and aesthetic ChatGPT-like application named "Vasuki 2.0" using React, Vite, and Tailwind CSS. The app will feature a modern dark-mode UI, smooth animations, and a responsive sidebar layout.

## User Review Required
- **Backend**: Currently, this plan focuses on the Frontend. The backend will be mocked or added in a later phase.
- **Design**: The design will mimic ChatGPT with "Premium" aesthetics (glassmorphism, gradients).

## Proposed Changes

### Project Configuration
#### [NEW] [tailwind.config.js](file:///home/harshpandya/.gemini/antigravity/scratch/vasuki-2.0/tailwind.config.js)
- Configure Tailwind CSS with custom colors and animations.
#### [MODIFY] [index.css](file:///home/harshpandya/.gemini/antigravity/scratch/vasuki-2.0/src/index.css)
- Add base styles, dark mode defaults, and custom utilities.

### Components
#### [NEW] [Layout.jsx](file:///home/harshpandya/.gemini/antigravity/scratch/vasuki-2.0/src/components/Layout.jsx)
- Main application wrapper with Sidebar and Chat Area.
- Handles responsive state (mobile drawer).

#### [NEW] [Sidebar.jsx](file:///home/harshpandya/.gemini/antigravity/scratch/vasuki-2.0/src/components/Sidebar.jsx)
- Navigation sidebar with chat history list (mocked).
- "New Chat" button.

#### [NEW] [ChatArea.jsx](file:///home/harshpandya/.gemini/antigravity/scratch/vasuki-2.0/src/components/ChatArea.jsx)
- Main chat container.
- Renders list of messages.

#### [NEW] [Message.jsx](file:///home/harshpandya/.gemini/antigravity/scratch/vasuki-2.0/src/components/Message.jsx)
- Individual chat message component (User/AI).
- Markdown rendering support (optional/later).

#### [NEW] [ChatInput.jsx](file:///home/harshpandya/.gemini/antigravity/scratch/vasuki-2.0/src/components/ChatInput.jsx)
- Textarea for user input.
- Send button.

### App Entry
#### [MODIFY] [App.jsx](file:///home/harshpandya/.gemini/antigravity/scratch/vasuki-2.0/src/App.jsx)
- Integrate Layout and State management.

## Verification Plan

### Automated Tests
- Run `npm run dev` to start the development server.
- Ensure no build errors with `npm run build`.

### Manual Verification
- **Responsiveness**:
    - Open the app in a browser subagent.
    - Resize window to mobile width (< 768px) to verify Sidebar collapses into a drawer/hamburger menu.
    - Verify desktop layout shows Sidebar permanently.
- **Interactions**:
    - Type in the input and send a message.
    - Verify message appears in the chat list.
    - Verify "New Chat" button clears the view (or mocks it).
- **Aesthetics**:
    - Check dark mode colors and glassmorphism effects.
