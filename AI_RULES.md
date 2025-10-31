# 🤖 AI Editor Guidelines (Dyad Rules)

This document outlines the core technology stack and specific rules for component creation and library usage within this project to ensure consistency, maintainability, and adherence to best practices.

## 🛠️ Tech Stack Overview

This application is built using a modern, robust, and scalable stack:

*   **React:** The primary library for building the user interface.
*   **TypeScript:** Used universally across the codebase for type safety and improved developer experience.
*   **Tailwind CSS:** A utility-first CSS framework used for all styling, ensuring responsive and modern designs.
*   **React Router:** Used for handling client-side navigation and routing within the application.
*   **shadcn/ui:** The source for pre-built, accessible, and customizable UI components (based on Radix UI).
*   **lucide-react:** The designated library for all icons used throughout the application.
*   **File Structure:** Components reside in `src/components/` and main routes/views are located in `src/pages/`.

## 📐 Component and Library Usage Rules

To maintain a clean and elegant codebase, the following rules must be strictly followed:

1.  **Styling:** All styling must be implemented using **Tailwind CSS** utility classes. Designs must be responsive by default.
2.  **UI Components:**
    *   Prioritize using components from **shadcn/ui**.
    *   If a component needs customization or is not available in shadcn/ui, create a new, dedicated component file in `src/components/`. **Do not modify the source files of shadcn/ui components.**
    *   Every new component or hook must be created in its own file. Avoid adding multiple components to a single file.
3.  **Icons:** Use the **lucide-react** library for all icon needs.
4.  **Routing:** Use **React Router** for defining and managing application routes, typically configured in `src/App.tsx`.
5.  **Code Quality:** Focus on simplicity and elegance. Avoid over-engineering, complex error handling (unless requested), and partial implementations. All code changes must result in a fully functional state.
6.  **File Naming & Structure:**
    *   Pages must be placed in `src/pages/`.
    *   Reusable components must be placed in `src/components/`.
    *   Directory names must be all lower-case.