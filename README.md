🚀 How to Run on Chromebook (No Linux Needed)
If your Chromebook has the Linux development environment blocked, you can run this project using GitHub Codespaces. This runs the code on GitHub's servers and streams the app to your browser.

1. Launch Codespace
Click the green "<> Code" button at the top of this repository.

Select the "Codespaces" tab.

Click "Create codespace on main".

2. Prepare the Environment
Once the terminal opens at the bottom, copy and paste these commands to fix the Node.js and Bun versions:

Bash
# 1. Upgrade Node.js (Required for Astro)
nvm install 20 && nvm use 20 && nvm alias default 20

# 2. Install Bun
curl -fsSL https://bun.sh/install | bash
export PATH="$HOME/.bun/bin:$PATH"

# 3. Verify versions
node -v  # Should be v20.x.x
bun -v   # Should be 1.x.x
3. Install & Start
Now you can install the dependencies and launch the proxy:

Bash
# Install the project pieces
bun install

# Start the server
bun start
4. Access the Proxy
Look for a notification in the bottom-right corner saying "Your application is running on port 8080."

Click "Make Public" (this is important, otherwise it will be blocked).

Click "Open in Browser" to launch your proxy.

⚠️ Pro-Tips for Chromebook Users
Saving Time: When you're done, go to the Explorer (top left), right-click your Codespace name, and select "Stop Codespace" to save your free monthly hours.

Avoid Clumping: Always leave a blank line before and after your code blocks to keep the formatting clean on GitHub.
