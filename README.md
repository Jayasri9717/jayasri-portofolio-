# Jayasri's editable portfolio

React + TypeScript + Vite portfolio with a light/dark mode toggle and emerald-teal styling.

## Run locally (Windows PowerShell)

Open this folder in VS Code, then run:

```powershell
npm.cmd install
npm.cmd run dev
```

Open the local address Vite prints (usually `http://localhost:5173/`). Keep the terminal open while using the site.

## Update your portfolio easily

**Most edits happen in one file: `src/portfolioData.ts`.** Open it in VS Code and update the text or arrays, then save. The browser refreshes automatically.

- Personal information: name, role, college, email, GitHub, LinkedIn, headline and introduction.
- Skills: edit items in `skills`.
- Projects: edit items in `projects`. The `repo` value should match the repository name on GitHub.
- Awards and hackathon participation: edit items in `achievements`. Keep prizes and participation clearly distinguished.
- Certificates: add items to `certificates`, with title, issuer, date, and optional file path.

### Add a certificate image or PDF

1. Create `public/certificates` if it does not exist.
2. Copy your certificate image/PDF into that folder, for example `python-course.jpg`.
3. Add an entry in `src/portfolioData.ts`, for example:

```ts
{ title: 'Python Course', issuer: 'Certificate Provider', date: '2026', file: '/certificates/python-course.jpg' }
```

Only add verified awards/certificates. Save the file; Vite refreshes the website.

## Build check

```powershell
npm.cmd run build
```
