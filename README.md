# AI Poet Chatbot 🎭

An interactive chatbot trained on the poetry of [Halim Madi](https://www.halimmadi.com). This AI-powered poetry companion brings Halim's unique poetic voice to life through natural conversation.

## ✨ Features

- 🤖 Chat with an AI trained on Halim Madi's poetry
- 🎙️ Voice input support with speech-to-text
- 🔊 Text-to-speech for AI responses
- 💬 Real-time message streaming
- 📱 Responsive design
- ⚡ Server-side API handling for security

## 🛠️ Technology Stack

- **Frontend**: Next.js 14, React 18, TypeScript
- **Styling**: Tailwind CSS
- **AI Integration**: OpenAI API
  - GPT-3.5 Turbo (Fine-tuned model)
  - Whisper API for speech-to-text
  - TTS-1 for text-to-speech
- **Icons**: Lucide React

## 🚀 Getting Started

### Prerequisites

- Node.js 18.0 or later
- OpenAI API key

### Environment Setup

1. Clone the repository
2. Create a `.env` file in the root directory with:
   ```env
   OPENAI_API_KEY=your_openai_api_key
   NEXT_PUBLIC_OPENAI_API_KEY=your_openai_api_key
   ```

### Installation

```bash
# Install dependencies
npm install

# Start development server
npm run dev
```

The application will be available at `http://localhost:3000`

## 🌟 Usage

1. **Text Chat**: Type your message in the input field and press send
2. **Voice Input**: 
   - Click the microphone icon to start recording
   - Speak your message
   - Click the stop button to end recording
3. **Text-to-Speech**: Click the speaker icon on any AI response to hear it spoken

## 🔒 Security Features

- Server-side API route for OpenAI chat completions
- Secure environment variable handling
- Client-side API key limited to speech features only

## 📦 Project Structure

```
├── src/
│   ├── app/
│   │   ├── api/
│   │   │   └── chat/
│   │   │       └── route.ts    # API endpoint for chat
│   │   ├── page.tsx            # Main chat interface
│   │   ├── layout.tsx          # Root layout
│   │   └── globals.css         # Global styles
│   └── ...
├── public/
├── .env
├── next.config.mjs
├── package.json
└── ...
```

## 🚀 Deployment

The application can be deployed on Vercel:

1. Push your code to a Git repository
2. Import the project in Vercel
3. Add environment variables:
   - `OPENAI_API_KEY` (for server-side API calls)
   - `NEXT_PUBLIC_OPENAI_API_KEY` (for client-side speech features)
4. Deploy

## 📝 License

MIT

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!
