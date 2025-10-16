# Smart Login System

A modern, fully responsive authentication system built with HTML5, CSS3, and JavaScript. Features a beautiful glass-morphism design with smooth animations, complete OTP verification, and JWT token management. The system includes three main pages: Login, Signup, and Profile with advanced UI/UX enhancements.

## ✨ Features

### 🔐 Authentication System
- **Login Page**: Email/password authentication with forgot password functionality
- **Signup Page**: User registration with email verification via OTP
- **Profile Page**: Enhanced user dashboard with account information and settings
- **Forgot Password**: Complete OTP-based password reset flow
- **Update Profile**: In-app profile editing with real-time updates

### 🛡️ Security Features
- JWT token-based authentication (access_token & refresh_token)
- OTP verification for email confirmation and password reset
- Password strength validation
- Secure token storage in localStorage
- Input validation and sanitization
- Protected routes with automatic redirects

### 🎨 Modern UI/UX Design
- **Glass-morphism Design**: Translucent cards with backdrop blur effects
- **Smooth Animations**: Staggered loading, hover effects, and transitions
- **Interactive Elements**: Ripple effects, pulse animations, and micro-interactions
- **Gradient Backgrounds**: Beautiful color schemes and visual hierarchy
- **Responsive Layout**: Mobile-first design with touch-friendly interfaces

### 📱 Responsive Design
- Mobile-first responsive design
- Bootstrap 5 framework with custom enhancements
- Cross-browser compatibility
- Touch-optimized interactions
- Adaptive typography and spacing

### 🔧 Technical Features
- AJAX API calls with comprehensive error handling
- Form validation (client-side and server-side)
- Loading states and user feedback
- Auto-redirect based on authentication status
- Global error handling with user-friendly messages
- Intersection Observer for performance optimization

## Project Structure

```
ThreeDos Task/
├── pages/
│   ├── index.html          # Login page
│   ├── signup.html         # Signup page
│   └── profile.html        # Profile page
├── css/
│   └── style.css           # Custom styles
├── js/
│   └── main.js             # Main JavaScript functionality
└── README.md               # Project documentation
```

## API Endpoints

The system integrates with the following API endpoints:

### Authentication
- `POST /auth/login` - User login (returns access_token & refresh_token)
- `POST /auth/signup/` - User registration
- `POST /auth/confirm-email/` - Verify OTP for signup
- `POST /auth/resend-otp/` - Resend OTP for signup

### Password Management
- `PATCH /auth/forgot-password` - Send OTP for password reset
- `PATCH /auth/verify-forget-code` - Verify OTP for password reset
- `PATCH /auth/reset-password` - Reset password with OTP

### User Management
- `GET /users` - Get user profile information
- `PATCH /users/` - Update user profile (name)
- `POST /users/logout` - User logout

## Getting Started

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- Web server (for local development) or live server

### Installation

1. **Clone or download the project files**
2. **Open the project in a web server environment**
   - For local development, you can use Live Server extension in VS Code
   - Or use Python's built-in server: `python -m http.server 8000`
   - Or use Node.js serve: `npx serve .`

3. **Access the application**
   - Open your browser and navigate to `http://localhost:8000/pages/`
   - The login page will be the default entry point

### Usage

#### Login Flow
1. Navigate to the login page (`pages/index.html`)
2. Enter your email and password
3. Click "Sign In" to authenticate
4. Upon successful login, you'll be redirected to the profile page
5. Tokens are automatically stored in localStorage

#### Signup Flow
1. Click "Sign up" link on the login page
2. Fill in the registration form with:
   - Full Name
   - Email Address
   - Password (minimum 8 characters)
   - Confirm Password
   - Phone Number
   - Gender
3. Accept terms and conditions
4. Click "Create Account"
5. Verify your email with the OTP sent to your inbox
6. Upon verification, you'll be automatically logged in

#### Forgot Password Flow
1. On the login page, click "Forgot your password?"
2. Enter your email address and click "Send OTP"
3. Check your email for the OTP code
4. Enter the 6-digit OTP code and click "Verify OTP"
5. Upon verification, set your new password
6. Click "Reset Password" to complete the process

#### Profile Management
1. View your enhanced account information with beautiful animations
2. Update your profile name using the "Update Profile" button
3. View security information and account statistics
4. Logout when finished

## Technologies Used

- **HTML5**: Semantic markup and form elements
- **CSS3**: Advanced styling with CSS custom properties, glass-morphism effects, and smooth animations
- **JavaScript (ES6+)**: Modern JavaScript with async/await, Intersection Observer API
- **Bootstrap 5**: Responsive framework with custom enhancements
- **Font Awesome**: Comprehensive icon library for visual elements
- **jQuery**: DOM manipulation, AJAX calls, and event handling
- **CSS Animations**: Keyframe animations, transitions, and micro-interactions

## Browser Support

- Chrome 60+
- Firefox 55+
- Safari 12+
- Edge 79+

## API Configuration

The system is configured to work with the provided API endpoint:
```
https://thetically-impressible-arla.ngrok-free.dev
```

The API integration includes:
- Automatic JWT token handling
- Request/response error handling
- Loading states for better UX
- Proper HTTP status code handling

## Security Considerations

- JWT tokens are stored securely in localStorage
- All API requests include proper authentication headers
- Input validation prevents malicious data submission
- CORS headers are handled appropriately
- ngrok-skip-browser-warning header is included for development

## Customization

### Styling
- Modify CSS variables in `style.css` for color scheme changes
- Update Bootstrap classes for layout modifications
- Add custom animations in the CSS file

### Functionality
- Extend the JavaScript modules for additional features
- Add new API endpoints in the `utils.apiRequest` function
- Implement additional validation rules as needed

## Error Handling

The system includes comprehensive error handling:
- Network connectivity issues
- API response errors
- Form validation errors
- Authentication failures
- User-friendly error messages

## Performance Features

- **Optimized Animations**: Hardware-accelerated CSS transforms and transitions
- **Efficient DOM Manipulation**: jQuery-based with minimal reflows
- **Lazy Loading**: Intersection Observer for performance optimization
- **Responsive Design**: Mobile-first approach with touch optimization
- **Smooth Transitions**: Cubic-bezier easing functions for natural motion
- **Memory Management**: Proper cleanup of event listeners and animations

## UI/UX Enhancements

### Visual Design
- **Glass-morphism Effects**: Translucent cards with backdrop blur
- **Gradient Backgrounds**: Beautiful color schemes and visual hierarchy
- **Interactive Animations**: Hover effects, ripple animations, and micro-interactions
- **Responsive Typography**: Adaptive font sizes and spacing
- **Modern Icons**: Font Awesome integration with contextual icons

### User Experience
- **Loading States**: Visual feedback during API calls
- **Error Handling**: User-friendly error messages and recovery
- **Form Validation**: Real-time validation with visual feedback
- **Accessibility**: Enhanced focus states and keyboard navigation
- **Mobile Optimization**: Touch-friendly interfaces and gestures

## Future Enhancements

Potential improvements for the system:
- **Two-factor authentication (2FA)**: Additional security layer
- **Social media login integration**: OAuth providers
- **Password strength meter**: Real-time password validation
- **Account lockout**: Security after failed attempts
- **Email templates**: Customizable notification emails
- **Multi-language support**: Internationalization
- **Progressive Web App**: Offline functionality and app-like experience

## Support

For technical support or questions about the implementation, please refer to the code comments and this documentation.

## License

This project is created for educational and demonstration purposes.

