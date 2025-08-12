Objective
Set up a first mobile application using the Expo Router template, modify the home screen, run and test the app, and document the scaffolding process along with the effects of the reset command.

Steps Followed for Scaffolding
Navigate to Project Directory

bash
Copy
Edit
cd prodev-mobile-setup
Initialize the Project with Expo Router Template

bash
Copy
Edit
npx create-expo-app@latest .
Modify the Home Screen

Open app/(tabs)/index.tsx.

Locate the default text "Welcome!".

Replace it with:

tsx
Copy
Edit
** First App Created**
Run the Application

bash
Copy
Edit
npx expo start
iOS: Scan the QR code in the terminal using the Camera app.

Android: Scan the QR code using the Expo Go app.

Reset the Application

bash
Copy
Edit
npm run reset-project
Observations from the Reset Command
The reset-project command clears all modifications made to the project and restores it to its initial scaffolded state.

All custom code changes (such as the updated "First App Created" text) are removed.

The file structure and content revert to the default Expo Router template setup.

It helps return the project to a clean baseline for fresh development.

File Structure After Scaffolding
pgsql
Copy
Edit
prodev-mobile-setup/
│
├── app/
│   ├── (tabs)/
│   │   ├── index.tsx       # Modified to display "First App Created"
│   │   └── other tab files
│   └── _layout.tsx
│
├── constants/
│   └── Colors.tsx
│
├── package.json
├── README.md

└── app.json
