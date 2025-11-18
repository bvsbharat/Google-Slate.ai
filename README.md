<div align="center">
<img width="1200" height="475" alt="GHBanner" src="./assets/Demo.png" />
</div>

# Slate.ai - AI-Powered Assisted Learning Platform

> **Bringing back the personalized, hand-in-hand learning experience of your childhood**


# Run and deploy your AI Studio app

This contains everything you need to run your app locally.

View your app in AI Studio: https://ai.studio/apps/drive/1EwcfBx_l1uIGXCw9S3eIUz6Tynn3G8h8

## 🎯 The Problem

Education is the main pillar for anyone to grow in their life, and if it is provided in a better way, everyone grows and achieves what they want. When we are young, we learn on a slate with our parents or teachers holding our hands and guiding us. But as we grow, we rely on books, iPads, and other digital resources. We become hesitant to ask questions, unsure if what we are learning is correct, and we lack a suggested, personalized way of learning.

## 💡 Our Solution: Slate.ai

**Slate.ai** is an AI-powered assisted learning platform designed to bring back the personalized, hand-in-hand learning experience of our childhood. This is **Assisted Learning** with a canvas-like experience where you get the nostalgia of learning when you're a kid on a slate and your parent or teacher holds your hand to teach you.

It acts as a virtual teacher, guiding you through your learning journey, providing assistance, and creating a safe space to learn and grow without the fear of making mistakes. Our goal is to make learning intuitive, interactive, and effective for everyone.

## ✨ Key Features

### 🎨 Interactive Canvas Experience
- **TLDraw-powered whiteboard** for natural writing and drawing
- Real-time collaboration with AI tutor
- Support for text, diagrams, code, and multimedia content
- Auto-generated initial code templates for coding problems

### 🤖 AI-Powered Learning Assistant
- **Real-time voice interaction** using Google Gemini 2.5 Flash with native audio
- **Multimodal understanding** - AI can see your canvas and provide contextual help
- **Smart interruption handling** - AI stops when you start speaking
- **Canvas monitoring** - AI tracks your progress and provides feedback

### 📚 Multi-Subject Support
- **Algorithms & Coding** - JavaScript practice with code execution and test cases
- **Mathematics** - Problem-solving with visual explanations
- **Science** - Physics, chemistry, and more with diagrams
- **Import Any Problem** - Screen capture, camera, or image upload support

### 🎥 Rich Media Generation
- **AI-generated diagrams** using Fal AI for visual explanations
- **8-second educational videos** using Google Veo 3.1 for animated concepts
- **Story-based animations** with cinematic prompts for better understanding

### 🧪 Interactive Learning Tools
- **Hint system** - Get help without revealing the solution
- **Code execution** - Run JavaScript code directly in the browser
- **Test cases** - Validate algorithm solutions automatically
- **Answer validation** - AI evaluates your work and provides feedback
- **Sticky notes** - AI adds helpful hints on your canvas

### 📊 Personalized Learning
- **Topic selection** across multiple subjects
- **Difficulty adaptation** based on your level
- **Progress tracking** with session history
- **Detailed feedback** with strengths and improvements

## 🛠️ Technology Stack

### Frontend
- **React 18.3.1** - UI framework
- **TypeScript 5.8.2** - Type-safe development
- **Vite 6.2.0** - Fast build tool and dev server
- **TLDraw 3.13.1** - Infinite canvas for drawing and writing
- **TailwindCSS** - Utility-first styling (via tailwind-merge & clsx)

### AI & Machine Learning
- **Google Gemini 2.5 Flash** - Real-time voice interaction with native audio
- **Google Gemini 2.5 Pro** - Advanced problem generation and validation
- **Google Gemini Vio** - Vision capabilities for canvas understanding
- **Fal AI** - Image generation for educational diagrams
- **Google Veo 3.1** - Video generation for animated explanations (via Fal AI)

### Development Tools
- **Node.js** - Runtime environment
- **npm** - Package management

## 🏗️ Architecture

