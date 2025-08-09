# React State Management Lab - Complete Solution

🧟‍♂️ **Zombie Fighter Team Builder** - A React application demonstrating state management concepts.

## Features Completed

✅ **All homework requirements implemented:**

1. **State Management**
   - `team` state (array of recruited fighters)
   - `money` state (budget tracking)  
   - `zombieFighters` state (available fighters)

2. **Add Fighter Functionality** 
   - Budget validation ("Not enough money")
   - Remove fighter from available list when recruited
   - Deduct cost from money

3. **Remove Fighter Functionality**
   - Remove from team, add back to available fighters
   - Refund money to budget

4. **Team Display**
   - Shows "Pick some team members!" when team is empty
   - Displays team members with images and stats
   - Remove button for each team member

5. **Statistics**
   - **Total Strength** calculation (sum of team members)
   - **Total Agility** calculation (sum of team members)
   - Real-time updates when team changes

6. **UI Improvements**
   - Fighter images displayed
   - Clean sections for Team vs Available Fighters
   - Responsive styling with CSS

## How to Run

```bash
npm install
npm run dev
```

Visit `http://localhost:5173` to play the game!

## Game Rules

- Start with **$100 budget**
- Recruit fighters from the available list
- Each fighter has different **price**, **strength**, and **agility**
- Build your team strategically for the zombie apocalypse!
- Remove team members to get refunds and try different combinations

## Technical Implementation

- **React 19.1.1** with functional components
- **useState** hooks for state management
- **Vite** for fast development
- **ESLint** for code quality
- Pure JavaScript (no TypeScript)

Built on top of Taeiko's foundation code and completed all General Assembly homework requirements! 🎯

---

# Original Vite Template Info

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
export default {
  // other rules...
  parserOptions: {
    ecmaVersion: 'latest',
    sourceType: 'module',
    project: ['./tsconfig.json', './tsconfig.node.json'],
    tsconfigRootDir: __dirname,
  },
}
```

- Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
- Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
- Install [eslint-plugin-react-hooks](https://www.npmjs.com/package/eslint-plugin-react-hooks) and add `plugin:react-hooks/recommended` to the `extends` list
