# 📦 ImageKit_Video_Image

A modern video & image upload and management app built with **Next.js** and integrated with **ImageKit.io**. This project demonstrates secure authentication, efficient media handling, and a full-stack developer workflow. 🚀

---

## ✨ Features

- 🔒 **Authentication:** Secure login system using email and password via NextAuth (JWT strategy).
- 🖼️ **ImageKit Integration:** Upload, authenticate, and manage media files using ImageKit.io.
- 📹 **Video Management:** Create, list, and manage video entries with API endpoints.
- ⚡ **Next.js 14:** Built with App Router, server components, and serverless API routes.
- 🎨 **Modern UI:** Uses TailwindCSS and DaisyUI for customizable and responsive design.
- 📚 **TypeScript:** Fully typed for safety and developer experience.

---

## 🚀 Getting Started

Clone the repo and install dependencies:

```bash
git clone https://github.com/suthar879/ImageKit_Video_Image.git
cd ImageKit_Video_Image
npm install
```

### 🔧 Environment Setup

Create a `.env.local` file and add the following:

```env
MONGODB_URI=your_mongodb_connection_string
NEXTAUTH_SECRET=your_nextauth_secret
NEXT_PUBLIC_PUBLIC_KEY=your_imagekit_public_key
IMAGEKIT_PRIVATE_KEY=your_imagekit_private_key
NEXT_PUBLIC_URL_ENDPOINT=your_imagekit_url_endpoint
```

### 🏃‍♂️ Run the Development Server

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Visit [http://localhost:3000](http://localhost:3000) to view the app.

---

## 🛠️ Usage

- **Authentication:** Register or login at `/login` or `/register`.
- **Media Upload:** Use the upload button to add images/videos via ImageKit.
- **Video API:**
  - `GET /api/videos` - List all videos.
  - `POST /api/videos` - Add a new video (authentication required).
- **Edit UI:** Modify `app/page.tsx` to customize your landing page.

---

## 🏗️ Project Structure

- `app/` - Next.js app directory (pages, components, API).
- `lib/` - Utility libraries (auth, db, API clients).
- `models/` - Mongoose models for User and Video.
- `middleware.ts` - Auth middleware for route protection.

---

## 🔒 Authentication Flow

- Uses NextAuth with credential provider.
- JWT sessions; user info stored in token/session.
- Protected API routes and pages using custom middleware.

---

## 🖼️ ImageKit Integration

- Uses `imagekitio-next` for uploading and authenticating media.
- Serverless route `/api/imagekit-auth` provides secure authentication parameters.

---

## 🧑‍💻 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you’d like to change.

---

## 📄 License

This project is for educational/demo purposes. Add a license if you plan to use it in production.

---

## 👤 Author

- **GitHub:** [suthar879](https://github.com/suthar879)

---

## 🌍 Deploy

Deploy easily on [Vercel](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme). See [Next.js deployment docs](https://nextjs.org/docs/app/building-your-application/deploying).

---

## 📚 Learn More

- [Next.js Documentation](https://nextjs.org/docs)
- [ImageKit Docs](https://docs.imagekit.io/)
- [Learn Next.js](https://nextjs.org/learn)
