# CMS Blog

A modern, full-featured blog application built with Next.js 15 and powered by GraphCMS (Hygraph). Features a responsive design with Tailwind CSS, dynamic content management, and interactive user engagement.

## ✨ Features

- 📝 **Dynamic Blog Posts** - Rich content powered by GraphCMS with GraphQL API
- 🏷️ **Category System** - Organize posts by categories
- 💬 **Comments System** - User engagement with comment functionality
- 👤 **Author Profiles** - Detailed author information and bios
- 🎨 **Featured Posts Carousel** - Showcase highlighted content
- 📱 **Responsive Design** - Mobile-first approach with Tailwind CSS
- ⚡ **Static Generation** - Optimized performance with SSG
- 🔍 **Related Posts Widget** - Smart content recommendations
- 📅 **Date Formatting** - Beautiful date displays with date-fns

## 🛠️ Tech Stack

- **Framework:** [Next.js 15.5.9](https://nextjs.org/)
- **React:** 19.0.0
- **CMS:** GraphCMS (Hygraph) with GraphQL
- **Styling:** Tailwind CSS 3.4.17
- **Language:** JavaScript/TypeScript 5.7.2
- **Date Handling:** date-fns 4.1.0
- **GraphQL Client:** graphql-request 7.1.2
- **Carousel:** react-multi-carousel 2.8.5

## 📦 Installation

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd cmsblog
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**

   Create a `.env` file in the root directory:
   ```env
   NEXT_PUBLIC_GRAPHCMS_ENDPOINT=your_graphcms_endpoint
   GRAPHCMS_TOKEN=your_graphcms_token
   ```

4. **Run the development server**
   ```bash
   npm run dev
   ```

   Open [http://localhost:3000](http://localhost:3000) in your browser.

## 🚀 Scripts

- `npm run dev` - Start development server
- `npm run build` - Build for production
- `npm start` - Start production server

## 📁 Project Structure

```
cmsblog/
├── components/          # React components
│   ├── Author.jsx      # Author profile component
│   ├── Categories.jsx  # Categories widget
│   ├── Comments.jsx    # Comments display
│   ├── CommentsForm.jsx # Comment submission form
│   ├── FeaturedPostCard.jsx # Featured post card
│   ├── Header.jsx      # Site header
│   ├── Layout.jsx      # Main layout wrapper
│   ├── PostCard.jsx    # Blog post card
│   ├── PostDetail.jsx  # Full post view
│   └── PostWidget.jsx  # Related posts widget
├── pages/              # Next.js pages
│   ├── api/           # API routes
│   ├── category/      # Category pages
│   ├── post/          # Individual post pages
│   └── index.js       # Homepage
├── sections/           # Page sections
│   └── FeaturedPosts.jsx
├── services/           # API service layer
│   └── index.js       # GraphQL queries
├── styles/            # Global styles
│   └── globals.scss
└── public/            # Static assets
```

## 🔧 Configuration

### Next.js Config
- Modern image optimization with `remotePatterns`
- React Strict Mode enabled
- Configured for GraphCMS image hosting

### TypeScript Config
- Modern module resolution (`bundler`)
- Strict type checking enabled
- ES5 target with ESNext modules

## 🎨 Components

### Core Components
- **Layout** - Main application wrapper with header
- **PostCard** - Preview card for blog posts
- **PostDetail** - Full post content with rich text rendering
- **Categories** - Dynamic category navigation
- **PostWidget** - Similar/recent posts sidebar
- **Author** - Author bio and avatar
- **Comments** - Comment display and management
- **CommentsForm** - User comment submission
- **FeaturedPosts** - Carousel of featured content

## 📡 API Routes

### `/api/comments`
POST endpoint for submitting new comments
- Accepts: name, email, comment, slug
- Uses GraphQL mutation to create comments

## 🌐 GraphQL Integration

The project uses GraphCMS (Hygraph) as a headless CMS with GraphQL API:
- Fetches posts, categories, and comments
- Handles post filtering and relationships
- Supports featured posts and related content

## 📝 Content Management

1. Set up your GraphCMS project
2. Create content models for:
   - Posts (with title, excerpt, content, featured image)
   - Authors (with name, bio, photo)
   - Categories
   - Comments
3. Configure API access and tokens
4. Update environment variables

## 🚀 Deployment

### Build for Production
```bash
npm run build
```

### Deploy to Vercel
The easiest way to deploy is using [Vercel](https://vercel.com):
```bash
vercel
```

Or connect your GitHub repository to Vercel for automatic deployments.


## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!

## 📧 Contact

For questions or support, please open an issue in the repository.
