<p align="center"><a href="https://www.codechefvit.com" target="_blank"><img src="https://i.ibb.co/4J9LXxS/cclogo.png" width="160" title="CodeChef-VIT" alt="Codechef-VIT"></a></p>

<h2 align="center">Cookoff X Admin</h2>
<br/>

> Cookoff is CodeChef VIT’s flagship competitive programming event that challenges developers across the country. This repository contains the Admin Portal for Cookoff X — the single interface for managing users, problems, testcases, rounds, judging operations, and event monitoring.

## 🌐 Deploy

(Replace with production URL)  
[https://cookoffx-admin.codechefvit.com](https://cookoffx-admin.codechefvit.com)

## ⚙️ Tech Stack:

- [Next.js](https://nextjs.org/)
- [TypeScript](https://www.typescriptlang.org/)
- [Tailwind CSS](https://tailwindcss.com/)
- [TanStack Query](https://tanstack.com/query/latest)
- [Shadcn UI](https://ui.shadcn.com/)
- [Zod](https://zod.dev/)
- [React Hook Form](https://react-hook-form.com/)
- [Axios](https://axios-http.com/)

<!-- ## 🖼 Screenshots

<p align="center">

</p> -->

## 🔧 Features

- Authentication & Access Control:
  - Secure admin-only login
  - Role-based feature gating (Super Admin, Problem Setter, Judge, Observer)
- User Management:
  - Paginated + searchable table
  - Ban / unban
  - Bulk round promotion
- Question Management:
  - CRUD with rich editor / markdown preview
  - Difficulty, tags, constraints metadata
- Testcase Management:
  - List, create, update, delete
  - Distinguish sample vs hidden
  - Bulk import (planned)
- Round / Contest Control:
  - Schedule management
  - Freeze scoreboard (planned)
- Judge / Evaluation (planned):
  - Rejudge flow
  - Queue monitoring
- Observability (optional):
  - Submission analytics
  - Audit log
- Performance:
  - Query caching & background refresh
  - Optimistic updates for UI responsiveness

<p align="center">

#### Login Page
<img width="1440" alt="login" src="/showcase_ss/login_page.png">

### Portal

#### Dashboard
<img width="1440" alt="dashboard" src="/showcase_ss/dashboard_page.png">

#### Edit Question Page
<img width="1440" alt="edit-question" src="/showcase_ss/edit_question_page.png">

#### Question Creation Page
<img width="1440" alt="create-question" src="/showcase_ss/question_creation_page.png">

#### Question Page
<img width="1440" alt="question" src="/showcase_ss/question_page.png">
<img width="1440" alt="testcases" src="/showcase_ss/testcase_question_page.png">

#### Users Page
<img width="1440" alt="users" src="/showcase_ss/users_page.png">

</p>

## 🏁 Get Started

Clone:

```bash
git clone -b main https://github.com/<your-username>/cookoff-admin-X.git
cd cookoff-admin-X
```

Install:

```bash
pnpm install
# or
npm install
```

Environment (create `.env.local`):

```bash
NEXT_PUBLIC_API_BASE_URL=https://api.cookoffx.codechefvit.com
NEXT_PUBLIC_EVENT_CODE=COOKOFFX
ADMIN_AUTH_ISSUER=https://auth.cookoffx.codechefvit.com
ADMIN_AUTH_CLIENT_ID=XXXX
ADMIN_AUTH_SECRET=XXXX
NEXT_PUBLIC_ENABLE_REALTIME=false
```

Run:

```bash
pnpm dev
```

Build:

```bash
pnpm build && pnpm start
```

Suggested structure:

```
/app
/components
/services
/hooks
/lib
/types
/showcase_ss
```

## 📝 Checkout:

- Backend (update with current year’s backend repo once available)  
  Previous cycle example: https://github.com/CodeChefVIT/cookoff-9.0-backend
- Participant Portal (update when ready)  
  Previous example: https://github.com/CodeChefVIT/cookoff-portal-9.0

## 🤝 Contribution Workflow

1. Branch naming: `feat/<scope>-<short-desc>` (e.g. `feat/users-bulk-promote`)
2. Conventional commits: `feat: add bulk user promotion`
3. Run checks:
   ```bash
   pnpm lint
   pnpm typecheck
   pnpm format
   ```
4. Open PR with screenshots for UI changes.

## 🧪 Scripts

```bash
pnpm dev
pnpm lint
pnpm typecheck
pnpm format
pnpm build
```

## ✅ Quality & Security

- Schema validation via Zod
- Protected routes with server session guard
- Role-based gating for destructive actions
- Avoid logging sensitive data
- API abstraction in `/services`

## 🧱 Roadmap

- Live scoreboard monitor
- Real-time judge queue depth
- Dark mode toggle
- Bulk user CSV import/export
- Rejudge workflow UI
- Anomaly detection (suspicious behavior)
- Email / webhook notifications

## 🚀 Contributors (Alphabetical)

(Alphabetical order by display name)

<table>
<tr align="center">

<td>
	<p align="center">
		<img src="https://avatars.githubusercontent.com/u/56132559?v=4" width="200" height="200" alt="Abhinav Ganeshan" style="border: 2px solid grey; width:170px; height:170px">
	</p>
	<p style="font-size:17px; font-weight:600;">Abhinav Ganeshan</p>
	<p align="center">
		<a href="https://github.com/Abh1noob">
			<img src="http://www.iconninja.com/files/241/825/211/round-collaboration-social-github-code-circle-network-icon.svg" width="36" height="36" alt="GitHub"/>
		</a>
	</p>
</td>

<td>
	<p align="center">
		<img src="https://avatars.githubusercontent.com/u/67090539?v=4" width="200" height="200" alt="Abhinav Pant" style="border: 2px solid grey; width:170px; height:170px">
	</p>
	<p style="font-size:17px; font-weight:600;">Abhinav Pant</p>
	<p align="center">
		<a href="https://github.com/abhitrueprogrammer">
			<img src="http://www.iconninja.com/files/241/825/211/round-collaboration-social-github-code-circle-network-icon.svg" width="36" height="36" alt="GitHub"/>
		</a>
	</p>
</td>

<td>
	<p align="center">
		<img src="https://avatars.githubusercontent.com/u/83698727?v=4" width="200" height="200" alt="Advik Gupta" style="border: 2px solid grey; width:170px; height:170px">
	</p>
	<p style="font-size:17px; font-weight:600;">Advik Gupta</p>
	<p align="center">
		<a href="https://github.com/Advik-Gupta">
			<img src="http://www.iconninja.com/files/241/825/211/round-collaboration-social-github-code-circle-network-icon.svg" width="36" height="36" alt="GitHub"/>
		</a>
	</p>
</td>

</tr>
</table>

<!-- Add more contributor <td> blocks as needed -->

## License

[![License](http://img.shields.io/:license-mit-blue.svg?style=flat-square)](http://badges.mit-license.org)

<p align="center">
	Made with ❤️ by <a href="https://www.codechefvit.com" target="_blank">CodeChef-VIT</a>
</p>