Slate.ai uses a sophisticated AI-powered architecture that combines **Google Gemini Pro** for intelligent question generation and planning, **Gemini Live API** for real-time voice interaction, and **Fal AI** (powered by Google Imagen & Veo) for multimedia content generation.

<div align="center">
<img src="./assets/image.png" alt="Slate.ai Architecture Diagram" width="800"/>
</div>

### Architecture Flow

1. **User Input** → User provides any question or topic they want to learn
2. **Planning & Generation** → Gemini 2.5 Pro creates:
   - Complete question set with examples
   - Unit tests for validation
   - Learning objectives
3. **Interactive Canvas** → TLDraw workspace where user works on solutions
4. **Real-time Agent** → Gemini Live API (2.5 Flash) provides:
   - Voice-based hints and suggestions
   - Code guidance and debugging help
   - Conceptual explanations
5. **Multimedia Generation** → On-demand content via Fal AI:
   - **Images**: Google Imagen generates educational diagrams
   - **Videos**: Google Veo 3.1 creates animated concept explanations
6. **Validation & Feedback** → Gemini 2.5 Pro evaluates solutions and provides detailed feedback

### Key Components

- **App.tsx** - Main application orchestrator
- **Slate.tsx** - Canvas component with TLDraw integration
- **useGeminiLive.ts** - Real-time AI voice interaction hook
- **geminiService.ts** - Problem generation and validation
- **videoService.ts** - Educational video generation
- **FloatingAIAvatar** - Voice assistant UI
- **LeftSidebar** - Navigation and action controls
- **StudyTopicsPanel** - Subject and topic selection

## 🚀 Getting Started

### Prerequisites

- **Node.js** (v16 or higher)
- **npm** or **yarn**
- **Google Gemini API Key** - Get from [Google AI Studio](https://ai.google.dev/)
- **Fal AI API Key** - Get from [Fal AI](https://fal.ai/)

### Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd Google-Slate.ai
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   
   Create a `.env.local` file in the root directory:
   ```env
   API_KEY=your_gemini_api_key_here
   FAL_API_KEY=your_fal_api_key_here
   ```

4. **Run the development server**
   ```bash
   npm run dev
   ```

5. **Open your browser**
   
   Navigate to `http://localhost:5173` (or the port shown in your terminal)

### Building for Production

```bash
npm run build
npm run preview
```

## 📖 How to Use

1. **Select a Subject** - Choose from Algorithms, Math, Science, or import your own problem
2. **Pick a Topic** - Select what you want to learn
3. **Start Learning** - The AI generates a personalized problem for you
4. **Connect Voice Assistant** - Click the floating avatar to start voice interaction
5. **Work on Canvas** - Write, draw, or code your solution
6. **Get Help** - Ask for hints, request visual explanations, or generate videos
7. **Validate** - Run tests (for code) or check your answer (for math/science)
8. **Review Feedback** - Learn from AI's detailed evaluation

## 🎓 Supported Learning Modes

### Practice Mode
- Work at your own pace
- Get unlimited hints
- Interactive feedback
- No pressure environment

### Exam Mode (Coming Soon)
- Timed challenges
- Limited hints
- Performance scoring
- Progress tracking

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is licensed under the MIT License.

## 🙏 Acknowledgments

- **Google Gemini** for powerful AI capabilities
- **Fal AI** for media generation services
- **TLDraw** for the amazing canvas library
- **Vite** for blazing-fast development experience


<div align="center">
<img width="1200" height="475" alt="GHBanner" src="https://github.com/user-attachments/assets/0aa67016-6eaf-458a-adb2-6e31a0763ed6" />
</div>

# Run and deploy your AI Studio app

This contains everything you need to run your app locally.

View your app in AI Studio: https://ai.studio/apps/drive/1EwcfBx_l1uIGXCw9S3eIUz6Tynn3G8h8

## 📞 Support

For questions or issues, please open an issue on GitHub.

---

**Made with ❤️ for learners everywhere**
