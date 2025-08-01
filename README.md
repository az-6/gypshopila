# Gypshophila Boardy - Next.js Website

Fully functional website untuk layanan sewa Standing Acrylic Flower & Banner dengan sistem review yang terintegrasi.

## ✨ Fitur Utama

### 🌐 Website Utama

- **Responsive Design** - Optimal di semua device
- **Interactive Gallery** - Showcase produk dengan dialog view
- **Pricing & Services** - Informasi lengkap paket layanan
- **Customer Reviews** - Sistem review real-time dari pelanggan
- **Contact Integration** - Direct link ke WhatsApp & Instagram
- **SOP Section** - Informasi lengkap prosedur penyewaan

### 📊 Sistem Review

- **Review Form** - Customer dapat submit review dengan star rating
- **Admin Moderation** - Review harus disetujui admin sebelum tampil
- **Real-time Stats** - Statistik otomatis berdasarkan review yang disetujui
- **Data Persistence** - Review tersimpan dalam database

### 🔐 Admin Panel

- **Password Protection** - Akses admin dengan autentikasi
- **Review Management** - Approve/reject review dari customer
- **Dashboard Stats** - Overview statistik review
- **Responsive Admin UI** - Interface admin yang user-friendly

## 🚀 Teknologi

- **Next.js 15** - React framework with App Router
- **TypeScript** - Type safety
- **Tailwind CSS** - Utility-first CSS framework
- **Radix UI** - Headless UI components
- **API Routes** - Built-in API with Next.js
- **Middleware** - Authentication & route protection

## 📁 Struktur Project

```
├── app/
│   ├── api/                    # API Routes
│   │   ├── reviews/           # Review CRUD operations
│   │   └── admin/             # Admin APIs
│   ├── admin/                 # Admin panel
│   ├── admin-login/          # Admin login page
│   ├── page.tsx              # Main landing page
│   └── layout.tsx            # Root layout
├── components/ui/             # Reusable UI components
├── lib/
│   ├── db.ts                 # Database operations & types
│   └── utils.ts              # Utility functions
├── middleware.ts             # Authentication middleware
└── public/                   # Static assets
```

## 🛠️ Setup Development

1. **Clone repository**

   ```bash
   git clone <your-repo-url>
   cd gypshophila-boardy
   ```

2. **Install dependencies**

   ```bash
   npm install
   # atau
   pnpm install
   ```

3. **Setup environment variables**

   ```bash
   cp .env.example .env.local
   ```

   Edit `.env.local`:

   ```env
   ADMIN_PASSWORD=your_secure_password_here
   ```

4. **Run development server**

   ```bash
   npm run dev
   # atau
   pnpm dev
   ```

5. **Akses aplikasi**
   - Website utama: http://localhost:3000
   - Admin login: http://localhost:3000/admin-login
   - Admin panel: http://localhost:3000/admin

## 🌐 Deploy ke Vercel

### Manual Deploy

1. **Push ke GitHub**

   ```bash
   git add .
   git commit -m "Full functional website with admin panel"
   git push origin main
   ```

2. **Connect ke Vercel**

   - Login ke [vercel.com](https://vercel.com)
   - Click "New Project"
   - Import dari GitHub repository
   - Set Framework Preset: "Next.js"

3. **Configure Environment Variables**
   Di Vercel dashboard, tambahkan:

   ```
   ADMIN_PASSWORD=your_secure_password_here
   ```

4. **Deploy**
   - Click "Deploy"
   - Website akan live di: `https://your-project-name.vercel.app`

## 🔧 Admin Panel

### Login Credentials

- **URL**: `/admin-login`
- **Default Password**: `gypshophila2024`
- **Features**: Review management, statistics, approval system

### Admin Functions

- ✅ Approve customer reviews
- ❌ Reject inappropriate reviews
- 📊 View statistics dashboard
- 🔄 Real-time data updates

## 📱 Customer Features

- 🌟 Submit reviews with star ratings
- 📝 Fill detailed review forms
- ✅ Consent for public display
- 📊 View approved reviews
- 📞 Direct WhatsApp & Instagram links

## 🔒 Security

- Password-protected admin access
- Input validation & sanitization
- CSRF protection with secure cookies
- Rate limiting ready

## 📞 Support

- **WhatsApp**: +62 821-8330-1667
- **Instagram**: @gypshophila.boardy
- **Location**: Semarang, Indonesia

---

**🎉 Website fully functional and ready for production deployment!**
