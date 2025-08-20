This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

frontend_web/
├── app/ # App Router (routes, layouts, metadata)
│ ├── layout.tsx # Root layout (shared UI, e.g. navbar, footer)
│ ├── page.tsx # Homepage
│ ├── dashboard/ # Example route (/dashboard)
│ │ ├── layout.tsx
│ │ ├── page.tsx
│ │ └── settings/
│ │ └── page.tsx
│ └── api/ # (Optional) Only for client-side helpers/proxy calls
│ └──
│
├── components/ # Reusable UI components
│ ├── ui/ # Atoms (buttons, inputs, modals, etc.)
│ ├── layout/ # Layout components (navbars, footers, sidebars)
│ └── forms/ # Form components (login, signup, profile forms)
│
├── lib/ # Client-side helpers (no DB here!)
│ ├── api.ts # API request functions (Axios/Fetch to .NET backend)
│ ├── auth.ts # Token handling, JWT helpers
│ └── utils.ts # Utility functions
│
├── hooks/ # Custom React hooks
│ └── useAuth.ts # Example: get logged-in user
│
├── context/ # Context providers (Theme, Auth, Global state)
│ └── ThemeContext.tsx
│
├── styles/ # Global styles (CSS/Tailwind)
│ └── globals.css
│
├── public/ # Static assets
│ └── logo.png
│
├── tests/ # Unit/integration tests
│
├── next.config.js
├── tailwind.config.js # use Tailwind css  
├── tsconfig.json
└── package.json
