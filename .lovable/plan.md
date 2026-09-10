# 3D Genre and Storybook Selection

## Goal
Replace the current flat selection grid with an original, polished interaction inspired by the reference clip. The clip itself will not appear in the app.

## Experience
1. Present all 12 genres as a horizontal 3D cover-flow.
2. Keep one genre centered and prominent while neighboring covers recede and fan out in perspective.
3. Support mouse drag, touch swipe, trackpad/wheel scrolling, arrow buttons, keyboard arrows, and direct cover selection.
4. Clicking the centered genre transitions into a second cover-flow containing that genre’s storybooks.
5. Each storybook cover shows its title and existing progress state; selecting the centered book starts or resumes its six-question set.
6. Preserve the existing Back to genres path, questionnaire, scoring, saved progress, and dashboard updates.

## Visual Direction
- Create crisp original genre and storybook covers from HTML/CSS typography and themed visual treatments, rather than copying low-resolution frames or copyrighted cover artwork.
- Use depth, perspective, overlap, scale, soft shadow, and restrained motion to reproduce the clip’s shelf-like flow.
- Keep the current warm wellness palette and avoid changing the rest of the page theme.
- Make the focused cover readable and clearly selected; soften distant covers without hiding them.

## Responsive and Accessible Behavior
- Desktop: wide, draggable 3D fan with visible neighboring covers.
- Mobile: touch-first swipe with snap-to-center and smaller overlap, without horizontal page overflow.
- Add clear focus states, keyboard navigation, screen-reader labels, reduced-motion behavior, and stable cover dimensions.

## Technical Details
- Restructure the selection area into persistent genre and story stages so transitions can animate smoothly.
- Keep the imported questionnaire data and existing genre/story IDs as the single source of content.
- Add vanilla JavaScript carousel state for active index, drag/swipe thresholds, wheel navigation, centering, and stage transitions.
- Use CSS transforms and perspective for the cover-flow; no framework, carousel library, or embedded video.
- Verify all 12 genres, story loading, resume badges, six-question launch, desktop drag, mobile swipe, keyboard controls, and no overflow.
