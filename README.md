# My Chat Search

A local web application for searching through your exported AI conversations from ChatGPT and Claude. This tool runs entirely in your browser with no server required, keeping your data completely private.

## Features

- **Dual AI support** - Works with both ChatGPT and Claude exports with automatic format detection
- **Full-text search** across all conversations and messages
- **Multi-term search** - Use comma-separated terms to find conversations containing ALL specified terms
- **Keyboard navigation** - Navigate conversations with arrow keys, clear search with Escape
- **Random conversation discovery** with shuffle feature
- **Markdown rendering** with toggle to view raw markdown
- **Copy functionality** for messages, titles, and search URLs
- **Scroll to top** - Quick navigation button for long conversations
- **Clean, intuitive UI** with resizable and collapsible sidebar
- **Accessibility-first** - Full screen reader support, ARIA labels, and keyboard-friendly interface
- **100% private** - runs locally in your browser, no data leaves your device
- **Fast and responsive** - handles large conversation exports efficiently

## Getting Started

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, Edge)
- Your ChatGPT and/or Claude conversation export file (conversations.json)

### How to Export Your Conversations

You can load ChatGPT exports, Claude exports, or both (by switching between tabs).

#### Exporting from ChatGPT

1. Visit: https://chatgpt.com/#settings
2. Click on the "Data Controls" tab
3. Scroll to the bottom and click "Export data"
4. Wait for the email from OpenAI with your export link
5. Download the file when the email arrives
6. Unzip the downloaded file
7. Locate the `conversations.json` file in the extracted folder

#### Exporting from Claude

1. Visit: https://claude.ai/settings/data-privacy-controls
2. Scroll to the bottom of the page and click "Export data"
3. Wait for the email from Anthropic with your export
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
2. Select your `conversations.json` file (from either ChatGPT or Claude)
3. The app automatically detects the format and switches to the appropriate service tab
4. Your conversations are loaded and ready to search

You can load conversations from both services - just use the tabs at the top to switch between ChatGPT and Claude, then load each export file separately.

### Searching

- Use the search box at the top to search through all conversations
- Search works across conversation titles and message content
- **Multi-term search**: Use comma-separated terms to find conversations containing ALL terms
  - Example: `python, api, testing` finds only conversations that contain all three terms
  - Example: `machine learning, tensorflow` finds conversations about both topics
- Results update as you type
- Click "Clear" or press **Escape** to reset the search

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
- **Scroll to top**: When viewing long conversations, a button appears to quickly scroll back to the top
- **Service switching**: Toggle between ChatGPT and Claude conversations using the tabs at the top

### Keyboard Shortcuts

- **Up/Down Arrow Keys**: Navigate between conversations in the sidebar
- **Escape**: Clear the current search and return to all conversations
- **Tab**: Navigate through interface elements (buttons, search box, etc.)
- **Enter**: Select a conversation when focused

The interface intelligently switches between keyboard and mouse modes:
- Using arrow keys disables hover previews until you click again
- Clicking a conversation enables hover previews for mouse navigation

## Privacy & Security

This application prioritizes your privacy:

- **No server**: Runs entirely in your browser
- **No external connections**: Your data never leaves your device
- **No tracking**: No analytics or data collection
- **No storage**: Data is only kept in memory while the page is open

## Technical Details

### Supported File Formats

The tool automatically detects and supports:
- `conversations.json` from ChatGPT exports (OpenAI format)
- `conversations.json` from Claude exports (Anthropic format)

No manual format selection needed - just load your file and the app handles the rest!

### Browser Compatibility

- Chrome 90+
- Firefox 88+
- Safari 14+
- Edge 90+

### Technologies Used

- Pure HTML/CSS/JavaScript
- [Marked.js](https://marked.js.org/) for markdown rendering
- No other external dependencies

### Accessibility Features

This tool is built with accessibility in mind:
- **Screen reader support**: ARIA live regions announce search results, conversation selections, and file loads
- **Keyboard navigation**: Full keyboard support with arrow keys, Escape, and Tab
- **Focus indicators**: Clear visual focus states for all interactive elements
- **Semantic HTML**: Proper use of headings, landmarks, and ARIA labels
- **Skip links**: Quick navigation to main content
- **Reduced motion support**: Respects user's motion preferences

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

**Note**: This tool is not officially affiliated with Anthropic (Claude AI) or OpenAI (ChatGPT). It is an independent, open-source project designed to help you search and explore your own conversation exports.
