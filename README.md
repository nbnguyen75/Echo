<div align="center">

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- Tech badges -->
[![Next.js][Next.js]][Next-url]
[![React][React.js]][React-url]
[![TypeScript][TypeScript]][TypeScript-url]
[![Tailwind][TailwindCSS]][Tailwind-url]
[![Convex][Convex]][Convex-url]
[![Turborepo][Turborepo]][Turborepo-url]
[![Clerk][Clerk]][Clerk-url]
[![AWS][AWS]][AWS-url]
[![Vapi][Vapi]][Vapi-url]
[![Sentry][Sentry]][Sentry-url]
[![Bun][Bun]][Bun-url]

</div>

<br />
<div align="center">
  <a href="https://github.com/nbnguyen75/echo">
    <img src="images/logo.png" alt="Logo" width="80" height="80">
  </a>

  <h3 align="center">Echo</h3>

  <p align="center">
    A full-stack, production-ready AI customer support platform with real-time chat, voice, RAG-powered knowledge base, and human handoff.
    <br />
    <a href="https://github.com/nbnguyen75/echo"><strong>Explore the docs »</strong></a>
    <br />
    <br />
    <a href="https://github.com/nbnguyen75/echo">View Demo</a>
    ·
    <a href="https://github.com/nbnguyen75/echo/issues/new?labels=bug&template=bug-report---.md">Report Bug</a>
    ·
    <a href="https://github.com/nbnguyen75/echo/issues/new?labels=enhancement&template=feature-request---.md">Request Feature</a>
  </p>
</div>

<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#key-features">Key Features</a></li>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#roadmap">Roadmap</a></li>
    <li><a href="#contributing">Contributing</a></li>
    <li><a href="#license">License</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

## About The Project

