# MyReads Project

## Application Setup
- `npm install` or `yarn install`
- `npm start` or `yarn start`

## Requirements
* npm

## How to Run:
1. Run `npm install` to install the project dependencies.
2. Run the app using `npm start`.
3. App can be seen at: `localhost:3000`.

## Backend Server
To simplify your development process, we've provided a backend server for you to develop against. The provided file [`BooksAPI.js`](src/BooksAPI.js) contains the methods you will need to perform necessary operations on the backend:

## Main Page
- The main page shows 3 shelves for books.
- The main page shows a control that allows users to move books between shelves. The control should be tied to each book instance.
- When the browser is refreshed, the same information is displayed on the page.

## Search Page
- The search page has a search input field. As the user types into the search field, books that match the query are displayed on the page.
- Search results on the search page allow the user to select “currently reading”, “want to read”, or “read” to place the book in a certain shelf.
- When an item is categorized on the search page, and the user navigates to the main page, it appears on that shelf in the main page.

## Routing
- The main page contains a link to the search page. When the link is clicked, the search page is displayed and the URL in the browser’s address bar is /search.
- The search page contains a link to the main page. When the link is clicked, the main page is displayed and the URL in the browser’s address bar is /.

## Code Functionality
- Component state is passed down from parent components to child components. The state variable is not modified directly - setState() function is used correctly.
- Books have the same state on both the search page and the main application page: If a book is on a bookshelf, that is reflected in both locations.
- All JSX code is formatted properly and functional.

## Important
The backend API uses a fixed set of cached search results and is limited to a particular set of search terms, which can be found in [SEARCH_TERMS.md](SEARCH_TERMS.md). That list of terms are the _only_ terms that will work with the backend, so don't be surprised if your searches for Basket Weaving or Bubble Wrap don't come back with any results.
