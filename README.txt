SAFESPACE AI WORLDWIDE — v0.8 GLOBAL SAFETY & SUPPORT EXPERIENCE

This package builds on the v0.7 prototype and adds a Global tools panel for the first seven development priorities. It preserves the existing Right Now emergency app, organisation portal, AI workflow panel, human review UI and administrator UI from v0.7.

WHAT IS INCLUDED
1. Global emergency assistance and country selection
   - Country selector and country-specific emergency-number reference for a starter set of countries.
   - South Africa is selected by default.
   - Emergency numbers are reference information; confirm them with official local authorities before production use.
2. Nearby support discovery
   - Search by city/suburb/postcode using an external map search.
   - Optional browser geolocation after explicit browser permission.
   - Coordinates are used only to open the external map search; this feature does not save or send them to SafeSpace servers.
   - External search results are NOT verified by SafeSpace. Users must check providers independently.
3. Safe Check-in and Safety Exit
   - Private reminder is stored locally in this browser; keep the page open for the timer.
   - It does not notify trusted contacts, emergency services or SafeSpace staff.
   - Quick Exit displays a neutral screen. It cannot clear browser history, network logs, screenshots or monitoring software.
4. Organisation verification and management
   - Existing organisation application and admin-review UI is retained.
   - Verification still requires a trusted server and an authorised administrator; no client-side self-verification is added.
5. AI-powered operational workflows
   - Existing AI workflow and human-review UI is retained.
   - AI suggestions remain drafts; no automatic dispatch, referral or external task execution.
   - Do not enter survivor case data or sensitive personal information.
6. Multilingual and accessibility support
   - Language selector includes a limited English, isiZulu and Afrikaans interface translation preview for the Global tools panel.
   - This is not a complete translation of the whole app. Further translation review and accessibility testing are required.
7. Platform analytics and reporting
   - Local browser-only counters for opening tools, searches, check-ins and quick exits.
   - No central reporting, cross-user analytics or personal tracking is performed by this layer.

IMPORTANT IMPLEMENTATION LIMITATIONS
- The v0.7 folder supplied as the base contains index.html, README.txt and CHANGELOG.txt only. It does NOT contain the backend package/server or Firebase deployment files described in the v0.7 README. Therefore this v0.8 package is a front-end prototype; existing sign-in, Firestore, AI, organisation approval and admin operations will not become live merely by opening this HTML file.
- Do not deploy this as a production emergency service. Verify emergency numbers, providers, security rules, backend endpoints, authentication, App Check, privacy impact and incident response before launch.
- Existing Firebase project target remains safe-space-ai-b19f9. No Firebase rules or database are changed by this package.

RUN
1. Extract the ZIP.
2. Open index.html in a modern browser to preview the existing app and Global tools panel.
3. For browser geolocation, notifications, and production Firebase/API integrations, serve the site from localhost or HTTPS; opening as a file may restrict browser features.
4. Test country switching, map search, location permission, check-in timer, quick exit, language selector and local counters.

PRIVACY
Never send survivor names, phone numbers, addresses, ID numbers, case notes, medical information, safety plans or emergency reports to AI tools, Switch, analytics or organisation workflows.
