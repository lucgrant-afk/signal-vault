# The Signal Vault

A seven-room browser escape game for IB DP Design Technology A3.4.
Students investigate simulated components and decoys, identify a logic gate, complete its truth table, and answer a structured broader-topic question. All three sections must pass to earn a digit.

## Publish with GitHub Pages

1. Create a GitHub repository, for example `signal-vault`. Use a public repository for GitHub Free.
2. Extract the ZIP on your computer.
3. In your repository, choose **Add file > Upload files**. Upload the extracted files, not the ZIP or its containing folder. `index.html`, `app.js`, `rules.js`, and `style.css` must sit together at the repository root. Commit them to `main`.
4. Open **Settings > Pages**.
5. Under **Build and deployment**, choose **Deploy from a branch**.
6. Select **main**, then **/(root)**, and click **Save**.
7. Wait for publishing to finish. The Pages settings will show **Visit site** and your website address. Share that address with students, rather than the repository URL.

The `.nojekyll` file is included to serve the files directly. If your file browser hides it, you can create an empty `.nojekyll` file in GitHub using Add file > Create new file. This application does not need a build step, npm installation, API key, server, or ChatGPT sign-in.

## Files

- `index.html`: page shell and instructions
- `style.css`: layout, room visuals and responsive design
- `app.js`: interaction, drawing, answer entry, progress and navigation
- `rules.js`: seven room definitions, gate logic, questions and checking
- `.nojekyll`: disables Jekyll processing

Keep the filenames unchanged. The relative paths also work when the site is hosted under a repository subdirectory.

## Classroom use

- Click a button or lever to activate it; click again to release. This lets pupils test combined inputs.
- Some connected controls have no effect.
- The drawing pad is for working. Pupils enter their final outputs in the grid for automatic checking.
- Broader-topic questions use structured responses so marking is deterministic.
- Progress saves in the current browser for the current site address. It is not a central teacher dashboard and does not sync between devices.
- Restart clears the browser's saved mission after confirmation.
- Fonts load from Google Fonts when available, with system-font fallbacks.

## Editing and updates

Edit room content and logic in `rules.js`, interactions in `app.js`, and appearance in `style.css`. Commit changes to `main`; GitHub Pages republishes from that branch.

For a local preview, serve the directory with any static web server, for example `python3 -m http.server 8000`, then open `http://localhost:8000`. Use a server rather than double-clicking `index.html`, because browsers restrict JavaScript module loading from local file URLs.

## GitHub documentation

- https://docs.github.com/en/pages/getting-started-with-github-pages/creating-a-github-pages-site
- https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site
