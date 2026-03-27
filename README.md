<div align="center">

# ✨ Rayhona Salon
### Professional Beauty Salon Management System

[![Next.js](https://img.shields.io/badge/Next.js-14.0-black?style=for-the-badge&logo=next.js)](https://nextjs.org/)
[![React](https://img.shields.io/badge/React-18.2-blue?style=for-the-badge&logo=react)](https://reactjs.org/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.3-38bdf8?style=for-the-badge&logo=tailwind-css)](https://tailwindcss.com/)
[![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)](LICENSE)

**A modern, feature-rich web application for beauty salon accounting, worker share calculations, and automated reporting.**

[Documentation](#documentation) • [Report Bug](#issues) • [Request Feature](#issues)

---

</div>

## 🎯 Overview

Rayhona Salon is a comprehensive **Next.js-powered** beauty salon management system designed to streamline financial operations, automate worker share calculations, and provide seamless reporting with Google Sheets integration.

> 💡 **Perfect for:** Salon owners seeking to digitize and automate their accounting workflows.

---

## ✨ Features

### 🔐 **Security & Authentication**
- Secure login system with session management
- Automatic session expiration (24 hours)
- Account lockout after failed attempts
- Local storage encryption

### 💼 **Business Management**
- Automatic worker share calculations
- Multiple pricing tiers (employees vs. apprentices)
- Service-based commission rules
- Real-time financial calculations

### 🌍 **Internationalization**
- Multi-language support (Uzbek Latin, Uzbek Cyrillic, Russian)
- Seamless language switching
- Cultural date/time formatting

### 🎨 **User Experience**
- Beautiful responsive design
- Dark/Light theme support
- Stunning animated UI with starry effects
- Mobile-first approach

### 📊 **Data Management**
- Google Sheets integration
- Automated data synchronization
- Export capabilities
- Historical data tracking

---

## 🚀 Quick Start

### Prerequisites

- **Node.js** 18.0 or higher
- **npm** or **yarn** package manager

### Installation

```bash
# Clone the repository
git clone https://github.com/NodirUstoz/Rayhona-Beauty-Salon.git
cd Rayhona-Beauty-Salon

# Install dependencies
npm install

# Configure environment variables
cp .env.example .env.local
```

### Configuration

Edit `.env.local` with your credentials:

```env
# Authentication
NEXT_PUBLIC_ADMIN_USERNAME=user
NEXT_PUBLIC_ADMIN_PASSWORD=your_secure_password

# Google Sheets (Optional)
NEXT_PUBLIC_GOOGLE_SCRIPT_URL=your_script_url
```

### Development

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) in your browser.

### Production

```bash
npm run build
npm start
```

---

## 📖 Documentation

### Default Credentials

| Username | Password | 
|----------|----------|
| `user` | Set in `.env.local` |

> ⚠️ **Security Note:** Always change default credentials before deployment!

### Worker Share System

The system implements intelligent commission calculations:

- **Salon Owner (Rayhona):** 100% of all services
- **Special Employees (Dilnoza, Mavluda):** 40% on manikur services, 50% on others
- **Regular Employees:** 50% standard commission
- **Apprentices:** Work for free (0% commission)

### Customization

#### Adding Services

Edit `pages/index.js` and update the `getServices()` function:

```javascript
const services = {
  'uz-latin': ['Manikyur', 'Pedikyur', /* ... */],
  'uz-cyrillic': ['Маникюр', 'Педикюр', /* ... */],
  'ru': ['Маникюр', 'Педикюр', /* ... */]
}
```

#### Adding Workers

Update the `getWorkers()` function:

```javascript
const workers = [
  { name: 'Your Name', type: 'xodim' },  // Employee
  { name: 'Apprentice', type: 'shogirt' } // Apprentice
]
```

#### Styling

- **Global Styles:** `styles/globals.css`
- **Tailwind Config:** `tailwind.config.js`
- **Theme Colors:** Modify gradient values in components

---

## 🎨 Screenshots

> *Beautiful starry sky animations with cosmic effects*

> *Intuitive login interface with modern design*

> *Real-time calculation with beautiful result cards*

---

## 🌐 Deployment

### Vercel (Recommended)

1. Fork this repository
2. Import project to [Vercel](https://vercel.com)
3. Add environment variables
4. Deploy! 🚀

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new)

### Other Platforms

- **Netlify:** [Deploy Guide](https://docs.netlify.com/)
- **Railway:** [Railway Docs](https://docs.railway.app/)
- **AWS Amplify:** [AWS Docs](https://docs.aws.amazon.com/)

---

## 🔒 Security

### Security Features

✅ Encrypted local storage  
✅ Session token generation  
✅ Failed login tracking  
✅ Automatic lockout system  
✅ HTTPS/SSL support  

### Before Deployment

1. Change default password
2. Set environment variables
3. Enable HTTPS/SSL
4. Review [SECURITY.md](SECURITY.md)

---

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Nodir Ustoz**

- GitHub: [@NodirUstoz](https://github.com/NodirUstoz)
- Portfolio: Coming Soon

---

## 🙏 Acknowledgments

- Built with [Next.js](https://nextjs.org/)
- UI powered by [Tailwind CSS](https://tailwindcss.com/)
- Icons from [Lucide](https://lucide.dev/)
- Special thanks to the Rayhona Beauty Salon team

---

<div align="center">

**Made with ❤️ and Next.js**

⭐ Star this repo if you find it helpful!

---

[⬆ Back to Top](#-rayhona-salon)

</div>
