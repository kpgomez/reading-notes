# Class 41: React 4

## Sources
- [Next.js - Dynamic Routes](https://nextjs.org/learn/basics/dynamic-routes)
- [Next.js - Deployment](https://nextjs.org/learn/basics/deploying-nextjs-app)
- [Video: Next.js 10 is here](https://www.youtube.com/watch?v=JWCS5IdECVI)

## Bookmark and Review
- [Next.js - Static File Serving](https://nextjs.org/docs/basic-features/static-file-serving)

## Reading Questions
1. Explain the concept of dynamic routes in Next.js and how they differ from static routes. [ChatGPT Prompt](https://chat.openai.com/c/c4f4d9e9-1a76-40fc-bba4-ca0064d8f509)
> Dynamic routes do not have a pre-defined endpoint. The route is generated dynamically. Dynamic routes are wrapped in square brackets indicating the route is not fixed. Static routes live in the "pages" directory.
2. Describe the process of deploying a Next.js application. What are the key steps involved, and what are some deployment platforms you can use? [ChatGPT Prompt](https://chat.openai.com/c/05fb7ffe-c9cd-4895-af10-ad9cf2ad40af)
> The key steps are 1) `$ npm run build` 2) configure package.json file 3) create .env (if needed) 4) choose deployment platform 5) configure deployment settings 6) deploy. Some popular deployment options include Vercel, Netlify, AWS Amplify, Heroku, and DigitalOcean.
3. How does Next.js handle static file serving? Discuss the default folder structure for storing static assets and explain how to reference them in a Next.js application. [ChatGPT Prompt](https://chat.openai.com/c/23e261c9-755c-424f-a3b0-686a7d029388)
> The default folder is "public". Reference it by using "/public" prefix. 

## Things I want to learn more about

- Code splitting
