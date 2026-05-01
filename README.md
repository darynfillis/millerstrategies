Miller Strategies verbatim HTML site. Pure HTML/CSS with vanilla JS mobile navigation. Add hero-video.mp4, hero-poster.jpg, and approved headshots before launch. Verbatim team bios and testimonials sourced from millerstrategies.com.


## Logo and favicon update
- Header now uses `assets/miller-strategies-logo.svg`.
- Favicon now uses `assets/favicon.svg`, cropped from the Capitol dome mark in the official logo file.


## Headshots and hero video
- Hero video added as `hero-video.mp4`.
- Hero poster added as `hero-poster.jpg`.
- Team headshots assigned based on uploaded file names.
- Steve Ruppel did not have a matching uploaded headshot file in this batch, so his placeholder remains.


## Final media update
- Steve Ruppel headshot added and assigned.
- Favicon replaced with transparent PNG: `assets/favicon.png`.


## CTA animation update
- CTA buttons now use a subtle floating animation via CSS.
- Animation respects `prefers-reduced-motion`.


## Phone icon update
- Replaced the old text phone symbol with a modern inline SVG phone icon.
- Restored subtle phone pulse animation on the header phone CTA.


## Mobile header and CTA spacing update
- Hero CTA buttons now have more spacing.
- Phone and Contact remain visible in the mobile header.
- Header Contact button no longer floats on the navigation line.
- Hamburger menu remains available on mobile.


## Contact form update
- Added `Company name` field to the contact page form.


## News and client logo update
- News page expanded with relevant public coverage and external article links.
- Client page expanded to include logos for the broader client roster.
- Logos use Clearbit-hosted logo URLs with an initials fallback when no logo is available.


## News sort and client review card update
- News articles now sort newest first.
- Client testimonials now live on the matching client logo cards.
- Cards with reviews show a red quote icon and expand on click.
- WellHive and National Fisheries Institute reviews are not assigned because those client cards are not in the current roster grid.


## Client logo reliability update
- Added WellHive and National Fisheries Institute client cards.
- Attached their client reviews to their cards.
- Replaced external logo pulls with local SVG logo cards in `assets/client-logos/` so logos render consistently without relying on Clearbit/external requests.
- Note: these are local branded client cards using names/initials, not official trademark artwork. Replace with approved official logo files later if desired.


## Principal bio rewrite
- Rewrote principal bio pages to be client-facing.
- Bios now emphasize the client problem, relevance, credibility, practical outcome, and when to engage each principal.
- Staff and Of Counsel bios were not changed.


## Client logo, review icon, and legal page update
- Client cards now render directly in HTML/CSS and no longer depend on external logo services or image files.
- Quote/review icons are larger and white for stronger contrast.
- Added Accessibility, Privacy Policy, and Terms of Use pages.
- Footer now links to Accessibility, Privacy Policy, and Terms of Use.


## Profile quote, client card, and navigation update
- Client cards now render directly in HTML/CSS with no image or external logo dependency.
- Client review quote icons were enlarged again and set in white for contrast.
- Broadcom quote was removed from all profile pages except Jeff Miller.
- Jeff Miller profile now includes the Broadcom quote with source attribution.
- Added a horizontal photo profile reel to each individual profile page for easier team navigation.


## Profile reel and quote icon update
- Reduced client review quote icon size.
- Rebuilt profile navigation reel as a continuous right-to-left auto-scroll.
- Profile reel pauses on hover/focus so users can click.
- Each reel card links directly to the matching profile HTML page.


## Interactive profile reel update
- Rebuilt profile carousel with JavaScript instead of CSS animation.
- Clicking a profile card now explicitly navigates to the correct profile page.
- Reel scrolls right-to-left automatically.
- Mouse position changes speed: left side slows, right side accelerates.
- Added left/right arrow controls.


## Mobile reel, services, quotes, and client card update
- Profile reel now supports mobile touch: slow auto-scroll, swipe/drag, tap-to-open, and resume after touch.
- Desktop profile reel speed still changes by mouse position.
- Services page now shows all details directly; expand/collapse removed.
- Client reviews are smaller and less bold.
- Testimonials naming principals are added to the corresponding principal profile pages with source attribution.
- Client cards no longer rely on image logos or external logo services.


