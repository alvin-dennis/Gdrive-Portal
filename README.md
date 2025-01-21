# Gdrive - Portal

This project is a modern web application built with Next.js, featuring a sleek UI powered by Tailwind CSS and shadcn/ui components, with secure authentication provided by NextAuth. This is used to create a structured organizational web portal to edit/write/access Google Drive files

## Features

- **Next.js**: A React framework for production-grade applications with server-side rendering and static site generation.
- **Tailwind CSS**: A utility-first CSS framework for rapid UI development.
- **shadcn/ui**: A collection of re-usable components built with Radix UI and Tailwind CSS.
- **NextAuth**: A complete authentication solution for Next.js applications.

## Prerequisites

Before you begin, ensure you have the following installed on your local machine:

- Node.js (v14.0.0 or later)
- npm (v6.0.0 or later)

## Getting Started

To get the project up and running on your local machine, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/your-project-name.git
   cd your-project-name
   ```

2. Install the dependencies:
   ```bash
   npm install
   ```

3. Set up your environment variables:
   Create a `.env.local` file in the root directory and add the following variables:
   ```
   NEXTAUTH_URL=http://localhost:3000
   NEXTAUTH_SECRET=your_nextauth_secret
   # Add any other required environment variables for your authentication providers
   ```

4. Run the development server:
   ```bash
   npm run dev
   ```

5. Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

## Project Structure

```
├── app/
│   ├── api/
│   │   └── auth/
│   │       └── [...nextauth]/
│   │           └── route.ts
│   ├── components/
│   ├── layout.tsx
│   └── page.tsx
├── lib/
│   └── auth.ts
├── styles/
│   └── globals.css
├── .env.local
├── next.config.js
├── package.json
├── postcss.config.js
├── tailwind.config.js
└── tsconfig.json
```

## Configuration

### Tailwind CSS

Tailwind CSS is configured in the `tailwind.config.js` file. You can customize your design tokens, add new utility classes, or modify existing ones here.

### shadcn/ui

shadcn/ui components are pre-configured and ready to use. You can find and customize these components in the `app/components/ui` directory.

### NextAuth

NextAuth is set up in `app/api/auth/[...nextauth]/route.ts`. Add your authentication providers and customize your authentication flow here.

## Adding New Pages

To add a new page, create a new file in the `app` directory. Next.js uses file-based routing, so the file name will determine the route.

## Styling

This project uses Tailwind CSS for styling. You can add custom styles in the `styles/globals.css` file or directly in your components using Tailwind's utility classes.

## Deployment

This project can be easily deployed on platforms like Vercel or Netlify. Follow their respective documentation for deploying Next.js applications.

## Learn More

To learn more about the technologies used in this project, check out the following resources:

- [Next.js Documentation](https://nextjs.org/docs)
- [Tailwind CSS Documentation](https://tailwindcss.com/docs)
- [shadcn/ui Documentation](https://ui.shadcn.com)
- [NextAuth Documentation](https://next-auth.js.org)

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License.