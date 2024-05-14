# Next.js with supabase auth

This is a super simple Next.js Supabase auth setup. I followed the tutorial under:  
[Setting up Server-Side Auth for Next.js](https://supabase.com/docs/guides/auth/server-side/nextjs) and  
[Build a User Management App with Next.js](https://supabase.com/docs/guides/getting-started/tutorials/with-nextjs?queryGroups=language&language=js)

It's a mix of both. 🥳

Next.js Version: 14.2.3  
supabase-js Version: 2.43.1
supabase-ssr Version: 0.3.0

## Important!

Please change the auth confirmation part in the email template as described (Step 6)  
in the [Setting up Server-Side Auth for Next.js](https://supabase.com/docs/guides/auth/server-side/nextjs).

```bash
Go to the Auth templates page in your dashboard. In the Confirm signup template,
change {{ .ConfirmationURL }} to
{{ .SiteURL }}/auth/confirm?token_hash={{ .TokenHash }}&type=signup.
```

## Getting Started

First, install the dependencies:

```bash
npm install
# or
yarn install
# or
pnpm install
```

Then, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.
