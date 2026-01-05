# LockX

A lightweight, browser-based password manager with local storage. Securely store, manage, search, and export your passwords with a clean, modern UI built with React and TypeScript.

## About The Project

LockX is a client-side password management tool designed for secure credential storage:
- What it solves: Provides a simple, accessible password manager without cloud syncing (100% local storage)
- What makes it unique: Minimal dependencies, TypeScript type safety, localStorage persistence, easy export functionality (text/copy)
- What was learned: React hooks (useState/useEffect), TypeScript type systems, localStorage data management, form handling, and Radix UI component patterns

The app stores passwords locally in the browser with CRUD operations, search filtering, export-to-text, and individual password export/copy features.

## Built With

- React 19 + TypeScript
- Vite 6
- Tailwind CSS 4
- Radix UI (Dialog, Dropdown, Alert Dialog, Avatar, Label, Toast, Tooltip)
- React Router 7
- React Query (@tanstack/react-query)
- Lucide React (icons)
- localStorage (browser storage)

## Getting Started

### Prerequisites
- Node.js 16+ and npm

### Installation

1. Clone the repo
   ```bash
   git clone https://github.com/tumansutradhar/lock-x.git
   cd lock-x
   ```

2. Install dependencies
   ```bash
   npm install
   ```

3. Run the development server
   ```bash
   npm run dev
   ```

4. Open in your browser
   ```
   http://localhost:5173/
   ```

## Usage

1. **Add Password**: Click "Add Password" button, fill in website, username, and password
2. **Search**: Use the search bar to filter passwords by website or username
3. **View/Edit**: Click on any password item to view or edit details
4. **Copy**: Copy username or password to clipboard with one click
5. **Export**: 
   - Export single password as text
   - Export all passwords as text file or copy to clipboard
6. **Delete**: Remove passwords with confirmation dialog

All data is stored locally in your browser's localStorage and never sent to any server.

## Features

- Create, read, update, delete (CRUD) passwords
- localStorage persistence (survives page refresh)
- Search/filter passwords by website or username
- Copy username/password to clipboard
- Export single password as text
- Export all passwords to file or clipboard
- Responsive design for mobile and desktop
- TypeScript type safety
- Radix UI dialog/dropdown components
- Toast notifications for user feedback
- Delete confirmation modal
- Clean, modern dark-themed UI with Tailwind CSS

## Project Structure

```
lock-x/
├── src/
│   ├── components/
│   │   ├── SearchBar.tsx
│   │   ├── PasswordList.tsx
│   │   ├── PasswordItem.tsx
│   │   ├── PasswordForm.tsx
│   │   ├── DeleteConfirmation.tsx
│   │   └── ui/ (Radix/shadcn components)
│   ├── hooks/
│   │   └── usePasswordManager.ts
│   ├── types/
│   │   └── password.ts
│   ├── pages/
│   │   ├── Index.tsx
│   │   └── NotFound.tsx
│   ├── App.tsx
│   └── main.tsx
├── package.json
├── vite.config.ts
├── tsconfig.json
└── tailwind.config.ts
```

## Roadmap

- [x] Add/edit/delete passwords
- [x] Search functionality
- [x] localStorage persistence
- [x] Export single/all passwords
- [x] Copy to clipboard
- [x] TypeScript implementation
- [ ] Master password/encryption
- [ ] Password strength indicator
- [ ] Categories/tags for passwords
- [ ] Import passwords from file
- [ ] Auto-fill in browser fields
- [ ] Cloud sync (optional, encrypted)
- [ ] Mobile app version

## Contributing

Contributions are welcome!
1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the MIT License. See `LICENSE.md` for more information.

## Contact

Tuman Sutradhar

- GitHub: [@tumansutradhar](https://github.com/tumansutradhar)
- Email: connect.tuman@gmail.com
- LinkedIn: [Tuman Sutradhar](https://www.linkedin.com/in/tumansutradhar/)

Project Link: [https://github.com/tumansutradhar/lock-x](https://github.com/tumansutradhar/lock-x)

## Acknowledgments

- Radix UI for accessible components
- Tailwind CSS for styling
- React and TypeScript documentation
- Lucide React for icons
