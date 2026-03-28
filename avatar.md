# Avatar Video Plan

avatar video: ~/Downloads/AVATAR.mp4

Use the Remotion best practices skill.

I've placed my talking-head video in public/avatar.mp4. This is a 9:16 vertical video (1080x1920) of me talking to camera, a selfie-style shot where my face is in the lower 60% of the frame, with open space above my head.

Create a Remotion composition (1080x1920, 30fps) playing this video FULL FRAME as the background layer, then overlays animated graphics on top, specifically in the open space above my head (roughly the top 35-40% of the frame). The video itself is never cropped, split, or resized.

SAFE ZONE: All overlay text and graphics must stay within the safe zone, at least 150px from the top and 170px from the bottom. Side margins: 60px minimum. MINIMUM FONT SIZES: Headlines 56px+, body/subtitles 36px+, labels/small text 28px absolute minimum.

## STEP 1, TRANSCRIBE & PLAN: Use Whisper to transcribe public/avatar.mp4. Identify:
- Total duration (set composition length to match)
- 3-5 key topic segments with start timestamps
- For each segment, propose an overlay graphic for the top portion of the frame:
  - Topic title with large step number ("01" faded in background, headline below)
  - Keyword pill/badge highlighting current topic
  - Simple animated icon or diagram
  - Progress bar showing position in video

Show me transcript segments and proposed overlays. Wait for approval before coding.

## STEP 2, BUILD:

BASE LAYER: <OffthreadVideo> filling entire 1080x1920 composition. This is the background. Never cropped, resized, or split.

OVERLAY LAYER (positioned in top ~35% of frame, above my head):
- Dark gradient overlay ONLY in top 40% of frame (transparent at bottom, rgba(0,0,0,0.6) at top) for text readability
- Large faded step number ("01", "02"), Inter 800, ~200px, 8% opacity
- Topic headline, Inter 700, 56-64px, white
- Keyword badge, rounded pill with glass-morphism background, 32px text
- Animated progress bar, thin line showing progress through current segment
- Each overlay synced to transcript timestamps using Sequence components

OPTIONAL BOTTOM OVERLAY, CAPTIONS:
- Word-level timestamps from Whisper, animated captions at y: 1600-1700px
- Bold white text, 36px, with text shadow
- Current word highlighted in accent color (#6366f1)

PREVIEW: After building, launch Remotion Studio (npx remotion studio) so I preview the video in my browser.
