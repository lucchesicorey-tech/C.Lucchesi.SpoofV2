🚀 Chromebook Installation Guide
1. Start a Codespace
Click the green "<> Code" button.

Select "Codespaces".

Click "Create codespace on main".

2. Update Node & Bun
Paste this into the terminal to prepare the system:

Bash
nvm install 20 && nvm use 20 && nvm alias default 20
curl -fsSL https://bun.sh/install | bash
export PATH="$HOME/.bun/bin:$PATH"
3. Install & Start
Run these to launch the proxy:

Bash
bun install
bun start
4. Open the App
Look for the pop-up: "Your application is running on port 8080."

Click "Make Public".

Click "Open in Browser".

⚠️ Pro-Tips
Stop Codespace: When finished, right-click your codespace name in the sidebar and select "Stop Codespace" to save your free hours.

Full Screen: Once the proxy opens, you can press F11 to make the game feel like a real app.
