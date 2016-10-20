# IG-eStatements

Notes
-----
- Typography in PDF is difficult to rely on: the PSD has been used as precedence
	- typography has no line heights (leading), and there is no medium size flat; line height has been guessed
	- pdf for section header on 'about' has 05 font for large, but 04 font for small... 04 is different for large versus small in summary
	- 04 is depicted as 28px in PSD, cited as 24px in PDF; 28 has been used in CSS
	- 02: callout title becomes content title... Medium size matches small in summary
	- callout body copy shifts from 07 to 06??

- grid in PDF does not match foundation's grid; attempts have been made to match the intent of the PSDs within the foundation grid

- space above section header is inconsistent; using 'about' section spacing across all
	- as a corollary, using about spacing as basis for collapsed section bar

- large to medium on about was a concern; this gets quite crushed following the margins in the guide, so an additional breakpoint was added to reduce the margins at an intermediate stage

- hover for primary button means text will match the background color... Added hover effect of transparent background to compensate

- alignment of dropdown conflicts between PSD and PDF: using PSD to style

- mailto link? Really? That is the only conclusion that can be drawn from the PSD's rendering of the dropdown.

- spacing below 'learn more' link inconsistent between layer comps

- 11 number callout is medium in PDF, semibold in PSD... PSD used. This in addition to a fundamentally different font class being used for mobile in the main profile.

- various spacings and font properties are inconsistent across the sections, as well as internally within a section; the first encountered instance has been used as a standard across all variants, and the rendered site will only perfectly match the PSD for these instances

- bordering between sections on mobile has been inconsistent; I have not yet applied these, and will examine what the rule/intent is

- MAPS (general inquiries):
	- in general, providing an address in the h3 will result in the appropriate map, however for problematic addresses, lat & lng can be manually determined and added as an attribute to the .map-icon (examples for both have been provided)
	- zoom is set to 15; this can be overridden with a data-zoom attribute on the .map-icon element
	- iconLocation in app.js may need updating based on site structure
	- google developer account info:
		- account email: ig.fall.campaign@gmail.com
		- account pw: fallcamp
		- account key: AIzaSyDtM1GEOMvof3wP-LOZnei_p19te8PeN2M

- Organization icons are centred vertically -- actual icons would need to be prepared with whitespace if required to ensure their centers are weighted correctly. I am assuming the icons in this piece are placeholders due to their low quality, and are simply cut to the bounding box

- modal contact link font size reduced, as it would unlikely fit without wrapping in most cases


Todo:
- check height under events tagline
- examine iphone issue with small icon grid display