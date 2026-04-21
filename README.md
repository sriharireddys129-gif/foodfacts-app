# FoodFacts App — Part 1

A React + Vite app that lets users search for food products and see real nutrition data from the Open Food Facts API.

## Getting Started

```bash
# 1. Install dependencies
npm install

# 2. Start the dev server
npm run dev
```

Then open **http://localhost:5173** in your browser.

## Features

- Controlled search input with `useState`
- Live API calls to Open Food Facts (no API key needed)
- Loading, empty, and no-results states
- Nutrition cards showing calories, protein, carbs, and fat per 100g
- URL-encoded queries (works for "peanut butter", "olive oil", etc.)
- Responsive grid layout

## Project Structure

```
src/
├── main.jsx
├── App.jsx
├── App.css
├── index.css
└── components/
    ├── SearchBar.jsx
    ├── FoodCard.jsx
    └── FoodList.jsx
```

## Concepts Covered

| Concept | Where |
|---|---|
| JSX | All components |
| Functional Components | SearchBar, FoodCard, FoodList |
| Props | FoodCard `product`, FoodList `products`, SearchBar `onSearch` |
| useState | SearchBar (query), App (results, loading, searched) |
| Controlled Inputs | SearchBar input |
| Event Handling | Form submit, onChange |
| List Rendering + keys | FoodList → `product.code` as key |
| Fetch API + async/await | App.jsx `handleSearch` |
| Conditional Rendering | App.jsx `renderContent()` |
