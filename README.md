# LuminaPDF — AI-Powered PDF Reader & QA Studio

**LuminaPDF** is a modern, high-performance web application designed for reading, exploring, and chatting with PDF documents with seamless AI grounded Question-Answering, page-by-page citations, voice readout, and interactive document insights.

---

## ✨ Key Highlights & Features

### 1. 📖 Interactive Dual-Pane PDF Reader
- **High-DPI Razor-Sharp Rendering**: Utilizes Mozilla PDF.js canvas rendering tuned with retina device pixel ratio support.
- **Visual Thumbnail Sidebar**: Fast thumbnail drawer to preview and jump to any page in the document.
- **Real-Time Document Search**: Full-text keyword search across all pages with match counters and jump-to-result controls.
- **Zoom & View Presets**: Zoom In/Out, Fit-to-Width, Fit-to-Page, and 100% reset.
- **Contextual Selection Tooltip**: Highlight any text in the PDF to reveal a floating action menu: **"Ask AI about this"** or **"Copy Text"**, immediately piping the excerpt into the chat assistant.

### 2. 🤖 Grounded AI Question-Answering & Deep Citations
- **Dual-Engine Architecture**:
  - **Gemini 2.5 Flash / Pro Integration**: Connect your Google Gemini API Key for deep reasoning, multi-turn conversational comprehension, and synthesis.
  - **Built-in Local Semantic Engine**: Works **100% offline with zero setup**! Automatically tokenizes, extracts, and matches page content with BM25 / TF-IDF scoring and grounded evidence.
- **Interactive Page Citations**: Every assistant answer cites exact page numbers (e.g., `[Page 2]`). Clicking the badge automatically scrolls the PDF reader directly to that page and flashes an indicator glow.
- **Document Insights Card**: Automatically extracts key statistics (percentages, savings, clinical rates) and provides recommended prompt questions.
- **Audio Voice Readout (TTS)**: Listen to answers aloud using the Web Speech Synthesis API.
- **Conversation Management**: Export chat sessions as Markdown (`.md`) or clear thread history.

### 3. 🎨 Modern Glassmorphic UI & Flow
- Sleek dark and light mode toggle.
- Fluid responsive layout with auto-collapsible panels and mobile-friendly tab navigation.
- Built-in 1-Click Sample Research Document ("Autonomous AI Agents in Healthcare: 2026 Strategic Overview") so you can test all features immediately without finding a PDF.

---

## 🚀 Getting Started

### Prerequisites
- Node.js (v18+)
- npm or pnpm

### Running Locally
```bash
# Navigate to the project directory
cd C:\Users\us031\.gemini\antigravity\scratch\pdf-ai-reader

# Install dependencies (already installed)
npm install

# Start development server
npm run dev
```

Open your browser at **[http://localhost:5173](http://localhost:5173)**.

---

## ⚙️ Connecting Google Gemini (Optional)

1. Open the app and click the **Settings** icon (or the engine status pill in the top-right).
2. Enter your API key from [Google AI Studio](https://aistudio.google.com/app/apikey).
3. Click **Test** to verify connection, then **Save Preferences**.
4. The status pill will switch to **Gemini AI Active**!
