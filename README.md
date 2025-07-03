# Dynamic Form Builder

## Description

This project provides a dynamic form interface with step-based navigation, language and currency selection, and region-specific fields. The form adapts to the selected language and currency, and dynamically renders different fields, including OTP and validation codes, based on the selected region.

### Key Features:
- **Language & Currency Selection**: Choose your language and currency via the **Header** component. The URL updates accordingly (e.g., `register?currency=IRT&lang=en`).
- **Step-Based Form**: The form is split into two steps. In the second step, region-specific fields are rendered based on the region selected (e.g., Turkey).
- **Dynamic Form Fields**: Fields are rendered dynamically based on configuration, and validation is handled accordingly.
- **ReCAPTCHA Integration**: A ReCAPTCHA widget is included in the second step for verification.
- **Responsive Design**: The form and header are fully responsive.

---

## Project Structure

Here’s an overview of the folder structure:

```
src/
├── components/
│   ├── Header.tsx        # Header component with language and currency selection
│   ├── Header.css        # CSS styles for the Header component
│   ├── DynamicForm.tsx   # Dynamic form component
│   ├── DynamicForm.css   # CSS styles for the DynamicForm component
├── hooks/
│   └── useFormConfig.ts  # Custom hook to fetch form configuration
├── App.tsx               # Main component with routing setup
├── index.tsx             # Entry point for the application
└── package.json          # Project dependencies and scripts
```


---

## Key Functionalities

### Language & Currency Selection

- The **Header** component allows users to select the **language** (English, Turkish, Persian) and **currency** (e.g., IRT, USD, TRY).
- Upon selecting a new language or currency, the URL updates to reflect the selected options. For example:
  - `register?currency=IRT&lang=en`
  - This ensures that the page reloads with the selected language and currency preferences.

### Step-Based Form

- The form consists of **two steps**:
  - **Step 1**: Basic fields (first name, last name, email, password).
  - **Step 2**: Region-specific fields (e.g., OTP, phone number) based on the region selected (e.g., Turkey).

  

### ReCAPTCHA Integration

- In Step 2, there’s a **ReCAPTCHA** widget for user verification.
- The current ReCAPTCHA is set up for **localhost**. You will need to update the **site key** for production or staging environments.

---
## Prerequisites

Before running the app, make sure you have the following tools installed:

- [Node.js](https://nodejs.org/) (which includes npm) – To manage dependencies.
- [npm](https://www.npmjs.com/) (Node Package Manager) – To install dependencies and run scripts.
- [TypeScript](https://www.typescriptlang.org/) – Used for static typing in this project.
- [react-router-dom](https://reactrouter.com/) – For routing between pages.

## How to Run

1. **Clone the repository**:

   ```bash
   https://github.com/nibaka/Dynamic-Form-Application


2. ## Installation

To install the required dependencies, run the following commands:

### Install `@types/react-google-recaptcha` (for TypeScript support with reCAPTCHA)

This package provides TypeScript definitions for the `react-google-recaptcha` library:

```bash
npm install --save-dev @types/react-google-recaptcha
```

### Install `react-router-dom` (for routing in React)

`react-router-dom` is used for routing in React apps, allowing navigation between different components or pages:

```bash
npm install react-router-dom
```

### Install TypeScript (if you haven't installed it already)

If TypeScript is not yet installed in your project, you can add it with:

```bash
npm install --save-dev typescript
```

### Install TypeScript-related dependencies (Optional)

If you are using TypeScript in your React project, you may also want to install TypeScript-related tools to manage `.ts` and `.tsx` files:

```bash
npm install --save-dev @types/react @types/react-dom
```

  
3. **Start the development server**:
    ```bash
     npm start
    
  
# 3- June - 3 July
