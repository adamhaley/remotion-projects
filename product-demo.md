# Product Demo Video Plan

Use the Remotion best practices skill.

Create a 25-second product demo and launch video (1080x1920, 30fps) for the product at https://app.megyk.com

SAFE ZONE: All text and key content must stay within the safe zone, at least 150px from the top (platform search bars, status bar) and 170px from the bottom (navigation buttons, swipe-up UI). Side margins: 60px minimum. Nothing important should touch the edges. MINIMUM FONT SIZES: Headlines 56px+, body/subtitles 36px+, labels/small text 28px absolute minimum. Nothing under 28px, it's unreadable on mobile.

## STEP 1, RESEARCH & ASSET DOWNLOAD: Visit the URL. Extract:
- Product name and logo (download any logo/favicon to public/)
- Brand colors (pull from the site's CSS or visible design)
- Tagline / hero headline
- The core user flow (what does someone DO with this product?)
- 3 key features or value propositions
- Any social proof (user counts, testimonials, logos)
- IMPORTANT, PRODUCT IMAGES: Use the Claude in Chrome MCP tools to navigate to the website, read the page, and find product screenshots/images the site already displays (hero images, product UI screenshots, feature images, app previews). Download 2-3 of the best product images and save them to public/. Prefer PNG/JPG product mockups over generic stock photos.
- Only take browser screenshots as a LAST RESORT if the website has no downloadable product images.

Show me what you found and a proposed 6-scene outline. Wait for approval before coding.

## STEP 2, BUILD THE VIDEO: After approval, build 6 scenes:

### SCENE 1 - Hook (3s):
- Bold text in safe zone: a pain-point question relevant to the product
- Text slams in with spring from 2x scale, holds 2s, fades out
- Dark background with subtle brand-color radial glow

### SCENE 2 - Product Intro (3s):
- Product name/logo scales in with spring from 3x to 1x
- Real tagline slides up below
- Particle burst behind logo using brand accent color

### SCENE 3 - Simulated Demo (8s):
- Recreate a simplified, MOBILE-SIZED version of the product's core interaction using React components
- NO device mockup frame, build UI elements directly on dark background, large enough to fill safe zone width (960px+)
- Animate a cursor moving to input field, typing, clicking submit, showing results
- All cursor movement uses spring({ damping: 15 }) for natural motion
- Everything must be readable on a phone screen, if in doubt, make it bigger

### SCENE 4 - Product Image Showcase (5s):
- Display downloaded product images LARGE (900px+ width), centered with drop shadow and rounded corners
- NO device mockup frame, product images already look polished
- Animate through 2-3 images with crossfade transitions
- Feature headline (56px) fades in above/below each image

### SCENE 5 - Feature Callouts (3s):
- Product image scales down to 40%, moves to top
- 3 feature benefit lines animate in below (36px+ text)
- Each line has a colored icon + short text pulled from real features

### SCENE 6 - Social Proof + CTA (3s):
- Social proof number counts up from 0
- Product URL pulses gently above bottom safe zone
- Fade to black

## BACKGROUND MUSIC (REQUIRED):
vibey electronic music
