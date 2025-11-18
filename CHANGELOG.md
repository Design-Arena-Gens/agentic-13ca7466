# Changelog

All notable changes to this project will be documented in this file.

## [0.1.0] - 2025-11-18

### Added
- Complete login and authentication system
- User registration with email, password, and name
- Secure password hashing using bcryptjs
- JWT-based authentication with httpOnly cookies
- Login functionality with email and password
- Protected dashboard page for authenticated users
- User profile display showing name, email, and registration date
- Logout functionality
- Responsive UI with gradient design
- Form validation (email format, password length)
- Error and success message handling
- Loading states during API calls
- In-memory database for user storage (demo purposes)
- Auto-redirect to dashboard if already logged in
- Auto-redirect to login if not authenticated
- Demo user account (email: demo@example.com, password: demo123)

### Tech Stack
- Next.js 14 with App Router
- React 18
- TypeScript
- JWT for authentication
- bcryptjs for password hashing
- httpOnly cookies for secure token storage
- CSS3 with gradients and animations

### API Endpoints
- POST /api/auth/register - User registration
- POST /api/auth/login - User login
- POST /api/auth/logout - User logout
- GET /api/auth/me - Get current user info

### Security Features
- Password hashing with bcrypt (10 rounds)
- JWT tokens with 7-day expiration
- httpOnly cookies to prevent XSS attacks
- Secure cookies in production
- Password minimum length validation (6 characters)
- Email uniqueness validation
- Token verification on protected routes

### Pages
- / (Home) - Login and registration forms
- /dashboard - Protected user dashboard

### Future Enhancements
- Replace in-memory database with real database (PostgreSQL, MongoDB)
- Add password reset functionality
- Add email verification
- Add OAuth providers (Google, GitHub)
- Add refresh token mechanism
- Add rate limiting
- Add CSRF protection
- Add session management
- Add user profile editing
- Add remember me functionality
