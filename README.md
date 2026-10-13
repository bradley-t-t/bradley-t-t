## Trenton Taylor

I'm a full-stack developer in Baytown, Texas, and I run [TaylorURL](https://www.taylorurl.com). I'm the only developer, so every project below is mine from end to end: the database schema and its security policies, the server functions, the payments, the front end and the hosting. The client sites in the taylorurl.com portfolio average 98 on mobile and 100 on desktop in Google PageSpeed Insights.

Before TaylorURL I spent seven years at Smyrna Ready Mix, starting in the yard and finishing as District Manager over 13 concrete plants. The job needed software, so I built it, and its results are the first thing below.

**What I work with:** React 19, Next.js, TypeScript, Vite, Tailwind CSS, Supabase (Postgres, row-level security, Deno edge functions, Realtime), Prisma, Stripe, WebGL and GLSL, Node, Electron, Go, Java and Vercel.

Want something like this built? [Start a Project](https://www.taylorurl.com/start) or email [trenton@taylorurl.com](mailto:trenton@taylorurl.com).

### Sites I've Built

#### [Smyrna Tools](https://www.smyrnatools.com) · [Source](https://github.com/TaylorURL/smyrnatools-com)

Smyrna Ready Mix is the largest family-owned ready-mix concrete producer in the country, with 563 plants and 8,500 team members across 24 states. I built Smyrna Tools while running 13 of its plants, and it became the operations platform for two Texas regions, used at both the regional and district level.

- **Problem:** Fleet records, operator rosters and plant numbers lived in spreadsheets, on paper and in text threads, so every manager compiled their own reports and no two plants worked from the same numbers.
- **Results:** By the time I left, customer satisfaction was up 20% and the trucks were reaching about 40% more customer jobs on time. Every asset was verified weekly with its full history kept, the shop queue got trucks back on the road sooner, and every plant and region read the same live numbers.
- **Engineering:** It pulled dispatch orders straight from Jonel and time punches from Dayforce, and read industrial probes on the cement, fly ash and slag silos, so one analytics layer covered trucks, people and materials. Eleven statistics views break the fleet down by plant, including status, service, shop performance, hours, aging and verification, and any list exports to Excel.
- **Security:** The browser never writes to the database. Every change goes through one of 22 edge functions that check the account's permissions, row-level security shuts anonymous visitors out of every table, and login is a custom auth service with PBKDF2 hashing, HttpOnly session cookies and signed JWTs.
- **Skills:** React 19, TypeScript, Vite, Tailwind CSS, Supabase (Postgres, row-level security, Deno edge functions, Realtime, pg_cron), third-party system integration, analytics dashboards with Recharts, ExcelJS, Sentry, Vitest, CI.

#### [Hollingshead Harbor](https://hollingsheadharbor.com) · [Source](https://github.com/TaylorURL/hollingsheadharbor-com)

The marine arm of the same SRM family: bulk dry cargo, vessel and barge charter, and full-service ports across thirteen harbors.

- **Problem:** The company hires deckhands and wheelmen constantly, and an applicant standing on a dock with a phone won't come back to finish a PDF.
- **Engineering:** One schema file drives the form, the browser validation and the email, so the three can't drift apart. The serverless endpoint drops bots with a honeypot, accepts only real resume formats under 3 MB, never logs an SSN or date of birth, and mails the hiring inbox with the resume attached and the applicant set as reply-to.
- **Skills:** React 19, Vite, Tailwind CSS, Vercel serverless functions, Resend, conditional form design, handling sensitive personal data.

#### [Dickinson Bayou Fleeting](https://dickinsonbayoufleeting.com) · [Source](https://github.com/TaylorURL/dickinsonbayoufleeting-com)

Two gated five-acre waterfront yards, one on Galveston Bay and one on the Gulf Intracoastal Waterway at Freeport, leased by the month with the shore crew already on them.

- **Problem:** Fleeting is a phone-call business, and the operators comparing yards are often on a dock with one bar of signal.
- **Engineering:** Every route is prerendered to its own HTML page and the JavaScript is requested only after the first paint, so both monthly rates ($4,100 and $4,800) and the phone number show before anything else loads. The site search (slash or Cmd+K) and the structured data are generated from the same content files as the pages, and each loading placeholder takes the exact type size of the line it stands in for, so nothing jumps when content arrives.
- **Skills:** React 19, esbuild, Node build scripts, a hand-written router, JSON-LD structured data, accessibility, load-performance tuning.

#### [Faded Barber Shop](https://faded-barbershop.com) · [Source](https://github.com/TaylorURL/fadedbarbershop-com)

A Main Street barber in Liberty since 2018, on a page that is one continuous fade.

- **Problem:** A small shop needed a site people remember, which also answers the question most callers ring about: Friday is walk-in day.
- **Engineering:** A GLSL shader draws 540 columns of hair whose length follows your scroll, long at the top and taken down to skin at the bottom, and the section markers are clipper guard numbers 3, 2, 1 and 0. Your pointer shaves a path into a 128 by 72 grid that the shader reads, and the cut grows back over time. On machines that render WebGL in software the effects switch off.
- **Skills:** WebGL, GLSL shaders, Canvas 2D particles, React 19, Vite, server-side prerendering, reduced-motion support.

#### [Speedway 146](https://baytowngokarts.com) · [Source](https://github.com/TaylorURL/baytowngocarts-com)

An outdoor go-kart track on TX-146 in Baytown, with five-minute heats, indoor bounce houses, and a party room that seats sixty.

- **Problem:** The track needed parents to buy wristbands and book parties online instead of calling, without trusting the browser with the prices.
- **Engineering:** A server function re-prices every cart line against a fixed price list and rejects any line more than a cent off. It applies the 10% group discount for 15 or more, Texas sales tax and fees in whole cents, and only then opens Stripe Checkout. The Stripe webhook verifies its signature before recording a purchase, and row-level security locks the staff panel for orders, revenue and traffic.
- **Skills:** React 18, Vite, Stripe Checkout and webhooks, Supabase edge functions, Postgres row-level security, WebGL, server-side prerendering.

#### [Impressiva Printing](https://impressivaprinting.com) · [Source](https://github.com/TaylorURL/impressivaprinting-com)

Offset, digital, screen, direct-to-film and wide-format presses in one Pasadena shop, which is how it takes anything from a hundred business cards to a ten-foot vinyl banner.

- **Problem:** Artwork and proofs went back and forth by email, and customers had no way to see where their job stood.
- **Engineering:** The seven-stage job pipeline is enforced inside Postgres with no server code at all. Triggers police every stage change, customers can make only the moves that belong to them, such as approving a proof, and column-level grants limit them to the status column. Staff run the pipeline from a panel with a command palette and hotkeys that also works on a phone.
- **Skills:** React 19, Vite 7, Supabase Auth, Postgres triggers, row-level security, column-level grants, critical-CSS build tooling.

#### [Southeast Arbor Care](https://southeastarbor.com) · [Source](https://github.com/TaylorURL/southeastarbor-com)

The tree service Terry Lloyd started in Pasadena in 2000.

- **Problem:** A local service business lives on showing up in search for "tree removal" plus a town name, and on being easy to reach the night a storm hits.
- **Engineering:** 22 pages are rendered to static HTML at build time, and the sitemap is built from the files actually written. Each of the six towns gets a page about its own trees, the structured data leaves out any field the business hasn't confirmed, and one setting puts a storm-response bar with the phone number on every page. It scores 100 on mobile.
- **Skills:** React 19, React Router 7, Vite server-side prerendering, JSON-LD structured data, technical and local SEO.

#### [TireTracker](https://www.tiretracker.app)

Service records for commercial tire shops and the fleets they work on.

- **Problem:** Paper service tickets leave a shop and its fleet customer arguing about what was done to which tire on which truck.
- **Engineering:** Each shop's data is walled off in Postgres itself: every request runs under a restricted role with the shop set on the connection, row-level security covers 12 tables, and a test proves the isolation against a real Postgres. Photos taken on bad signal wait on the phone in IndexedDB and retry with backoff until they reach Cloudflare R2. About 400 tests cover 48 API routes.
- **Skills:** Next.js 16, React 19, Prisma, Postgres row-level security, multi-tenant design, Clerk, Stripe webhooks, Cloudflare R2, offline-first PWA, Upstash rate limiting, Sentry, Vitest.

#### [Compound Industrial Scale Services](https://ccscaleservices.com) · [Source](https://github.com/TaylorURL/ccscaleservicesinc-com)

A family-owned shop in Huffman that calibrates industrial scales against certified test weights, repairs them, and sells the parts.

- **Problem:** A customer with a failed load cell needs a price, and sales needs enough detail to quote it without calling back.
- **Engineering:** There's no database and no backend. Each of the 16 parts has its own URL with Product structured data, the quote list lives in the browser's local storage, and the request goes to sales as one composed email, with the text left on screen to copy if no mail app opens. The sitemap, robots.txt, llms.txt and business structured data are all generated from the same content files.
- **Skills:** React 19, React Router, Vite, schema.org structured data, technical SEO, client-side state.

#### [Dylan Jordan Real Estate](https://djrxexcellence.com) · [Source](https://github.com/TaylorURL/djrxexcellence-com)

Listings for Dayton and the Liberty County towns around it, sorted by town instead of by a radius on a map.

- **Problem:** A small-town agent needed one place where buyers search, save and compare homes and ask questions, with every lead landing with the agent.
- **Engineering:** Buyers save homes and searches, compare up to four side by side, and ask questions on the listing itself, where Dylan answers in the same thread. At build time the site pulls published listings from the database and writes a static page for each of its 25 routes, plus the sitemap. A script checks the row-level security policies against the live database as a visitor, a member and the agent in turn.
- **Skills:** React 19, React Router 7, Vite, Supabase (Postgres, Auth, Storage, row-level security), Leaflet maps, build-time prerendering, Vitest and Testing Library.

#### [DeluxFit by Angie](https://deluxfitbyangie.com) · [Source](https://github.com/TaylorURL/deluxfitbyangie-com)

A certified personal trainer's practice: memberships, online coaching and one-on-one sessions.

- **Problem:** Most trainers sell a plan and then run the client on spreadsheets and text threads. Angie needed the sale and the coaching in one app.
- **Engineering:** The checkout function calls Stripe's API directly for subscriptions and one-time payments, and the webhook verifies signatures itself with Web Crypto and a timing-safe compare. Private files sit in three locked buckets, reachable only through a function that checks the viewer is staff, the thread's owner or an assigned client before it issues a link that expires in 30 minutes.
- **Skills:** React 19, Vite 7, Supabase edge functions (15 of them), Storage signed URLs, Stripe API and webhooks, Radix, a separate design-system package.

#### [Delux Financial Solutions](https://deluxlavello.com) · [Source](https://github.com/TaylorURL/deluxlavello-com)

A Houston credit-education practice, with every page in English and Spanish.

- **Problem:** The practice serves clients in both languages, and every page had to read naturally in each.
- **Engineering:** Translation swaps text in place, keyed on the English sentence itself, so no component carries translation markup. Each of the 14 prerendered routes inlines only the Spanish strings it uses, the full 483-string dictionary loads only for Spanish readers, and tests load the built pages in jsdom to check what a reader actually sees. It scores 100 on mobile and desktop.
- **Skills:** React 19, Vite server-side prerendering, internationalization, jsdom testing, Python tooling.

#### [SETX Football](https://www.setxfootball.org) · [Source](https://github.com/TaylorURL/setxfootball-com)

A youth football camp in Daisetta for kids five to twelve, with no tryouts and no bench.

- **Problem:** Parents needed to sign up and order shirts quickly on a phone, and volunteers needed to check payments and run check-in on camp morning.
- **Engineering:** Parents register and order shirts without making an account, and a signed-out visitor can submit but read nothing back. A database trigger enforces the three-day edit window and stops families from marking their own registration paid, and the staff check in the security policies runs once per query instead of once per row. Volunteers verify CashApp payments and search and export the roster from a role-gated panel.
- **Skills:** React 19, Supabase Auth, Postgres row-level security and triggers, query performance, Radix, Jest.

#### [Southbelt Repair and Supply](https://southbelt.taylorurl.com) · [Source](https://github.com/TaylorURL/southbeltinc-com)

Concrete batch plants, the parts that keep them running, and the crews that fix them.

- **Problem:** A request has to reach the right desk (quotes, rentals or sales) with the machine already named, or it costs a callback.
- **Engineering:** Every request topic maps to a desk's inbox, and every quote button opens an email with the machine in the subject line. The 11 machines, 30 parts and used listings all carry Product structured data across 51 sitemap URLs, alongside 13 brochure PDFs. It's staged at southbelt.taylorurl.com ahead of its move to southbeltinc.com.
- **Skills:** React 19, Vite, React Router, schema.org structured data, sitemap generation, form validation.

#### [Root & Rise](https://www.rootriseholdings.com) · [Source](https://github.com/TaylorURL/rootriseholdings-com)

A trading desk and the platform it runs on.

- **Problem:** A trader needed risk rules that actually stop a bad trade, and a record of market calls that can't be edited after the outcome is known.
- **Engineering:** The journal refuses a trade that risks more than 1% of the account and locks the day after two losses in a row. Every two minutes a server cron reads market structure on nine instruments across three timeframes, publishes its calls first, and scores each one against the bars that follow. Each pass is idempotent and writes a heartbeat row, so a quiet morning and a broken data feed never look the same.
- **Skills:** React 18, Vite server-side prerendering, Supabase, Vercel cron functions, market-data integration, charting, about 250 tests on Node's built-in test runner.

#### [SouthBound](https://southboundofficial.website) · [Source](https://github.com/TaylorURL/southboundofficial-website)

A storefront and giveaway site for a truck-merch brand: shirts, hoodies, caps and decals.

- **Problem:** A giveaway has official rules, and the dates and prizes on the front page have to match them exactly.
- **Engineering:** One giveaway config feeds both the front page and the Official Rules page, so they can't disagree, and any value not set yet shows as missing instead of a placeholder date. The countdown waits for the visitor's own clock instead of showing the build time, and the rules include a free mail-in entry, so no purchase is necessary.
- **Skills:** React 19, Vite prerendering, React Router, sweepstakes rules.

### My Own Products

#### [DomeBreak](https://domebreak.com) · [Source](https://github.com/TaylorURL/domebreak-com)

A real-time missile strategy game played on the actual world map.

- **Problem:** Most missile-war games flatten the planet into an abstract grid. DomeBreak plays on the real one, with about 222 nations to choose from.
- **Engineering:** The simulation is a pure, deterministic engine that both the browser and an authoritative Node match server run, which keeps multiplayer in sync over WebSockets. The map is MapLibre GL reading PMTiles through a custom protocol, and the AI has layers for perception, threat maps, a fire solver, diplomacy (betrayal included) and five doctrines. It ships on the web and as an Electron app for macOS, Windows and Linux, with 685 tests.
- **Skills:** React 19, MapLibre GL, PMTiles, deterministic simulation, game AI, Node, WebSockets, Electron, Supabase, Vitest.

#### [Sunday](https://github.com/TaylorURL/sunday)

A checkpoint that runs before every action a coding agent takes.

- **Problem:** An AI coding agent reports what it believes it did, and nothing in the loop checks that report against what actually happened.
- **Engineering:** Sunday runs inside the agent harness before every tool call and at the end of every turn. It evaluates 33 YAML rules through a small all/any/not/count condition language, then steps aside, fixes the action, or stops it with a sentence the agent has to answer, catching things like "tests pass" after a failed test command or an edit to a file that was never read.
- **Skills:** Go (about 5,100 lines, one dependency, 94 tests), policy engines, agent tooling and hooks, cross-platform release builds.

### On My Own Time

- [kOS Flight Scripts](https://github.com/bradley-t-t/kos-flight-scripts): autopilots for Kerbal Space Program. A booster flies back and lands 0.57 m from its target on a barge, re-measuring its drag every flight and saving it for the next, and a capsule rendezvous and docks with a station from whatever phase it starts in. *Skills: guidance and control, orbital mechanics, KerboScript, multi-processor coordination.*
- [Telemetry Ground Station](https://github.com/bradley-t-t/telemetry-ground-station): mission control for a simulated two-stage rocket. The simulator integrates the flight with RK4 and sends CCSDS space packets over UDP through a link that drops, corrupts and reorders them, and in a recorded engine-out flight the ground flagged engine 5's failure 0.1 s after it happened. *Skills: Java 21 with no runtime dependencies, binary protocols, UDP, physics simulation, concurrency, server-sent events, JUnit 5.*
- [CryptoFort](https://github.com/bradley-t-t/cryptofort): an encrypted credential vault, published on npm, that lets an AI agent find the credential it needs without ever holding its value. Each secret is sealed with AES-256-GCM and bound to its own record, so it can't be moved to another one. *Skills: TypeScript, Web Crypto, MCP servers, SQLite, Postgres and Supabase adapters, Vitest.*
- [Viltrum Empire](https://github.com/bradley-t-t/stellaris-vilrumite-empire-mod): a Stellaris mod with more than 3,000 subscribers on the Steam Workshop, bringing seven factions from *Invincible* into the game with custom event chains and localization in 10 languages. *Skills: Paradox scripting, game balance, Steam Workshop publishing.*
- Six Prison Architect mods, built with Lua scripts and Python tools that generate the art and test the Lua against a stand-in for the game: [laser fences, and laser doors that open for staff but never for prisoners](https://github.com/bradley-t-t/prison-architect-sci-fi-security), [sci-fi furniture](https://github.com/bradley-t-t/prison-architect-sci-fi-objects) to match, [robot staff](https://github.com/bradley-t-t/prison-architect-robot-staff), a [crematorium](https://github.com/bradley-t-t/prison-architect-crematorium) that turns the hearse away, a [contraband checkpoint](https://github.com/bradley-t-t/prison-architect-contraband-checkpoint-scanner) room that searches anyone who steps in, and a [staffing terminal](https://github.com/bradley-t-t/prison-architect-auto-hire) that hires to the headcount you set. *Skills: Lua, Python, image processing, working inside a closed game engine.*

### Contact

[Start a Project](https://www.taylorurl.com/start) · [trenton@taylorurl.com](mailto:trenton@taylorurl.com) · [taylorurl.com](https://www.taylorurl.com)
