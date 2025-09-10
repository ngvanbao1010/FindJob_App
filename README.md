# FindJob App

A comprehensive job search platform built with Django REST Framework and React Native, designed for connecting job seekers with employers.

## Technologies Used

### Backend (Django REST API)
- **Django 4.2.11** - Web framework
- **Django REST Framework** - API development
- **OAuth2 Toolkit** - Authentication & authorization
- **Cloudinary** - Image storage and management
- **MySQL** - Database
- **drf-yasg** - API documentation (Swagger)
- **Google OAuth2** - Social authentication

### Frontend (React Native/Expo)
- **React Native 0.79.2** - Mobile app framework
- **Expo** - Development platform
- **React Navigation** - Navigation system
- **React Native Paper** - UI components
- **Axios** - HTTP client
- **AsyncStorage** - Local data storage

## Features

### For Job Seekers (Candidates)
- User registration and authentication
- Browse and search job listings
- Filter jobs by category, location, and salary
- Apply for jobs with CV upload
- Track application status
- Follow favorite employers
- Review and rate employers

### For Employers
- Company registration with verification system
- Post and manage job listings
- Review applications and manage candidates
- Approve/reject job applications
- Employer verification process
- Company profile with location mapping

### For Administrators
- User management and verification
- Application statistics and analytics
- Content moderation
- System monitoring

### Additional Features
- Real-time chat messaging
- Push notifications
- Email notifications
- Work schedule management
- Rating and review system
- Google Maps integration
- Multi-role authentication (Admin, Employer, Candidate)

## Project Structure

```
findJobApp/
├── apiJob/                 # Django project settings
├── findJobApp/            # Main Django app
│   ├── models.py         # Database models
│   ├── views.py          # API views
│   ├── serializers.py    # Data serializers
│   ├── urls.py           # URL routing
│   └── migrations/       # Database migrations
├── findjobappmobile/     # React Native mobile app
│   ├── components/       # UI components
│   ├── configs/          # App configuration
│   ├── reducers/         # State management
│   └── styles/           # Styling
├── requirements.txt      # Python dependencies
└── manage.py            # Django management script
```

## Installation & Setup

### Backend Setup

1. **Clone the repository**
   ```bash
   git clone https://github.com/ngvanbao1010/FindJob_App.git
   cd findJobApp
   ```

2. **Create virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Configure database**
   - Update database settings in `apiJob/settings.py`
   - Run migrations:
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

5. **Create superuser**
   ```bash
   python manage.py createsuperuser
   ```

6. **Run development server**
   ```bash
   python manage.py runserver
   ```

### Mobile App Setup

1. **Navigate to mobile directory**
   ```bash
   cd findjobappmobile
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start Expo development server**
   ```bash
   npm start
   ```

4. **Run on device/emulator**
   ```bash
   npm run android  # For Android
   ```
