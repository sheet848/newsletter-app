# AI Newsletter App

A Next.js application for creating AI-powered newsletters with Supabase backend.

## Features

- 🤖 AI-powered newsletter generation using OpenAI
- 📧 Email subscriber management
- 💾 Database storage with Supabase
- ✏️ Rich text newsletter editor
- 📱 Responsive design with Tailwind CSS
- 🔒 Row Level Security with Supabase Auth

## Tech Stack

- **Frontend:** Next.js 14, React 18, Tailwind CSS
- **Backend:** Next.js API Routes
- **Database:** Supabase (PostgreSQL)
- **AI:** OpenAI GPT-3.5-turbo
- **Icons:** Lucide React

## Getting Started

### Prerequisites

- Node.js 18+ installed
- Supabase account and project
- OpenAI API key

### Installation

1. Clone the repository:
```bash
git clone <your-repo-url>
cd ai-newsletter-app
```

2. Install dependencies:
```bash
npm install
```

3. Set up environment variables:
Create a `.env.local` file in the root directory:
```bash
NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
OPENAI_API_KEY=your_openai_api_key
```

4. Set up Supabase database:
- Go to your Supabase dashboard
- Run the SQL migrations provided in the code
- Enable Row Level Security on tables

5. Run the development server:
```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to view the app.

## Usage

1. **Generate Newsletter:** Enter a topic and select a tone to generate AI-powered content
2. **Edit Content:** Use the editor to modify the generated content
3. **Save Draft:** Save your work as a draft
4. **Publish:** Publish the newsletter
5. **Manage Subscribers:** Users can subscribe via the subscription form

## Project Structure

```
ai-newsletter-app/
├── components/           # React components
│   ├── NewsletterGenerator.js
│   ├── NewsletterEditor.js
│   └── SubscriberForm.js
├── lib/                 # Utility functions
│   ├── supabase.js      # Supabase client
│   └── openai.js        # OpenAI integration
├── pages/               # Next.js pages
│   ├── api/             # API routes
│   │   ├── generate-newsletter.js
│   │   └── subscribe.js
│   └── index.js         # Home page
├── styles/              # CSS styles
│   └── globals.css
└── public/              # Static assets
```

## API Endpoints

- `POST /api/generate-newsletter` - Generate AI newsletter content
- `POST /api/subscribe` - Subscribe email to newsletter

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

MIT License