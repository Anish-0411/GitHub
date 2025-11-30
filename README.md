# GitHub Repositories Viewer

This project is a simple HTML + JavaScript web app for viewing public repositories of any GitHub user. Enter a username, and the app fetches and displays the user's repositories in a table. Each entry shows repo details such as name, description, main coding language, number of stars, and a direct link.

---

## Features

- **Fetch GitHub Repositories:**  
  Enter any GitHub username to see all public repositories belonging to that user.  
- **Repository Table:**  
  Results are shown in a sortable table, including Repository Name, Description, Language, and Stars.  
- **Direct Links:**  
  Click "View Repo" to open the repository on GitHub in a new tab.
- **Error Handling:**  
  Displays a helpful message if the username is not found or the user has no public repositories.

---

## How It Works

- The user inputs a GitHub username.
- On clicking "Fetch Repos," a request is made to GitHub’s public API endpoint:  
  `https://api.github.com/users/${username}/repos`
- The JavaScript uses **XMLHttpRequest** to send the request and process the response.
- Repositories are listed with their:
  - **Name**
  - **Description** (shows "No Description Available" if missing)
  - **Language** (shows "Not Specified" if missing)
  - **Stars** (stargazers_count)
  - **URL** (clickable link)

---

## Tech Stack

| Technology      | Purpose                   | Color Tag Example |
|-----------------|--------------------------|-------------------|
| HTML            | Structure                | ![#e34c26](https://via.placeholder.com/15/e34c26/000000?text=+) `HTML` |
| CSS             | Styling of layout         | ![#563d7c](https://via.placeholder.com/15/563d7c/000000?text=+) `CSS`  |
| JavaScript      | Interactive data fetching | ![#f1e05a](https://via.placeholder.com/15/f1e05a/000000?text=+) `JavaScript` |
| GitHub API      | Data source               | ![#24292e](https://via.placeholder.com/15/24292e/000000?text=+) `GitHub`  |

- Tech color tags shown above follow [GitHub's language color conventions](https://github.com/ozh/github-colors).

---

## How to Run

1. **Clone or Download this Repo**
2. Open `index.html` in your browser.
3. Enter the GitHub username you want to search for.
4. Click "Fetch Repos" to display their repos.

> **No build step required; works entirely client-side.**

---

## Example Usage

![Screenshot of App](https://user-images.githubusercontent.com/your-demo-image.png)  
*Example: Viewing repositories from `octocat`.*

---

## Customization Ideas

- Add badge colors for programming languages (use GitHub language color codes).
- Add more columns, such as forks, issues, last updated.
- Style with [Bootstrap](https://getbootstrap.com/) or another framework.
- Handle pagination and API rate limits gracefully.

---

## License

MIT

---

## Credits

- Built with [GitHub REST API](https://docs.github.com/en/rest).
- Color tags inspired by [github-language-colors](https://github.com/ozh/github-colors).
