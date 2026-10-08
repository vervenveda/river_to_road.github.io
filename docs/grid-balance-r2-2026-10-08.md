# River-to-Road grid balance — revision 2

## Current source and application status

Based on main commit `0d7ef34e1e884ba0fdae80b60bcd14ee24cda9c2`, with index blob `38d07a09b0249f8ebf6622a4d11b78790628d95c`.
The current repository index includes the previous repair package. These NEW layout and link changes are tested locally and packaged for upload; they have not been committed by this assistant because GitHub integration write access was previously denied.

The user's screenshots showed uneven action-button baselines and 10-card sections wrapping as 4 + 4 + 2. The prior fixed 18px button top margin allowed action buttons to sit at different heights; R2 restores automatic top spacing and puts the minimum gap on the preceding content instead.

## Changes

- All card buttons stay at the bottom of the card with at least 18px clearance from preceding content and a consistent 64px minimum height.
- Event finders, news, and network: 5 columns from 1200px upward, 2 columns at intermediate widths, 1 column on phones. Each has 10 cards, so all rows are complete.
- Games: added EPA Recycle City for 12 games, giving 4 × 3 on desktop, 3 × 4 on smaller desktops, 2 × 6 on tablets, and 1 column on phones.
- All 28 resource cards use 4, 2, or 1 columns, avoiding a lone last card at tablet widths.
- Action pathways remain 3 × 2 on desktop, calendar 3 × 4, and safety 4 × 2.
- Jennifer Pearl 2028 now links directly to `https://jenniferpearl2028.github.io/`, verified with HTTP 200 and the title "Jennifer Pearl for President 2028". The Verve N Veda campaign gateway identifies this as the official campaign website.
- Recycle City points to `https://www3.epa.gov/recyclecity/games.htm`, verified with HTTP 200 and title "Play the Games | Recycle City | U.S. EPA". This is its game collection page; full external gameplay is not certified by this update.

## Checks

16 widths tested: 280, 320, 390, 560, 561, 760, 768, 840, 900, 1024, 1120, 1199, 1200, 1280, 1440, 1920 pixels.

At each width, every default grid has complete rows. Buttons in each row have matching top, bottom, and height within 1 pixel. No horizontal element overflow was found.

Resource search, filtering, reset, menu, downloads, print control, local anchors, both local game flows, and absence of JavaScript errors were rechecked successfully. Search results may naturally have an incomplete final row when the user filters the resource directory.

No existing links were removed in R2. The user's verification of the other existing buttons is retained; previous automated access-restriction results are historical test limitations rather than claims that those links are broken.

## Upload

Only the root `index.html` is changed by R2. Upload that file to the root of `vervenveda/river_to_road.github.io` on main. Do not overwrite newer changes from another conversation. The apps folder is included for checkpoint completeness and does not need to be uploaded again. Reports and previews are provided for review.
