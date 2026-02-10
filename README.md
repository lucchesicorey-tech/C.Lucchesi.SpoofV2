🚀 How to Run on Chromebook (No Linux Needed)

If your Chromebook has the Linux development environment blocked, you can run this project using GitHub Codespaces. This runs the code on GitHub's servers and streams the app to your browser.

1. Launch Codespace

Click the green "<> Code" button at the top of this repository.

Select the "Codespaces" tab.

Click "Create codespace on main".

2. Prepare the Environment

Once the terminal opens at the bottom, copy and paste these commands in order to fix the Node.js and Bun versions:

nvm install 20 && nvm use 20 && nvm alias default 20

curl -fsSL https://bun.sh/install | bash
export PATH="$HOME/.bun/bin:$PATH"

node -v  # Should be v20.x.x

bun -v   # Should be 1.x.x

3. Install & Start

Now you can install the dependencies and launch the proxy:

bun install

bun start

4. Access the Proxy

After running bun start, look for a notification in the bottom-right corner saying "Your application is running on port 8080."

Click "Make Public" (this is important, otherwise it will block you).

Click "Open in Browser".

Enjoy! You can now use the proxy to access blocked sites
