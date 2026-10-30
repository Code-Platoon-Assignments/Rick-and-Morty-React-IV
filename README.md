# Rick and Morty React IV

By the end of this assignment your project should meet the following requirements:
    
  - FavoriteCharactersPage.jsx should display all characters marked as favorite by the user
  - Route to render FavoriteCharactersPage.jsx as a child of App.jsx
  - Users should be able to add or remove Characters from their Favorites and they can't have more than 4 favorite characters at a time
  - Ensure to utilize ReactBootStrap and Tailwind.css for styling
  - Add a Cypress test suite that will reinforce all the requirements above.
  - Have fun!

## Hints

- Keep working in your Rick and Morty React III project.
- Child routes can't receive props from App, so keep the favorites in App's state and share them with `<Outlet context={...} />`; any page or component under the Outlet reads them with `useOutletContext()` (from `'react-router'`).
- Using React Bootstrap and Tailwind together: install both (`npm install react-bootstrap bootstrap tailwindcss @tailwindcss/vite`), add `tailwindcss()` to the plugins in `vite.config.js`, import `'bootstrap/dist/css/bootstrap.min.css'` above `'./index.css'` in `src/main.jsx`, and make `src/index.css` start with `@import "tailwindcss" important;`. Without `important`, Bootstrap's CSS overrides your Tailwind classes.
