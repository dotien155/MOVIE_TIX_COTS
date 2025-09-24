# Movie Frontend - do an DTU

Day la du an frontend su dung [Next.js](https://nextjs.org) duoc tao boi [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

Ung dung nay la giao dien quan li rap phim, ket hop tri tue nhan tao (AI) va chatbox ho tro khach hang trong viec dat ve, xem phim va tu van thong tin.

## Bat dau

Truoc tien, chay server phat trien:

```bash
npm run dev 
# hoac
yarn dev
# hoac
pnpm dev
# hoac
bun dev
## cấu trúc dự án
src/
├── app/                    # Next.js App Router
│   ├── (default)/         # Default layout group
│   │   ├── page.tsx       # Home page with movie listings
│   │   ├── HomeClient.tsx # Client-side home component
│   │   ├── movies/        # Movie-related pages
│   │   │   ├── page.tsx   # Movies listing page
│   │   │   └── [id]/      # Movie detail pages
│   │   ├── booking/       # Booking flow
│   │   │   └── [movieId]/ # Seat selection page
│   │   ├── checkout/      # Payment checkout
│   │   │   └── page.tsx   # Customer info & payment
│   │   └── confirmation/  # Booking confirmation
│   │       └── page.tsx   # Success page with ticket
│   ├── globals.css        # Global styles and Tailwind
│   └── layout.tsx         # Root layout with providers
├── components/            # Reusable components
│   ├── ui/               # Basic UI components
│   ├── skeletons/        # Loading skeleton components
│   │   ├── HomeSkeleton.tsx
│   │   ├── MovieSkeleton.tsx
│   │   ├── ArticleSkeleton.tsx
│   │   └── CommonSkeleton.tsx
│   └── test/             # Development test components
├── types/                # TypeScript definitions
│   ├── global-type.ts    # Main type definitions
│   └── format-price.ts   # Price formatting utilities
├── lib/                  # Utility functions
├── public/              # Static assets
│   ├── images/          # Image assets
│   └── icons/           # Icon files
└── docs/                # Documentation
    └── SKELETON_LOADING.md
