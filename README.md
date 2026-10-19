# Sreedevi Balaji — Career Website

A responsive, multi-page career website built with plain HTML, CSS, and JavaScript. It is a static site: there is no build step, package installation, or backend to configure.

## Run the website on your computer

### Option 1: Open it directly

1. Open the website folder in File Explorer.
2. Double-click `index.html` to open the home page in your browser.
3. Use the navigation at the top of the page to visit **Experience**, **Selected work**, and **Contact**.

The pages and downloadable profile work when opened this way in most browsers. If you run into browser restrictions or want to test the site as a locally hosted website, use Option 2.

### Option 2: Run a local web server (recommended)

The website does not need a dedicated server application. Python's built-in HTTP server is sufficient.

1. Open **PowerShell** or **Windows Terminal**.
2. Change to the website folder. For the current location, run:

   ```powershell
   cd "C:\Sreedevi_Documents\PM_Learnings\GitHubRepo\My Website"
   ```

   If you have moved the folder, replace the path above with its new location. Alternatively, in File Explorer, open the website folder, click the address bar, type `powershell`, and press **Enter**.

3. Start the local server:

   ```powershell
   py -m http.server 8000 --bind 127.0.0.1
   ```

   If the `py` command is unavailable but Python is installed, use:

   ```powershell
   python -m http.server 8000 --bind 127.0.0.1
   ```

4. Leave that terminal window open while you use the site. Open this address in your browser:

   [http://localhost:8000](http://localhost:8000)

   The server displays the files in the folder. If it shows a file listing, select `index.html`.

5. To stop the server, return to the terminal and press **Ctrl+C**.

If port `8000` is already in use, choose another port, such as `8080`, in the server command and visit `http://localhost:8080` instead.

## Open and edit the site in Visual Studio Code

1. In Visual Studio Code, select **File → Open Folder...**.
2. Select the folder that contains `index.html` and `Profile.pdf`.
3. Open `index.html`, `experience.html`, `projects.html`, or `contact.html` to edit page content. Shared styling is in `styles.css`, and the small navigation/year script is in `script.js`.
4. Save your changes and refresh the browser to see them. If you are using the local server, keep it running in its terminal window.

No extensions are required. You can optionally use a VS Code live-preview extension if you already have one installed.

## Pages and files

| File | Purpose |
| --- | --- |
| `index.html` | Home page and career overview |
| `experience.html` | Roles, experience, education, certifications, and recognition |
| `projects.html` | Selected product work and reported outcomes |
| `contact.html` | Email, phone, LinkedIn, blog, and profile download |
| `styles.css` | Shared layout, colors, typography, and responsive styles |
| `script.js` | Mobile navigation and automatically updated footer year |
| `Profile.pdf` | Source profile and downloadable resume |

## Troubleshooting

- **The page does not load at `localhost`:** Make sure the server command is still running and the terminal is in the folder containing `index.html`.
- **The port is busy:** Use another port, for example `py -m http.server 8080 --bind 127.0.0.1`, and open `http://localhost:8080`.
- **The profile download cannot be found:** Keep `Profile.pdf` in the same folder as the HTML files.
- **Changes are not visible:** Save the edited file and refresh the browser. A hard refresh with **Ctrl+F5** can clear a cached stylesheet.
- **Python is not installed:** Use Option 1 to open `index.html` directly, or install Python from the official Python website before using Option 2.

The local server command above binds to your own computer (`127.0.0.1`) and serves the current folder. Stop it with **Ctrl+C** when you are done.
