# Smart Login System

A fully responsive smart login system built with native HTML, CSS, and JavaScript. This system includes three main pages: Login, Signup, and Profile, with complete OTP verification functionality and JWT token management.

## Features

### 🔐 Authentication System
- **Login Page**: Email/password authentication with remember me functionality
- **Signup Page**: User registration with email verification via OTP
- **Profile Page**: User dashboard with account information and settings
- **Forgot Password**: OTP-based password reset functionality

### 🛡️ Security Features
- JWT token-based authentication
- OTP verification for email confirmation
- Password strength validation
- Secure token storage in localStorage
- Input validation and sanitization

### 📱 Responsive Design
- Mobile-first responsive design
- Bootstrap 5 framework
- Modern UI with smooth animations
- Cross-browser compatibility

### 🔧 Technical Features
- AJAX API calls with error handling
- Form validation (client-side and server-side)
- Loading states and user feedback
- Auto-redirect based on authentication status
- Global error handling

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

- `POST /auth/login` - User login
- `POST /auth/signup` - User registration
- `POST /auth/forgot-password` - Send OTP for password reset
- `POST /auth/verify-otp` - Verify OTP for password reset
- `POST /auth/verify-signup-otp` - Verify OTP for signup
- `POST /auth/resend-otp` - Resend OTP
- `POST /auth/change-password` - Change user password
- `GET /auth/profile` - Get user profile information

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
1. Navigate to the login page
2. Enter your email and password
3. Click "Sign In" to authenticate
4. Upon successful login, you'll be redirected to the profile page

#### Signup Flow
1. Click "Sign up" link on the login page
2. Fill in the registration form with:
   - Full Name
   - Email Address
   - Password (minimum 8 characters)
   - Confirm Password
3. Accept terms and conditions
4. Click "Create Account"
5. Verify your email with the OTP sent to your inbox
6. Upon verification, you'll be automatically logged in

#### Forgot Password Flow
1. On the login page, click "Forgot your password?"
2. Enter your email address
3. Check your email for the OTP code
4. Enter the 6-digit OTP code
5. Upon verification, you can reset your password

#### Profile Management
1. View your account information
2. Change your password using the "Change Password" button
3. Logout when finished

## Technologies Used

- **HTML5**: Semantic markup and form elements
- **CSS3**: Custom styling with CSS variables and animations
- **JavaScript (ES6+)**: Modern JavaScript with async/await
- **Bootstrap 5**: Responsive framework and components
- **Font Awesome**: Icons and visual elements
- **jQuery**: DOM manipulation and event handling

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

- Lazy loading of page components
- Efficient DOM manipulation
- Optimized API calls
- Responsive image handling
- Smooth animations and transitions

## Future Enhancements

Potential improvements for the system:
- Two-factor authentication (2FA)
- Social media login integration
- Password strength meter
- Account lockout after failed attempts
- Email templates customization
- Multi-language support
- Dark mode theme

## Support

For technical support or questions about the implementation, please refer to the code comments and this documentation.

## License

This project is created for educational and demonstration purposes.

