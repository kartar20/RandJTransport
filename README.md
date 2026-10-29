# R and J Transport Ltd website

Open `index.html` in any modern browser. No installation, build step or server is required. Google Fonts needs an internet connection; system fallback fonts work offline. The Google Maps link opens an address search.

## Editing

- Text: open the relevant `.html` file in a text editor and change the content inside the HTML tags.
- Colours: edit the variables at the top of `css/style.css`. `--blue` is the brand blue, `--deep` is the darker blue, and `--accent` is the silver-grey accent and `--yellow` is reserved for the registration plate and hazard stripe. Dark mode follows the visitor’s system preference; edit its variables inside `prefers-color-scheme: dark`.
- Contact details: search all four HTML files for the phone, email or address and replace each occurrence. Update `tel:+447814727388` and `mailto:info@randjtransport.com` as well as the visible text. Update the Google Maps address query in `contact.html` if the address changes.
- Header and footer: these are repeated in each HTML file so every page works independently. Apply shared edits to all four files.
- New page: copy an inner page, rename it (for example `fleet.html`), then change its title, meta description, banner and main content. Add its navigation link to every page. Set `aria-current="page"` only on the link matching the current file. Keep the shared CSS and script links.

## Accessibility and maintenance

The mobile menu uses `js/main.js`. Without JavaScript, navigation stays visible. Keyboard focus, a skip link, reduced motion and system dark mode are included. The contact form uses FormSubmit; no tracking or frameworks are added.

Company information is supplied by the business. Review accreditation and waste registration details when they change. The registration is displayed as active through 6 December 2028. The FORS explanation links to the scheme’s official guidance.

## Photos

The Home and About pages use the original lorry photographs in `Photos/`. Publish the `Photos/` folder alongside the HTML and CSS so the photographs load online. Keep the capital P in the folder name and preserve the filenames. To change a photograph, replace its file or update its `src`, descriptive `alt` text, and intrinsic width and height in the HTML.

## Contact form activation

The Contact page has two visible fields: name and message. Messages are posted to `https://formsubmit.co/info@randjtransport.com` for email delivery using FormSubmit's free service. Visitors should include a phone number or email address in the message if they want a reply.

After publishing, submit a test message from the live website. FormSubmit sends an activation email to info@randjtransport.com: the mailbox owner must click the confirmation link before delivery is enabled. Check spam if it does not arrive. Then submit another test and confirm it reaches the inbox. The form uses FormSubmit's default spam checks and confirmation page; it requires an internet connection and should be tested on the hosted site, not a file URL. Delivery has not been verified during implementation.

To change the receiving email, edit the form's `action` in contact.html and activate the new address. Documentation: https://formsubmit.co/documentation
