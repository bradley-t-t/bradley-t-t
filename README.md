## Trenton Taylor

I run [TaylorURL](https://www.taylorurl.com), a small web development company in Baytown, Texas. We build websites for shops and trades around Baytown and Houston, then keep looking after them once they're live. The twelve client sites in the taylorurl.com portfolio average 98 on mobile and 100 on desktop in Google PageSpeed Insights.

Before TaylorURL I spent seven years at Smyrna Ready Mix, starting in the yard and finishing as District Manager over 13 concrete plants. We needed software, so I built it, and then I left to do this full time.

Most of what's below runs on React, Vite, Tailwind CSS, Supabase and Vercel.

### Sites We've Built

#### [Smyrna Tools](https://www.smyrnatools.com) · [Source](https://github.com/TaylorURL/smyrnatools-com)

Smyrna Ready Mix is the largest ready-mix concrete supplier in the country, with 563 plants and 8,500 people across 24 states. Its Texas operations run on Smyrna Tools, which puts every mixer, tractor and trailer, every operator from first day to last, and the efficiency numbers for every plant behind one sign-in. I built it while I was running 13 of those plants. The browser never writes to the database; every change goes through a server function, and Postgres row-level security decides what each account can read.

#### [Hollingshead Harbor](https://hollingsheadharbor.com) · [Source](https://github.com/TaylorURL/hollingsheadharbor-com)

The marine arm of the same SRM family. It moves bulk dry cargo, charters vessels and barges, and runs full-service ports across thirteen harbors. The company hires constantly, so the employment application is a page of its own, laid out for a deckhand filling it in once, on a phone, standing on a dock. The browser checks it, the server checks it again, and then the server mails it to the hiring inbox with the resume attached.

#### [Dickinson Bayou Fleeting](https://dickinsonbayoufleeting.com) · [Source](https://github.com/TaylorURL/dickinsonbayoufleeting-com)

Two gated five-acre waterfront yards, one on Galveston Bay and one on the Gulf Intracoastal Waterway at Freeport, leased by the month with the shore crew already on them. Both rates are printed on the page, $4,100 and $4,800 a month, so an operator can compare yards without filling in a quote form. The whole site is black, white and gray, and small enough to load on a phone with one bar of signal out on a dock. Press slash anywhere to search every yard, rate and town it names.

#### [Faded Barber Shop](https://faded-barbershop.com) · [Source](https://github.com/TaylorURL/fadedbarbershop-com)

A Main Street barber in Liberty since 2018, on a page that is one continuous fade. A WebGL shader draws a field of hair that starts long at the top and gets taken down to skin as you scroll, the section markers are clipper guard numbers, and your pointer shaves a path through it as it moves. It also answers the question most callers are ringing about: Friday is walk-in day.

#### [Speedway 146](https://baytowngokarts.com) · [Source](https://github.com/TaylorURL/baytowngocarts-com)

An outdoor go-kart track on TX-146 in Baytown, with five-minute heats, indoor bounce houses, and a party room that seats sixty. A parent can buy wristbands or book a party through a cart and Stripe Checkout without calling. Before any money moves, a server function re-prices every line against the real price list, so a total edited in the browser doesn't survive the trip.

#### [Impressiva Printing](https://impressivaprinting.com) · [Source](https://github.com/TaylorURL/impressivaprinting-com)

Offset, digital, screen, direct-to-film and wide-format presses in one Pasadena shop, which is how it takes anything from a hundred business cards to a ten-foot vinyl banner. Customers upload their artwork, approve the proof, and follow the job through the same pipeline the press floor works from. Staff run that pipeline from an admin panel on any device.

#### [Southeast Arbor Care](https://southeastarbor.com) · [Source](https://github.com/TaylorURL/southeastarbor-com)

The tree service Terry Lloyd started in Pasadena in 2000. Every town the trucks work has a page about its own trees: water oaks and pines in Pasadena, what salt air does to a canopy in La Porte, the old live oaks around Clear Lake. When a storm comes through, one setting puts a storm-response bar with the phone number across the top of every page. It scores 100 on mobile.

#### [Compound Industrial Scale Services](https://ccscaleservices.com) · [Source](https://github.com/TaylorURL/ccscaleservicesinc-com)

A family-owned shop in Huffman that calibrates industrial scales against certified test weights, repairs them, and sells the parts. Every part has its own page, so someone searching for a failed load cell lands on that load cell. There's no server and no database. Parts go on a quote list kept in the browser, and the customer sends sales one email with the make, model and capacity of their scale already filled in.

#### [Dylan Jordan Real Estate](https://djrxexcellence.com) · [Source](https://github.com/TaylorURL/djrxexcellence-com)

Listings for Dayton and the Liberty County towns around it, sorted by town instead of by a radius on a map. Buyers save the homes worth a second look, compare their shortlist side by side, and ask questions on the listing itself. Dylan answers them there, and posts listings and reads leads from a dashboard on the same site.

#### [DeluxFit by Angie](https://deluxfitbyangie.com) · [Source](https://github.com/TaylorURL/deluxfitbyangie-com)

A certified personal trainer who sells memberships, online coaching and one-on-one sessions through Stripe, then runs the whole client relationship in the same app. Clients sign in for their plan, their nutrition, their bookings and a message thread with the coach. Angie works the other side of that data and assigns training material to named clients from a private library.

#### [Delux Financial Solutions](https://deluxlavello.com) · [Source](https://github.com/TaylorURL/deluxlavello-com)

A Houston credit-education practice, with every page in English and Spanish. Switching languages fetches nothing and keeps you on the same URL. Each page is plain HTML assembled at build time, so there's no app to boot before the first word appears, and it scores 100 on mobile and desktop.

#### [SETX Football](https://www.setxfootball.org) · [Source](https://github.com/TaylorURL/setxfootball-com)

A youth football camp in Daisetta for kids five to twelve, with no tryouts and no bench. Parents register, order shirts and pay without making an account first, and get three days to fix a mistake, counted down on screen. On camp morning, volunteers verify payments and work the roster from a staff panel, which keeps check-in moving with a line of parents waiting.

#### [Southbelt Repair and Supply](https://southbelt.taylorurl.com) · [Source](https://github.com/TaylorURL/southbeltinc-com)

Concrete batch plants, the parts that keep them running, and the crews that fix them. Each of the eleven machines and every part has its own page. The contact form routes each message to the right desk (quotes, rentals or parts), and every quote button opens an email with the machine's model already in the subject line. It's staged at southbelt.taylorurl.com ahead of its move to southbeltinc.com.

#### [Root & Rise](https://www.rootriseholdings.com) · [Source](https://github.com/TaylorURL/rootriseholdings-com)

A trading desk and the platform it runs on. Its five risk rules are written into the code: the journal refuses a trade that risks more than 1% of the account and locks the day after two losses in a row. Every two minutes a server sweep reads market structure on nine instruments, publishes its calls before the market answers, and scores each one against the bars that follow.

#### [SouthBound](https://southboundofficial.website) · [Source](https://github.com/TaylorURL/southboundofficial-website)

Truck merch: shirts, hoodies, caps and decals, and every order is an entry in the next giveaway. The front page holds the current giveaway, the latest drop, past winners and how entries work.

### Our Own Products

#### [TireTracker](https://www.tiretracker.app)

Service records for commercial tire shops. A technician logs tire positions, DOT codes, tread depths, photos and a signature at the roadside, and the fleet customer reads that history in their own portal instead of calling to ask. The app sends photos through an upload queue, so a tech on weak signal isn't left holding a job open. Next.js, Clerk, Prisma and Neon Postgres.

#### [DomeBreak](https://domebreak.com) · [Source](https://github.com/TaylorURL/domebreak-com)

A real-time missile strategy game played on the actual world map. You pick a nation, put defenses over your cities, build silos, warships, submarines and an orbital tier, and keep a war economy running while missiles are already in the air. It plays in the browser and as a desktop app for macOS, Windows and Linux, with an authoritative match server for multiplayer.

#### [Sunday](https://github.com/TaylorURL/sunday)

A checkpoint that runs before every action a coding agent takes. When an agent reports that the tests pass and a test command failed in the same turn, or says it edited a file it never opened, Sunday stops it and hands back a sentence it has to answer. Written in Go.

### On My Own Time

- [kOS Flight Scripts](https://github.com/bradley-t-t/kos-flight-scripts) are my autopilots for Kerbal Space Program. A booster flies back and lands 0.57 m from its target on a barge, a capsule docks with a station, and landers set down on a chosen spot on the Mun and Duna.
- [Telemetry Ground Station](https://github.com/bradley-t-t/telemetry-ground-station) is mission control for a simulated two-stage rocket, in Java 21 with no runtime dependencies. In one recorded flight, engine 5 failed at T+80 s and the ground flagged it 0.1 s later.
- [CryptoFort](https://github.com/bradley-t-t/cryptofort) is an encrypted credential vault with an MCP server, published on npm. An agent can find the credential it needs without ever holding its value.
- [Viltrum Empire](https://github.com/bradley-t-t/stellaris-vilrumite-empire-mod) is a total-conversion Stellaris mod on the Steam Workshop that brings seven factions from *Invincible* into the galaxy.
- Six Prison Architect mods: [laser fences, and laser doors that open for staff but never for prisoners](https://github.com/bradley-t-t/prison-architect-sci-fi-security), [sci-fi furniture](https://github.com/bradley-t-t/prison-architect-sci-fi-objects) to match, [robot staff](https://github.com/bradley-t-t/prison-architect-robot-staff), a [crematorium](https://github.com/bradley-t-t/prison-architect-crematorium) that turns the hearse away, a [contraband checkpoint](https://github.com/bradley-t-t/prison-architect-contraband-checkpoint-scanner) room that searches anyone who steps in, and a [staffing terminal](https://github.com/bradley-t-t/prison-architect-auto-hire) that hires to the headcount you set.

### Contact

[Start a Project](https://www.taylorurl.com/start) · [trenton@taylorurl.com](mailto:trenton@taylorurl.com) · [taylorurl.com](https://www.taylorurl.com)
