# 🖼️ MediaSearch Gallery

A small React gallery for searching **photos, videos, and GIFs**. Browse results from Unsplash, Pexels, and Tenor, then save favorites to a collection stored in your browser.

## ✨ Features

- 🔎 Search media by keyword and switch between photos, videos, and GIFs.
- 🔗 Open the original media source in a new tab.
- 💾 Save and remove items from your collection, or clear it all at once.
- 📱 Collection data is saved in browser `localStorage` on your device.

## 🧰 Tech stack

React 18, Vite, Redux Toolkit, React Redux, React Router, Axios, Tailwind CSS, and React Toastify.

There’s no custom backend. The app requests media directly from the Unsplash, Pexels, and Tenor APIs.

## 🚀 Getting started

1. Install Node.js (npm is included).
2. Open a terminal in the project directory and install dependencies:

   ```bash
   npm install
3. Create a .env file in the project root and add your API keys:
   VITE_UNSPLASH_KEY=your_unsplash_access_key
   VITE_PEXELS_KEY=your_pexels_api_key
   VITE_TENOR_KEY=your_tenor_api_key
4. Start the development server:
   npm run dev
## 📁 Project layout
- src/api/mediaApi.js — requests to Unsplash, Pexels, and Tenor.
- src/redux/features/searchSlice.js — search query, selected tab, results, and loading/error state.
- src/redux/features/collectionSlice.js — saved media and browser storage persistence.
- src/components/ — navigation, search controls, tabs, and media cards/grid.
- src/pages/ — search home and saved collection pages.
