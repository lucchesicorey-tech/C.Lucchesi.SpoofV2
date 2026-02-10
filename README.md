🚀 Chromebook Installation Guide
1. Start a Codespace
Click the green "<> Code" button on this GitHub page.

Select "Codespaces" and click "Create codespace on main".

2. Run the Setup
Wait for the terminal to appear at the bottom. Copy and paste this entire block into the terminal and press Enter:

Bash
nvm install 20 && nvm use 20 && nvm alias default 20
curl -fsSL https://bun.sh/install | bash
export PATH="$HOME/.bun/bin:$PATH"
bun install
bun start
3. Open the Game
A notification will appear: "Your application is running on port 8080."

Click "Make Public" (important!).

Click "Open in Browser".

⚠️ Pro-Tips
Save your hours: When you're done playing, right-click the Codespace name in the bottom-left corner and select "Stop Codespace".

Missing Pop-up? If you don't see the "Port 8080" message, click the "Ports" tab next to the terminal and click the "globe" icon.
