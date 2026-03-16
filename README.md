# P2P Secure Chat

A peer-to-peer encrypted chat application that runs entirely in the browser. No server required!

## Features

- 🔒 **End-to-end encryption** - Password-based message verification
- 👥 **Two users** - Connect directly via PeerJS
- 💾 **Message history** - Saved locally in browser
- 🌐 **No server** - Runs on GitHub Pages (static only)
- 📱 **Mobile friendly** - Works on any device with a browser

## How to Use

### Setup

1. Open the app in your browser
2. Enter your **name** and **password**
3. You'll get a unique **Peer ID** (e.g., `p2p-abc123-xyz`)

### Connect with Friend

1. Share your Peer ID with your friend
2. Friend enters your Peer ID + your password
3. Connection established automatically!

### Chat

- Type messages and press Enter or click Send
- Messages are saved locally in your browser
- History persists across sessions

## Deploy to GitHub Pages

```bash
# Fork or create a new repo, then:
git clone your-repo
cd your-repo
# Copy index.html here
git add index.html
git commit -m "Add P2P chat app"
git push
```

Then go to **Settings → Pages** and enable GitHub Pages from the `main` branch.

## Technical Details

- **PeerJS** - Handles WebRTC peer-to-peer connections
- **localStorage** - Stores profile and message history
- **Password verification** - Simple handshake to verify identity

## Security Note

This is a simple P2P chat. The "password" is used for:
1. Verifying the connection (handshake)
2. Identifying yourself to the other user

For true end-to-end encryption, you'd need a more sophisticated implementation with proper key exchange.

## License

MIT
