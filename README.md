# Daily Hunt Application

This is a React-based web application named **Daily Hunt** that displays news articles from various categories using the News API. The application features two navigation bars, various news categories, and utilizes infinite scrolling to load more news articles as the user scrolls down.

## Features

- **Multiple News Categories**: Users can browse news articles in different categories like Entertainment, Technology, Sports, Business, Health, and Science.
- **Infinite Scroll**: As users scroll down, more news articles are loaded dynamically.
- **Responsive Design**: The application is designed to be responsive and works well on different screen sizes.
- **Navigation Bars**: Two navigation bars for ease of navigation— one for the app branding and another for category links.

## Installation and Setup

1. **Clone the repository**:
    ```sh
    git clone https://github.com/yourusername/news.git
    cd news
    ```

2. **Install dependencies**:
    ```sh
    npm install
    ```

3. **Run the application**:
    ```sh
    npm start
    ```

4. **Open your browser** and navigate to `http://localhost:3000` to see the app in action.

## Components

1. **App.js**:
    - Main component that sets up the routing and includes `NavBar1`, `NavBar2`, and different routes for news categories.

2. **NavBar1.js**:
    - The top navigation bar that displays the application name.

3. **NavBar2.js**:
    - The secondary navigation bar that contains links to various news categories.

4. **News.js**:
    - Fetches news articles from the News API and manages state for the articles, total results, and pagination. It also implements infinite scrolling using the `react-infinite-scroll-component`.

5. **NewsItem.js**:
    - Displays individual news articles with an image, title, description, source name, and a link to read more.

## API Integration

The application uses the [News API](https://newsapi.org/) to fetch news articles. The API key is included in the fetch URL for demonstration purposes. In a real-world application, it's recommended to keep the API key secure.

```js
const url = `https://newsapi.org/v2/top-headlines?country=in&category=${category}&page=${page}&apiKey=your_api_key`;
```

## Usage

- **Browse News Categories**: Click on the categories in the navigation bar to view news articles for that specific category.
- **Load More Articles**: Scroll down to automatically load more news articles.
- **Read Full Articles**: Click on "Read More..." to open the full news article in a new tab.

## Dependencies

- **React**: JavaScript library for building user interfaces.
- **react-router-dom**: DOM bindings for React Router for navigation.
- **react-infinite-scroll-component**: Component to implement infinite scrolling.
- **Bootstrap**: CSS framework for styling.

Install these dependencies using npm:

```sh
npm install react react-dom react-router-dom react-infinite-scroll-component bootstrap
```


## Contribution

Contributions are welcome! Feel free to fork the repository and submit pull requests.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
