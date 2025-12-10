# Studio Sariya Consent Form

A beautiful, modern, and professional consent form for Studio Sariya eyelash extension services.

## Features

- Modern, responsive design using Tailwind CSS
- Professional gradient styling
- All required form fields:
  - Name
  - Email
  - Phone number
  - First time getting eyelash extensions? (Yes/No)
  - Able to sit still for 3 hours? (Yes/No)
  - Consent to be touched around the eye area (checkbox)
  - Allergies text box
  - Terms and conditions checkbox (required)
- Form validation
- JSON POST request to `/submit` endpoint
- Loading states and error handling

## Setup

Simply open `index.html` in a web browser. The form uses Tailwind CSS via CDN, so no build process is required.

## Backend Integration

The form sends a POST request to `/submit` with the following JSON structure:

```json
{
  "name": "string",
  "email": "string",
  "phone": "string",
  "firstTime": "yes" | "no",
  "sitStill": "yes" | "no",
  "consentTouch": true,
  "allergies": "string",
  "terms": true
}
```

Make sure your backend server has an endpoint at `/submit` that accepts POST requests with JSON data.

## Customization

The form is designed to be easily customizable. You can modify:
- Colors (currently using purple/pink gradient theme)
- Additional fields can be added to the form
- Styling can be adjusted via Tailwind CSS classes

