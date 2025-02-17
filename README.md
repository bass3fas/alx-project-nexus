# 🍽️ Paratha and More - Restaurant Ordering App

## 📌 Project Overview

**Paratha and More** is an intuitive restaurant ordering app where customers can:
- Drag and drop meals into their cart.
- Provide their delivery location via **Google Maps API**.
- Pay via a **payment link** or upload an **invoice** as an alternative.
- Track their order progress in real-time.

**Admin features include:**
- Viewing all incoming orders.
- Managing order statuses.
- Receiving **email notifications** for new orders.

---

## 🚀 Tech Stack

**Frontend Framework:** Next.js 14 (App Router)  
**UI Library:** Tailwind CSS  
**Drag & Drop:** React DnD  
**Location Services:** Google Maps API  
**Payments:** Stripe (or alternative manual invoice upload)  
**File Uploads:** Cloudinary  
**Email Notifications:** Nodemailer  
**State Management:** Zustand / Redux Toolkit  
**Backend (if needed):** Node.js with Express.js  
**Database:** MongoDB with Mongoose (if backend required)  
**Authentication:** NextAuth.js (Google & Email sign-in)  
**Deployment:** Vercel (Frontend) & Railway/Render (Backend)  

---

## 📖 Features Breakdown

### ✅ Client Features
1. **Browse Menu:** View food items with prices, images, and descriptions.
2. **Drag & Drop:** Easily add or remove items from the cart.
3. **Location Sharing:** Get the customer’s location using **Google Maps API**.
4. **Checkout Process:**
   - Option 1: Pay via **Stripe**.
   - Option 2: Upload an **invoice** instead.
5. **Order Tracking:** View the status of past & ongoing orders.
6. **Authentication:** Login via **NextAuth.js** (Google/email).

### ✅ Admin Features
1. **View Orders:** Dashboard listing all customer orders.
2. **Update Order Status:** Mark orders as **Pending, Preparing, Out for Delivery, Delivered**.
3. **Email Alerts:** Receive new order notifications via **Nodemailer**.

---

## 🏗️ Project Setup & Steps

### 1️⃣ Initialize Next.js Project
```bash
npx create-next-app@latest paratha-and-more
cd paratha-and-more
npm install
```

### 2️⃣ Install Required Dependencies
```bash
npm install tailwindcss react-dnd react-dnd-html5-backend google-maps-react 
npm install next-auth stripe cloudinary multer nodemailer zustand
```

### 3️⃣ Setup Tailwind CSS
```bash
npx tailwindcss init -p
```
Update `tailwind.config.js`:
```js
/** @type {import('tailwindcss').Config} */
module.exports = {
  content: ["./pages/**/*.{js,ts,jsx,tsx}", "./components/**/*.{js,ts,jsx,tsx}"],
  theme: { extend: {} },
  plugins: [],
};
```
Import Tailwind into `globals.css`:
```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

### 4️⃣ Setup Drag & Drop for Orders
- Use **React DnD** to implement a drag-and-drop cart.

### 5️⃣ Integrate Google Maps API for Location
- Get an **API Key** from Google Cloud.
- Use **Google Maps API** to retrieve user location.

### 6️⃣ Setup Payment Gateway (Stripe)
- Configure **Stripe** payment processing for checkout.

### 7️⃣ Alternative: Invoice Upload (Cloudinary)
- Customers upload an invoice instead of using Stripe.
- Use **Cloudinary** to store invoice images.

### 8️⃣ Email Notifications with Nodemailer
- Send new order notifications to the admin.

### 9️⃣ Order Status Management
- Admin can update the **status** of orders.

### 🔟 Authentication with NextAuth.js
- Google & Email sign-in for customers and admins.

### 1️⃣1️⃣ Deployment
- **Frontend:** Deploy to **Vercel**.
- **Backend (if needed):** Deploy to **Railway/Render**.

---

## 🎯 Milestones & Timeline

| Milestone | Task | Deadline |
|-----------|------|----------|
| 1 | Project Setup & UI Design (Figma) | Feb 25-26 |
| 2 | Drag & Drop, Cart Functionality | Feb 27-28 |
| 3 | Google Maps Integration | Feb 29 |
| 4 | Payment & Invoice Upload | Mar 1-2 |
| 5 | Email Notifications & Admin Panel | Mar 3-4 |
| 6 | Final Testing & Deployment | Mar 5-6 |

---

## 🎓 Evaluation Criteria (80%+ Score)

✅ **Functionality & Features:** All features implemented smoothly.  
✅ **Code Quality:** Clean, modular, and follows best practices.  
✅ **UI/UX & Responsiveness:** Well-designed and mobile-friendly.  
✅ **Performance Optimization:** Lazy loading, caching, minification.  
✅ **Presentation & Documentation:** Clear README, presentation slides, and video demo.  

---

## 📂 Project Submission Checklist
- ✅ **GitHub Repository** with source code.
- ✅ **README.md** with clear setup instructions.
- ✅ **Presentation Slides** explaining features & tech stack.
- ✅ **Video Demo** showcasing the project in action.

---

## 📬 Contact & Collaboration
- **Discord Channel:** `#ProDevProjectNexus`
- **Mentors:** Cole, Faith, Amanuel (`@Cohort PD-FE-Pilot Mentor`)

🚀 **Let's build something amazing!** 💻✨

