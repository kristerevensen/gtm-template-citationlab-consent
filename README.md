# CitationLab Consent — Google Tag Manager template

Runs CitationLab's cookie banner and consent management from Google Tag
Manager, with Google Consent Mode v2.

## Install

1. Add the template: search for **CitationLab Consent** in the Community
   Template Gallery (Tags → New → Tag Configuration → Discover more tag types),
   or import `template.tpl` under Templates → Tag Templates → New → ⋮ → Import.
2. Create a **CitationLab Consent** tag and paste your project token. You find
   it in CitationLab under Cite Consent → Install.
3. Fire it on **Consent Initialization - All Pages**, then submit and publish the
   container. Remove any other tag in the container that sets Consent Mode
   defaults.

The banner's texts, categories, regional rules and design are managed in
CitationLab and take effect when you publish them there — the tag does not need
to change.

## What the tag does

- Sets Google Consent Mode v2 defaults: every signal denied until the visitor
  decides, `security_storage` granted. Add rows under *Regional defaults* to give
  a region a different default.
- Applies a returning visitor's earlier decision before any other tag in the
  container fires.
- Shows the banner and passes each decision to Google Tag Manager the moment the
  visitor makes it.

## Tag Manager or the page?

Loaded from Tag Manager, the banner governs the tags in your container. Scripts
pasted directly into the site's HTML start before Tag Manager does. If the site
has such scripts, paste the CitationLab Consent script at the top of `<head>`
instead (Cite Consent → Install) and leave this tag out.

## License

Apache 2.0 — see [LICENSE](LICENSE).
