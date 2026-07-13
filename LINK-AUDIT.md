# QDL Visual Guide Link and Function Audit

**Audit result: PASS**

- HTML pages checked: 10
- Link, image, manifest, and canonical references inspected: 432
- Unique same-site targets/fragments inspected: 47
- Unique external URLs inventoried: 37
- Inline JavaScript files syntax-checked: 4
- Poster images decoded and dimension-checked: 3

## Corrections made during audit

- The three animation pages now use relative same-site links rather than root-absolute links, so navigation works both after deployment and during local preview.
- Missing canonical links were added to the Structural Admissibility animation, the GM-to-QDC animation, and the Research Program page.

## Validation results

- Every same-site reference in the supplied update resolves either to a file included in this package or to an established existing website page/asset.
- Every fragment link targeting a supplied HTML page resolves to an existing element ID.
- All three poster images are valid 1600 × 900 PNG files.
- The QDL Calculator and all three animation scripts pass Node.js syntax validation.
- No duplicate HTML IDs were found.
- All external links opened in a new tab include `noopener noreferrer`.
- Every supplied HTML page has exactly one canonical link.

## External-link note

The audit inventories all external DOI, Zenodo, journal, Amazon, canonical, and community URLs. Their destinations remain controlled by third-party services and should be rechecked periodically. The QDL-site links and page/fragment structure are fully checked within the supplied deployment set.
