# Google OAuth Setup Guide

✅ **CONFIGURED** - Your Google OAuth is already set up with Client ID: `880790160266-nheta7vamr068cs7u4rm5upimu176l5t.apps.googleusercontent.com`

## Setup Complete ✅

Your Google Sign-In is now fully functional! Here's what was configured:

## 1. Create a Google Cloud Project

1. Go to the [Google Cloud Console](https://console.cloud.google.com/)
2. Create a new project or select an existing one
3. Enable the Google+ API (or Google Identity API)

## 2. Configure OAuth Consent Screen

1. In the Google Cloud Console, go to "APIs & Services" > "OAuth consent screen"
2. Choose "External" user type
3. Fill in the required information:
   - App name: "EcoLearn"
   - User support email: your email
   - Developer contact information: your email

## 3. Create OAuth 2.0 Credentials

1. Go to "APIs & Services" > "Credentials"
2. Click "Create Credentials" > "OAuth 2.0 Client IDs"
3. Choose "Web application"
4. Add authorized JavaScript origins:
   - `http://localhost:3000` (for local development)
   - `https://yourdomain.com` (for production)
5. Copy the Client ID

## 4. Update the Sign-In Page ✅

Your Client ID is already configured: `880790160266-nheta7vamr068cs7u4rm5upimu176l5t.apps.googleusercontent.com`

## 5. Configure Authorized Origins

Make sure to add these URLs to your Google OAuth settings:
- `http://localhost:3001` (for development)
- `http://127.0.0.1:3001` (for development)
- Your production domain (when you deploy)

## 5. Test the Integration

1. Open `signin.html` in your browser
2. Click "Continue with Google"
3. Complete the OAuth flow
4. Verify that user data is stored in localStorage

## Security Notes

- Never expose your Client Secret in frontend code
- Use HTTPS in production
- Configure proper redirect URIs
- Review OAuth consent screen settings

## Troubleshooting

- Make sure your domain is added to authorized origins
- Check that the Google+ API is enabled
- Verify the Client ID is correct
- Ensure the OAuth consent screen is properly configured


