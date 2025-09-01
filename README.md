# EDJS Platform - École du Jeune Spectateur

A complete platform for managing theatrical spectacles for schools, associations, and families in Morocco.

## 🏗️ Architecture

This platform consists of two main components:

### 📱 Website (`/website`)
- **Public-facing EDJS website** for spectacle discovery and booking
- **Static HTML/CSS/JS** with Supabase integration
- **Authentication system** with role-based access
- **Real-time spectacle synchronization**
- **Responsive design** optimized for all devices

### 🔧 Admin App (`/admin-app`)
- **React-based admin dashboard** for spectacle management
- **Role-based admin interface** (Super Admin, Spectacle Manager, etc.)
- **Real-time data synchronization** with the website
- **Comprehensive spectacle CRUD operations**
- **User management and invitations**

## 🚀 Features

### Website Features
- **Spectacle Browsing**: Browse available spectacles with filtering
- **Authentication**: Login/register with role selection (School, Association, Individual)
- **Guest Access**: Browse spectacles without registration
- **Reservation System**: Book spectacles for authenticated and guest users
- **Real-time Updates**: Spectacle data updates live from admin changes
- **Responsive Design**: Mobile-first approach

### Admin Features
- **Spectacle Management**: Create, edit, delete, and manage spectacles
- **Data Import**: Import spectacle data from existing EDJS website
- **Real-time Sync**: Changes reflect immediately on the public website
- **User Management**: Invite and manage admin users with different roles
- **Analytics Dashboard**: Track spectacle performance and bookings

## 🛠️ Technology Stack

### Frontend
- **Website**: HTML5, CSS3, JavaScript ES6+
- **Admin App**: React 18, TypeScript, Vite
- **Styling**: Bootstrap 5, Custom CSS
- **Icons**: Font Awesome, Lucide React

### Backend & Database
- **Database**: Supabase (PostgreSQL)
- **Authentication**: Supabase Auth
- **Real-time**: Supabase Realtime
- **Storage**: Supabase Storage (for images/media)

### Deployment
- **Website**: Static hosting (Netlify, Vercel, or similar)
- **Admin App**: Static hosting with SPA routing
- **Database**: Supabase cloud hosting

## 📦 Installation & Setup

### Prerequisites
- Node.js 18+ and npm
- Supabase account and project

### 1. Clone the Repository
```bash
git clone https://github.com/imadexpndy/edjs.site.git
cd edjs.site
```

### 2. Setup Admin App
```bash
cd admin-app
npm install
cp .env.example .env
# Update .env with your Supabase credentials
npm run dev
```

### 3. Setup Website
```bash
cd ../website
# Update assets/js/supabase-config.js with your Supabase credentials
# Serve with any static server (Python, Node, etc.)
python -m http.server 8000
```

### 4. Database Setup
1. Create a new Supabase project
2. Run the SQL migrations in `/admin-app/supabase/migrations/`
3. Set up Row Level Security (RLS) policies
4. Update environment variables in both projects

## 🔧 Configuration

### Supabase Configuration
Update the following files with your Supabase credentials:
- `/admin-app/.env` - Admin app environment variables
- `/website/assets/js/supabase-config.js` - Website Supabase config

### Environment Variables
```env
VITE_SUPABASE_URL=your_supabase_url
VITE_SUPABASE_ANON_KEY=your_supabase_anon_key
```

## 🚀 Deployment

### Website Deployment
1. Build static files (if needed)
2. Deploy to static hosting (Netlify, Vercel, GitHub Pages)
3. Configure custom domain if desired

### Admin App Deployment
1. Build the React app: `npm run build`
2. Deploy the `dist` folder to static hosting
3. Configure SPA routing for client-side routing

## 📝 Usage

### For End Users (Website)
1. Visit the website
2. Browse available spectacles
3. Login or continue as guest
4. Make reservations for spectacles
5. Manage bookings through user dashboard

### For Administrators (Admin App)
1. Access the admin dashboard
2. Login with admin credentials
3. Manage spectacles (create, edit, delete)
4. Import data from existing sources
5. Monitor real-time updates on the website

## 🔐 Authentication & Roles

### Website Roles
- **Individual**: Personal bookings and guest access
- **School**: Educational institution bookings
- **Association**: Organization bookings

### Admin Roles
- **Super Admin**: Full platform access
- **Admin Full**: Complete spectacle and user management
- **Admin Spectacles**: Spectacle management only
- **Admin Schools**: School management
- **Admin Partners**: Partner management

## 🔄 Real-time Synchronization

The platform uses Supabase Realtime to ensure:
- Admin changes reflect immediately on the website
- Spectacle availability updates in real-time
- User actions sync across all sessions

## 📱 Mobile Responsiveness

Both the website and admin app are fully responsive:
- Mobile-first design approach
- Touch-friendly interfaces
- Optimized for tablets and smartphones

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Test thoroughly
5. Submit a pull request

## 📄 License

This project is proprietary software for École du Jeune Spectateur.

## 📞 Support

For support and questions:
- Email: info@edjs.ma
- Phone: +212 5 22 98 10 85
- Website: https://edjs.ma

---

**École du Jeune Spectateur** - Bringing theatrical arts to young audiences across Morocco.
