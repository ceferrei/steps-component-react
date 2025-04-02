# Interactive Steps Component - React

This project implements an interactive user interface (UI) component that guides the user through a multi-step process. It was built using React and demonstrates several fundamental concepts of the library.

## Description

The "Steps" component presents a numbered sequence of steps, along with a descriptive message for the current step. It includes navigation buttons ("Previous" and "Next") to move through the steps and a button to hide or show the entire component.

## Demo

<div align="center">
  <video src="https://github.com/user-attachments/assets/dcdc0696-a85e-4b48-89b7-7b80af0a9eb6" controls width="600">
    Seu navegador não suporta o elemento de vídeo.
  </video>
</div>

## Features

- **Step Visualization:** Displays a numbered list of steps (1, 2, 3).
- **Progress Indication:** Highlights the current step number and completed steps.
- **Dynamic Messages:** Shows a specific message corresponding to the active step.
- **Navigation:** Allows navigation between steps using the "Previous" and "Next" buttons.
- **Visibility Toggle:** Includes a "Close" button (`&times;`) to show or hide the component.
- **Per-Step Actions:** Demonstrates including an action button ("Learn how") within the step message.
- **Componentization:** Uses reusable components (`Button`, `StepMessage`) for a modular structure.

## State Management

The application's state is managed locally within the `Steps` component using the `useState` Hook:

- **`step`**: Stores the current step number (initialized to `1`). It is updated using the callback form (`setStep(s => s - 1)`) to ensure safe updates based on the previous state.
- **`isOpen`**: Stores a boolean indicating whether the component is visible (initialized to `true`). It is toggled using the callback form (`setIsOpen(is => !is)`).

## How to Use/Run

1.  **Clone the repository** (or ensure you have the project files).

    ```
    git clone https://github.com/ceferrei/steps-component-react.git
    ```

2.  **Navigate to the project directory** in your terminal.

    ```
    cd steps-component-react
    ```

3.  **Install the necessary dependencies**:
    ```bash
    npm install
    # or
    yarn install
    ```
4.  **Start the development server**:
    ```bash
    npm start
    # or
    yarn start
    ```
5.  Open your browser and go to `http://localhost:3000` (or the port indicated in the terminal).

## Key Concepts Demonstrated

- React Functional Components.
- `useState` Hook for local state management.
- Props for passing data and functions between components.
- Component Composition (nesting `StepMessage` and `Button` within `Steps`).
- Conditional Rendering (to show/hide the component with `isOpen` and to apply the `.active` class).
- Event Handling (`onClick` on buttons).
- Using Arrays to store data (messages).
- Styling with CSS and classes.
- Safe state updates using callbacks in `setState`.
