# My English Story — Single HTTPS Web App

Built for The First British Center for Online Education.

## Included
- Single-page responsive web app
- Official center logo in `assets/logo.png`
- Stage 1: personal vocabulary and information
- Stage 2: word substitution + sentence builder + A/B conversation
- Stage 3: AI-style conversation practice, speech recognition, speech playback, role swap
- Stage 4: automatically generated personal paragraph + reading practice
- Stage 5: camera/microphone + achievement certificate + WebM recording
- Local progress persistence with localStorage
- HTTPS redirect via `.htaccess`

## Deploy to Hostinger
1. Create/use your domain or subdomain.
2. Open File Manager → `public_html` (or the subdomain document root).
3. Upload `index.html`, `.htaccess`, and the `assets` folder.
4. Make sure `assets/logo.png` exists.
5. Enable an SSL certificate in Hostinger.
6. Visit the HTTPS address.

Example:
`https://your-subdomain.example.com/`

## Important browser requirements
Camera, microphone and speech recognition require HTTPS (localhost is also normally treated as secure for development).

## AI voice
This first version uses browser speech synthesis for spoken AI prompts and browser speech recognition for student responses. It is intentionally API-key-free.

For a production version with a specific natural teenage-girl AI voice and true conversational AI, connect:
- Speech-to-text provider
- LLM conversation endpoint
- Text-to-speech provider

Never put secret API keys directly into `index.html`. Put them behind a server-side API.

## Data
Student data is stored locally in the browser in this version. It is not a multi-device school database yet.
