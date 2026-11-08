<h1 align="center">🔐 Next.js Auth Template</h1>

<p align="center">
A production-ready authentication starter built with <b>Next.js</b>, <b>Auth.js</b>, <b>Prisma</b>, <b>PostgreSQL</b>, and <b>Feature-Sliced Design (FSD)</b>.
</p>

<p align="center">
<a href="https://next-template-rho-six.vercel.app/en"><b>🚀 Live Demo</b></a>
</p>

---

> [!NOTE]
> This is a ready-to-use base for apps that need more than a simple login form. OAuth, email verification, password reset, 2FA, profile settings, admin panel, rate limiting, and security protection are already done.

> [!IMPORTANT]
> The project uses **Feature-Sliced Design (FSD)**. Layer boundaries are checked automatically with **ESLint**, so the code stays clean as the project grows.

---

## ✨ Features

<table>
  <thead>
    <tr>
      <th width="260" align="left">Feature</th>
      <th align="left">Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td width="260"><b>Language Switching</b></td>
      <td>English and Russian.</td>
    </tr>
    <tr>
      <td width="260"><b>Credentials Auth</b></td>
      <td>Sign up and log in with email and password.</td>
    </tr>
    <tr>
      <td width="260"><b>OAuth Auth</b></td>
      <td>Log in with Google or GitHub.</td>
    </tr>
    <tr>
      <td width="260"><b>Email Verification</b></td>
      <td>Safe one-time tokens with automatic login.</td>
    </tr>
    <tr>
      <td width="260"><b>Password Recovery</b></td>
      <td>Password reset links that expire after some time.</td>
    </tr>
    <tr>
      <td width="260"><b>Two-Factor Auth</b></td>
      <td>TOTP (RFC 6238) with QR code setup and backup codes.</td>
    </tr>
    <tr>
      <td width="260"><b>Profile Management</b></td>
      <td>Change username, display name, avatar, email, and password.</td>
    </tr>
    <tr>
      <td width="260"><b>Cloudinary Uploads</b></td>
      <td>Signed avatar uploads from the client.</td>
    </tr>
    <tr>
      <td width="260"><b>Admin Panel</b></td>
      <td>User management, pagination, search, roles, and audit log.</td>
    </tr>
    <tr>
      <td width="260"><b>Rate Limiting</b></td>
      <td>Based on PostgreSQL. No extra services needed.</td>
    </tr>
    <tr>
      <td width="260"><b>Account Linking</b></td>
      <td>Safe OAuth linking with protection from account takeover.</td>
    </tr>
    <tr>
      <td width="260"><b>Session Validation</b></td>
      <td>User status is checked against the database again.</td>
    </tr>
    <tr>
      <td width="260"><b>Themes</b></td>
      <td>Dark, light, and system theme. The choice is saved.</td>
    </tr>
    <tr>
      <td width="260"><b>Responsive UI</b></td>
      <td>Modern interface built with shadcn/ui and Tailwind CSS.</td>
    </tr>
    <tr>
      <td width="260"><b>FSD Architecture</b></td>
      <td>Layer rules are enforced with ESLint.</td>
    </tr>
  </tbody>
</table>

---

## 🖥️ Screenshots

<details>
<summary><b>Click to open</b></summary>

<br>

<table>
  <tr>
    <td align="center" width="50%">
      <b>Profile</b><br><br>
      <img src="https://github.com/nfluvv/next-template/blob/main/public/screenshots/profile.PNG?raw=true" alt="Profile" />
    </td>
    <td align="center" width="50%">
      <b>Register</b><br><br>
      <img src="https://github.com/nfluvv/next-template/blob/main/public/screenshots/register.PNG?raw=true" alt="Register" />
    </td>
  </tr>
  <tr>
    <td align="center" width="50%">
      <b>Settings</b><br><br>
      <img src="https://github.com/nfluvv/next-template/blob/main/public/screenshots/settings2.PNG?raw=true" alt="Settings" />
    </td>
    <td align="center" width="50%">
      <b>Settings — Security</b><br><br>
      <img src="https://github.com/nfluvv/next-template/blob/main/public/screenshots/settings.PNG?raw=true" alt="Settings Security" />
    </td>
  </tr>
</table>

</details>

---

## 🛠 Tech Stack

<table>
  <thead>
    <tr>
      <th width="220" align="left">Area</th>
      <th align="left">Tools</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td width="220"><b>Framework</b></td>
      <td>Next.js 16</td>
    </tr>
    <tr>
      <td width="220"><b>UI</b></td>
      <td>React 19</td>
    </tr>
    <tr>
      <td width="220"><b>Authentication</b></td>
      <td>Auth.js / NextAuth.js v5</td>
    </tr>
    <tr>
      <td width="220"><b>Database & ORM</b></td>
      <td>PostgreSQL, Prisma</td>
    </tr>
    <tr>
      <td width="220"><b>State</b></td>
      <td>Zustand (client), TanStack Query (server)</td>
    </tr>
    <tr>
      <td width="220"><b>Forms</b></td>
      <td>React Hook Form + Zod</td>
    </tr>
    <tr>
      <td width="220"><b>UI Components</b></td>
      <td>shadcn/ui + Radix UI</td>
    </tr>
    <tr>
      <td width="220"><b>Styling</b></td>
      <td>Tailwind CSS 4</td>
    </tr>
    <tr>
      <td width="220"><b>Services</b></td>
      <td>Cloudinary (images), Resend (email)</td>
    </tr>
    <tr>
      <td width="220"><b>2FA</b></td>
      <td>OTPAuth / TOTP</td>
    </tr>
    <tr>
      <td width="220"><b>Testing & CI</b></td>
      <td>Vitest, GitHub Actions</td>
    </tr>
    <tr>
      <td width="220"><b>Architecture</b></td>
      <td>Feature-Sliced Design</td>
    </tr>
  </tbody>
</table>

---

## 🚀 Installation

<details>
<summary><b>Step-by-step guide</b></summary>

<br>

**1. Clone the repository**

```bash
git clone https://github.com/nfluvv/next-template.git
cd next-template
```

**2. Install dependencies**

```bash
npm install
```

**3. Set up environment variables**

```bash
cp .env.example .env
```

Fill in the values in `.env`: PostgreSQL connection, Auth.js secret, OAuth keys, Cloudinary, and Resend.

**4. Set up the database**

Make sure PostgreSQL is running and `DATABASE_URL` is set in `.env`.

```bash
npx prisma generate
npx prisma migrate dev
```

**5. Start the dev server**

```bash
npm run dev
```

Open the app at `http://localhost:3000`.

</details>

<details>
<summary><b>Useful Prisma commands</b></summary>

<br>

```bash
# Generate Prisma Client
npx prisma generate

# Create and apply a new migration
npx prisma migrate dev

# Apply migrations in production
npx prisma migrate deploy

# Open Prisma Studio (database viewer)
npx prisma studio

# Reset the database
npx prisma migrate reset
```

> [!WARNING]
> `prisma migrate reset` deletes all data in the database. Use it only in development.

</details>

---

## 🏗️ Architecture

> [!TIP]
> Each layer can only import from the layers below it. This keeps the code simple to read and easy to scale.

<details>
<summary><b>Project structure</b></summary>

<br>

```text
src/
├── app/          # App providers and global config
├── views/        # Page-level compositions
├── widgets/      # Complex reusable UI blocks
├── features/     # User actions and business logic
├── entities/     # Domain models, schemas, and queries
└── shared/       # UI kit, utilities, and infrastructure

app/              # Next.js routing layer
```

</details>
