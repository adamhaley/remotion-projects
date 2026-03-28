# Remotion Video Plan

Use the Remotion best practices skill.

Create an educational explainer video (1080x1920, 30fps, 30 seconds) teaching "How AI Agents Work".

## SAFE ZONE
All text and key content must stay within the safe zone, at least 150px from the top (platform search bars, status bar) and 170px from the bottom (navigation buttons, swipe-up UI). Side margins: 60px minimum. Nothing important should touch the edges. MINIMUM FONT SIZES: Headlines 56px+, body/subtitles 36px+, labels/small text 28px absolute minimum. Nothing under 28px, it's unreadable on mobile.

## STEP 1, RESEARCH & SCRIPT
Before writing any code, research the topic and write a 5-scene script. Each scene needs: a one-line headline, 1-2 sentences of explanation, and a visual description of what to animate. Show me the script and wait for approval before coding.

## STEP 2, DESIGN & ANIMATE
After I approve the script, build all 5 scenes with these specs:

### VISUAL STYLE:
- Background: #0a0a0a
- Primary text: white
- Accent: #6366f1 (indigo)
- Success/emphasis: #22c55e (green)
- Font: Inter (weights 400, 600, 800)
- All icons/diagrams built as SVG components (no external assets needed)

### ANIMATION RULES:
- Every element enters with spring({ damping: 200 }), no linear motion
- Stagger related items by 8-12 frames
- Use TransitionSeries with 12-frame fade transitions between scenes
- Diagrams and flowcharts should draw themselves (SVG stroke-dashoffset animation)
- Key numbers use count-up animation with interpolate() and tabular-nums
- Final scene: particle effect background (10-15 circles drifting upward)

Each scene should have a clear visual metaphor, diagrams, flowcharts, icons, or step-by-step animations. No walls of text. Think Kurzgesagt: beautiful motion, fast pacing.

## BACKGROUND MUSIC (REQUIRED, do not skip this step):
1. Search Pixabay for a royalty-free lo-fi or electronic beat
2. If it fails, search for any free-to-use .mp3 beat online and download it to public/music.mp3
3. If all downloads fail, generate a simple rhythmic beat programmatically
4. Add the audio file to the composition using Remotion's <Audio> component with volume set to 0.3
5. The music MUST loop for the full video duration

This is not optional. Every video needs background music.
