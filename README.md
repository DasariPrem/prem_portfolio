# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

## Contact form email setup

The contact form sends messages through EmailJS. To enable it:

1. Create an EmailJS account and connect an email service.
2. Create an email template with the **To Email** set to `2200030565cseh@gmail.com`. Use `{{from_name}}` for the sender's name, `{{from_email}}` for their email, and `{{message}}` for their message. Set **Reply-To** to `{{reply_to}}`.
3. Copy `.env.example` to `.env.local` and fill in the service ID, template ID, and public key from your EmailJS account.
4. Restart the Vite development server after editing `.env.local`.

The EmailJS public key is intended for browser use. Configure allowed origins and abuse protections in EmailJS before deploying.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Oxc](https://oxc.rs)
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/)

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.
