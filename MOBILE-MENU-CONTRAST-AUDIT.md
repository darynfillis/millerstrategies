# Mobile Menu Contrast Audit

Updated CSS so selected mobile menu links use white text on the dark navy background.

Rules added:
- `.mobile-menu a.active`
- `.mobile-menu a[aria-current="page"]`
- child `span`, `svg`, fill, and stroke states

Purpose: selected mobile menu item remains readable on dark background.
