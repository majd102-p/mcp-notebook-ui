![MIT License](https://img.shields.io/badge/license-MIT-green.svg)
![Vanilla JS](https://img.shields.io/badge/Vanilla-JavaScript-yellow.svg)
![Vercel](https://img.shields.io/badge/deploy-Vercel-black.svg?logo=vercel)
![Notion Ready](https://img.shields.io/badge/Notion-Embed%20Ready-blueviolet.svg)
![Status](https://img.shields.io/badge/status-production--ready-brightgreen.svg)

# 📓 Model Context Protocol (MCP) - Developer Reference Book
👤 Author: Majd Majdi Ayoub  
🔗 GitHub: @majd102-p  
🤗 Hugging Face: @Ma120  
💼 LinkedIn: Majd Ayoub  

A single-page, responsive developer reference notebook for the Model Context Protocol (MCP). This project is styled with a dark developer documentation theme and is built with vanilla web technologies to remain fully functional and lightweight when nested inside a Notion /embed block or hosted statically.

⚡ Live Demo: [https://mcp-notebook-ui-git-main-majd102-ps-projects.vercel.app](https://mcp-notebook-ui-git-main-majd102-ps-projects.vercel.app/)


 Notion: https://www.notion.so/Model-Context-Protocol-MCP-Developer-Notebook-363402a71ca08031a7c1cd4b4e17ff97?source=copy_link

✨ Features & Interactivity

🔍 Local Search (Ctrl+K / ⌘K): A keyboard-accessible spotlight search that filters and links to text segments instantly.

📂 Smart Sidebar: Automatically expands and highlights active chapters based on scroll position (Scrollspy).

💡 Explanatory Hover Tooltips: Contextual tooltips explaining technical terms (JSON-RPC, Roots, Sampling, stdio, realpath, FastMCP) on hover or touch.

🛠️ HTML/CSS System Simulators: Lightweight, non-blocking visual flow maps built with pure CSS and Tailwind classes:

Protocol Simulator (Section 2): Visualizes packet flow steps from server to client and LLM.

Roots Validation Playground (Section 4.1): Simulates path validation and shows realpath traversal blocks.

Handshake Timeline (Section 5.1): Staggered sequence layout showing handshake progression.

Scaling Map (Section 10.1): Displays routing through load balancers and syncing state to Redis.

📋 Code Highlighting & Clipboard: Prism.js syntax highlighting with quick copy-to-clipboard buttons.

📚 Technical Chapters Covered

The guide contains structured documentation on:

Core Concepts: Distinguishing between Protocol-level Sampling and LLM-level Decoding ($temperature$, $top\_p$).

Sampling Workflow: Execution loops and authorization boundaries.

Delegated Sampling Trade-offs: Economic factors, safety layers, and server complexity reductions.

Roots & Filesystem Security: Canonical validation guidelines, traversal prevention, and STRIDE Threat Modeling.

JSON-RPC 2.0 message schemas: Separation of conceptual schemas from strict production standards.

Handshake Lifecycle: Capabilities negotiation and sequence progression.

Communication Transports: Same-machine stdio subprocess stream pipes vs. remote networks.

Deep Dive Streamable HTTP: Session ID rules, persistent SSE channels, and stateless FastMCP deployments.

Decision Matrix: Practical transport choice matrices.

HA Production Scaling: Load balancing desynchronization issues and shared caching (Redis) architectures.

Reflections on Advanced Applications: UX priorities and multi-turn architectural design considerations.

Recommended Production Stack: Minimalist ASGI (Uvicorn), Fargate, Redis, and OpenTelemetry orchestration guidelines.

💻 Running Locally

Since the application is fully self-contained, no external local packages or node build setups are required:

Clone the repository:

git clone https://github.com/majd102-p/mcp-notebook-ui.git
cd your-repo-name


Open directly in your browser:
Double-click index.html or run a lightweight local static server:

# Python 3
python -m http.server 8000


Navigate to http://localhost:8000.

🛠️ Built With

Pure HTML5 & Vanilla JavaScript: Zero JS framework dependencies to guarantee low load times inside iframe containers.

Tailwind CSS (Premium dark developer theme)

FontAwesome 6 (Technical SVG iconography)

Prism.js (Syntax highlighter)

Inter & JetBrains Mono (Google Fonts)

📄 License

This project is licensed under the MIT License.
