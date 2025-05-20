# About This Project
Loan app is a modern, responsive loan application web platform built using React, Vite, Tailwind CSS, and Redux Toolkit. The platform enables users to securely apply for loans, manage their loan status, and receive timely updates — all within an intuitive, user-friendly interface.

The application is integrated with Appwrite to handle authentication, user management, and secure backend operations. 
## 🔧 Tech Stack

- React + Vite: Fast frontend development and lightning-fast builds.
- Tailwind CSS: Utility-first styling for a clean, responsive UI.
- Redux Toolkit: Predictable state management.
- React Router: Client-side routing with protected pages.
- Appwrite: Backend-as-a-service (BaaS) for auth, database, and functions.

## 🎯 Key Features (Planned or Implemented)
- 🔐 User registration, login, and email verification
- 📄 Loan application form with validation
- 👤 User dashboard to track applications
- 📬 Notifications for approval or rejection
- 📂 Admin panel for managing user submissions 

# React + TypeScript + Vite
## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type-aware lint rules:

```js
export default tseslint.config({
  extends: [
    // Remove ...tseslint.configs.recommended and replace with this
    ...tseslint.configs.recommendedTypeChecked,
    // Alternatively, use this for stricter rules
    ...tseslint.configs.strictTypeChecked,
    // Optionally, add this for stylistic rules
    ...tseslint.configs.stylisticTypeChecked,
  ],
  languageOptions: {
    // other options...
    parserOptions: {
      project: ['./tsconfig.node.json', './tsconfig.app.json'],
      tsconfigRootDir: import.meta.dirname,
    },
  },
})
```

You can also install [eslint-plugin-react-x](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-x) and [eslint-plugin-react-dom](https://github.com/Rel1cx/eslint-react/tree/main/packages/plugins/eslint-plugin-react-dom) for React-specific lint rules:

```js
// eslint.config.js
import reactX from 'eslint-plugin-react-x'
import reactDom from 'eslint-plugin-react-dom'

export default tseslint.config({
  plugins: {
    // Add the react-x and react-dom plugins
    'react-x': reactX,
    'react-dom': reactDom,
  },
  rules: {
    // other rules...
    // Enable its recommended typescript rules
    ...reactX.configs['recommended-typescript'].rules,
    ...reactDom.configs.recommended.rules,
  },
})
```
