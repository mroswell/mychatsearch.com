# Claude Conversation Search

A local web application for searching through your exported Claude AI conversations. This tool runs entirely in your browser with no server required, keeping your data completely private.

## Features

- 🔍 **Full-text search** across all conversations and messages
- 🎲 **Random conversation discovery** with shuffle feature
- 📝 **Markdown rendering** with toggle to view raw markdown
- 📋 **Copy functionality** for messages, titles, and Claude search URLs
- 🎨 **Claude-inspired UI** with resizable and collapsible sidebar
- 🔒 **100% private** - runs locally in your browser, no data leaves your device
- 🚀 **Fast and responsive** - handles large conversation exports efficiently

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- Your Claude conversation export file (conversations.json)

### How to Export Your Claude Conversations

1. Visit: https://claude.ai/settings/data-privacy-controls
2. Scroll to the bottom of the page and click "Export data"
3. Wait for the email from Claude with your export
4. Download the file when the email arrives
5. Unzip the downloaded file
6. Locate the `conversations.json` file in the extracted folder

### Installation

You have two options:

#### Option 1: Use the hosted version (easiest)
1. Visit https://mychatsearch.com
2. That's it! The tool is ready to use.

#### Option 2: Run locally
1. Download the `index.html` file from this repository
2. Save it anywhere on your computer
3. Double-click the file to open it in your browser

Both options work exactly the same way - your data never leaves your browser.

## Usage

### Loading Your Conversations

1. Click the "Load JSON file" button in the sidebar
2. Select your `conversations.json` file
3. The app will load and display all your conversations

### Searching

- Use the search box at the top to search through all conversations
- Search works across conversation titles and message content
- Results update as you type
- Click "Clear" to reset the search

### Viewing Conversations

- Click any conversation in the sidebar to view its messages
- Toggle between rendered markdown and raw markdown view
- Copy individual prompts and messages with the "Copy" button
- Click "Copy Title" to copy just the conversation name
- Click "Copy Claude Search URL" to get a link that searches for this conversation in Claude. This is helpful since Claude exports do not include all artifacts or file uploads.
- Likewise, Click "Visit ChatGPT.com"  to search a copied title on chatgpt.com. (Click "Search chats")

### Interface Features

- **Resizable sidebar**: Drag the edge to resize
- **Collapsible sidebar**: Click the arrow to hide/show
- **Random conversations**: Click the shuffle button to discover random conversations

## Privacy & Security

This application prioritizes your privacy:

- **No server**: Runs entirely in your browser
- **No external connections**: Your data never leaves your device
- **No tracking**: No analytics or data collection
- **No storage**: Data is only kept in memory while the page is open

## Technical Details

### Supported File Format

- `conversations.json` from Claude exports

### Browser Compatibility

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

### Technologies Used

- Pure HTML/CSS/JavaScript
- [Marked.js](https://marked.js.org/) for markdown rendering
- No other external dependencies

## Troubleshooting

### "Failed to copy" errors

If you get copy errors when running from a local file:
- The app includes a fallback copy method that should work
- Try using a different browser
- Serve the file through a local web server if needed

### Large file performance

For very large conversation exports:
- The initial load may take a few seconds
- Search performance remains fast due to efficient filtering
- Consider using a modern browser for best performance

## Contributing

This is a standalone tool designed for local use. If you have suggestions or improvements:

1. Fork the repository
2. Make your changes
3. Test thoroughly with your own conversation exports
4. Submit a pull request

## License

MIT License - feel free to modify and distribute as needed.

---

**Note**: This tool is not officially affiliated with Anthropic or Claude AI.