## Profile restoration
- Regenerated all individual team profile pages as standalone HTML pages.
- Restored profile navigation reel on every individual page.
- Team profile links point to individual `.html` pages.


## Five-law profile bios update
- Rewrote all individual profiles to lead with client-facing value.
- Each profile now includes five-law framing: problem solved, how they help, why it matters, proof/perspective, and when to engage.
- Jeff's profile now foregrounds client value while retaining major accolades and outside roles.
- Applied the same logic to principals, of counsel, and staff profiles.


## Profile nav and prose bio cleanup
- Removed script-driven profile carousel that interfered with profile clicks.
- Replaced it with native horizontal scrolling links and optional arrow buttons.
- Removed five-law cards from individual bios and converted the content into written prose.


## Bio and profile review cleanup
- Removed “Client perspective” labels from profile review boxes.
- Removed five-law labels such as “How she helps,” “Why it matters,” “Proof and perspective,” and “When to engage.”
- Bios now read as prose rather than labeled framework cards.
- Preserved native clickable profile navigation.


## Logo and legal policy update
- Client cards now use Google favicon logo icons with initials fallback. This is more reliable than Clearbit for many domains, but approved local SVG/PNG logo files remain the best final solution.
- Expanded Privacy Policy and Terms of Use pages with more standard website policy language.
- Accessibility page updated with stronger WCAG-oriented language.
- Footer contact information retained with clickable address, phone, and email.


## Social icons update
- Added company social icons to the footer: LinkedIn, X, and Facebook.
- Added individual LinkedIn icons only where the exact public profile URL was identified with high confidence: Jeff Miller, Jessica Mandel, Jonny Hiler, James Min, and Cate Redmond.
- Did not add personal social links for other team members without confirmed URLs.


## Services content restored
- Rebuilt `services.html` with all six full service cards and detail text.
- Removed expand/collapse behavior from the Services page.
- Preserved one cited GE Aerospace quote.
- Preserved social footer and legal/profile updates from the current package.


## Instagram and social spacing update
- Added company Instagram to the footer: https://www.instagram.com/miller_strategies/
- Added Jeff Miller Instagram to his profile: https://www.instagram.com/millertimeintx/
- Added spacing between profile social icons and the Start a Conversation button.


## Jeff Miller YouTube embed
- Added responsive YouTube embed to `jeff-miller.html`.
- Source video: https://www.youtube.com/watch?v=srJpjKBlCJY


## Jeff Miller YouTube embed fallback
- Replaced the standard YouTube embed with the privacy-enhanced YouTube-nocookie embed.
- Added a direct “Open Video on YouTube” fallback button.
- If YouTube or the video owner blocks embedded playback, the direct YouTube link will still work.


## Jeff Miller video Error 153 fix
- Removed the embedded YouTube iframe from Jeff Miller’s profile because YouTube Error 153 can be caused by referrer/browser restrictions outside the page’s control.
- Replaced the embed with a YouTube preview card that opens the video directly on YouTube.
- Added `<meta name="referrer" content="strict-origin-when-cross-origin">` site-wide for future embed compatibility.


## Jeff Miller official YouTube embed
- Replaced the preview card with the exact YouTube embed code provided by the user.
- Kept a direct fallback button below the embedded video.
- Kept `strict-origin-when-cross-origin` referrer policy site-wide.


## Jeff Miller YouTube IFrame Player API update
- Replaced the static YouTube iframe on `jeff-miller.html` with the official YouTube IFrame Player API.
- The API loads `https://www.youtube.com/iframe_api` and creates a player for video ID `srJpjKBlCJY`.
- Added an inline error message if the player fails to create.
- Kept the direct YouTube fallback button below the player.


## Review audit
- Audited displayed testimonials against the approved review set.
- Removed/replaced generic placeholder testimonials where found.
- Ensured profile reviews and client-card reviews use approved wording and source attribution.
- Added `REVIEW-AUDIT.md` to the package.


## Services GE Aerospace quote citation fix
- Added attribution for Pete Giambastiani, VP for Global Government Relations, GE Aerospace, to the services page quote.