[![Product Name Screen Shot][product-screenshot]](https://example.com)

**Echo** is an AI-powered, multi-tenant customer support platform built from the ground up as a full-stack, production-grade B2B SaaS template — not just a demo.

It ships with real-time AI chat powered by Convex Agents, voice support via VAPI, a RAG-based knowledge base for smart document search, and full workspace/team/billing management using Clerk. Every feature was built chapter-by-chapter with real pull requests and CodeRabbit code reviews, making it a great reference for building production SaaS apps.

Inspired by and built along with [Code With Antonio](https://www.youtube.com/@codewithantonio)'s tutorial series.

### Key Features

- 🤖 **Real-time AI Chat** — powered by Convex Agents
- 📣 **Human Handoff & Auto-Close** — using AI Tools
- 🧠 **Smart Knowledge Base** — Embeddings + RAG
- 🔊 **Voice Support** — by VAPI
- 🔑 **API Key Storage** — AWS Secrets Manager
- 👥 **Team Management** — by Clerk
- 🔐 **Authentication** — by Clerk
- 💳 **Subscription Billing** — by Clerk
- 🛠️ **Embeddable Widget** — drop-in support chat for any site
- 📈 **Operator Dashboard** — for managing conversations
- 🧰 **Developer Toolkit** — for embed script integration
- 🧠 **Multi-Model AI Support** — OpenAI, Anthropic, Grok
- 🪵 **Error Tracking** — by Sentry
- 🧑‍💻 **Automated PR Reviews** — by CodeRabbit

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Built With

* [![Next.js][Next.js]][Next-url]
* [![React][React.js]][React-url]
* [![TypeScript][TypeScript]][TypeScript-url]
* [![Tailwind CSS][TailwindCSS]][Tailwind-url]
* [![shadcn/ui][shadcn]][shadcn-url]
* [![Convex][Convex]][Convex-url]
* [![Turborepo][Turborepo]][Turborepo-url]
* [![Clerk][Clerk]][Clerk-url]
* [![AWS][AWS]][AWS-url]
* [![Vapi][Vapi]][Vapi-url]
* [![Sentry][Sentry]][Sentry-url]
* [![Bun][Bun]][Bun-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Getting Started

Follow these steps to get a local copy of Echo up and running.

### Prerequisites

* Node.js (LTS recommended)
  ```sh
  node -v
  ```
* Package manager — this monorepo works with either **Bun** (recommended, faster installs) or **pnpm**:
  ```sh
  # Bun
  curl -fsSL https://bun.sh/install | bash
  bun -v

  # or pnpm
  npm install -g pnpm
  ```
* Accounts/API keys for:
  * [Convex](https://convex.dev)
  * [Clerk](https://clerk.com)
  * [VAPI](https://vapi.ai)
  * [AWS Secrets Manager](https://aws.amazon.com)
  * [Sentry](https://sentry.io)
  * OpenAI / Anthropic / Grok API keys

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/nbnguyen75/echo.git
   cd echo
   ```
2. Install dependencies

   Using Bun:
   ```sh
   bun install
   ```
   Using pnpm:
   ```sh
   pnpm install
   ```
3. Set up environment variables — copy `.env.example` to `.env.local` in each app and fill in:
   ```
   NEXT_PUBLIC_CONVEX_URL=
   CLERK_SECRET_KEY=
   NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
   VAPI_API_KEY=
   AWS_ACCESS_KEY_ID=
   AWS_SECRET_ACCESS_KEY=
   OPENAI_API_KEY=
   ANTHROPIC_API_KEY=
   SENTRY_DSN=
   ```
4. Push your Convex schema

   Using Bun:
   ```sh
   bun convex dev
   ```
   Using pnpm:
   ```sh
   pnpm convex dev
   ```
5. Run the dev server

   Using Bun:
   ```sh
   bun dev
   ```
   Using pnpm:
   ```sh
   pnpm dev
   ```
6. Change the git remote to avoid accidental pushes to the base project
   ```sh
   git remote set-url origin nbnguyen75/echo
   git remote -v # confirm the changes
   ```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Usage

- Embed the support widget on any website using the generated embed script.
- Manage conversations, knowledge base docs, and escalations from the **Operator Dashboard**.
- Configure your preferred AI model (OpenAI, Anthropic, or Grok) per workspace.
- Enable voice conversations via VAPI for a richer support experience.

_For more examples and API reference, please refer to the [Documentation](https://example.com)._

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Roadmap

- [ ] Multi-language support for chat & KB
- [ ] Analytics dashboard for conversation insights
- [ ] Slack / Teams integration for handoff notifications
- [ ] Mobile-optimized widget
- [ ] Additional AI model providers

See the [open issues](https://github.com/nbnguyen75/echo/issues) for a full list of proposed features (and known issues).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Contributing

Contributions make the open-source community amazing. Any contributions are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## License

Distributed under the MIT License. See `LICENSE.txt` for more information.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Contact

Your Name - [@twitter_handle](https://twitter.com/twitter_handle) - email@example.com

Project Link: [https://github.com/nbnguyen75/echo](https://github.com/nbnguyen75/echo)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

## Acknowledgments

* [Code With Antonio](https://www.youtube.com/@codewithantonio) — original tutorial series this project is based on
* [Best-README-Template](https://github.com/othneildrew/Best-README-Template)
* [Convex](https://convex.dev)
* [Clerk](https://clerk.com)
* [VAPI](https://vapi.ai)
* [shadcn/ui](https://ui.shadcn.com)

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/github/contributors/nbnguyen75/echo.svg?style=for-the-badge
[contributors-url]: https://github.com/nbnguyen75/echo/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/nbnguyen75/echo.svg?style=for-the-badge
[forks-url]: https://github.com/nbnguyen75/echo/network/members
[stars-shield]: https://img.shields.io/github/stars/nbnguyen75/echo.svg?style=for-the-badge
[stars-url]: https://github.com/nbnguyen75/echo/stargazers
[issues-shield]: https://img.shields.io/github/issues/nbnguyen75/echo.svg?style=for-the-badge
[issues-url]: https://github.com/nbnguyen75/echo/issues
[license-shield]: https://img.shields.io/github/license/nbnguyen75/echo.svg?style=for-the-badge
[license-url]: https://github.com/nbnguyen75/echo/blob/main/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/linkedin_username
[product-screenshot]: images/screenshot.png

[Next.js]: https://img.shields.io/badge/Next.js_16-000000?style=for-the-badge&logo=nextdotjs&logoColor=white
[Next-url]: https://nextjs.org/
[React.js]: https://img.shields.io/badge/React_19-20232A?style=for-the-badge&logo=react&logoColor=61DAFB
[React-url]: https://reactjs.org/
[TypeScript]: https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white
[TypeScript-url]: https://www.typescriptlang.org/
[TailwindCSS]: https://img.shields.io/badge/Tailwind_v4-38B2AC?style=for-the-badge&logo=tailwind-css&logoColor=white
[Tailwind-url]: https://tailwindcss.com/
[shadcn]: https://img.shields.io/badge/shadcn%2Fui-000000?style=for-the-badge&logo=shadcnui&logoColor=white
[shadcn-url]: https://ui.shadcn.com/
[Convex]: https://img.shields.io/badge/Convex-EE342F?style=for-the-badge&logo=convex&logoColor=white
[Convex-url]: https://convex.dev/
[Turborepo]: https://img.shields.io/badge/Turborepo-EF4444?style=for-the-badge&logo=turborepo&logoColor=white
[Turborepo-url]: https://turbo.build/repo
[Clerk]: https://img.shields.io/badge/Clerk-6C47FF?style=for-the-badge&logo=clerk&logoColor=white
[Clerk-url]: https://clerk.com/
[AWS]: https://img.shields.io/badge/AWS_Secrets_Manager-232F3E?style=for-the-badge&logo=amazonaws&logoColor=white
[AWS-url]: https://aws.amazon.com/secrets-manager/
[Vapi]: https://img.shields.io/badge/Vapi-000000?style=for-the-badge&logo=voip&logoColor=white
[Vapi-url]: https://vapi.ai/
[Sentry]: https://img.shields.io/badge/Sentry-362D59?style=for-the-badge&logo=sentry&logoColor=white
[Sentry-url]: https://sentry.io/
[Bun]: https://img.shields.io/badge/Bun-000000?style=for-the-badge&logo=bun&logoColor=white
[Bun-url]: https://bun.sh/
