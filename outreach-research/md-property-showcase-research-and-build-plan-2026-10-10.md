# Property showcase: research and build plan

Prepared 10 Oct 2026. Research and planning only. Nothing built, published, sent or signed up for. No agent, photographer or business was contacted.

## 1. The short version

1. **The gap is real but it is not "nobody does editorial".** The Modern House already does editorial listings well. The gap is that every other UK agent, including premium ones, still shows a swipe carousel plus a spec table. At 390px the Modern House page is a hero photo, a title, a paragraph and a "Read more" button. Sotheby's UK is a 12-photo carousel, a details table, a map and boilerplate. Neither is cinematic.
2. **Cinematic scroll templates already exist and are cheap** ($149 source code, free prompts, a licensable theme). So the scene itself is not the moat. The moat is: UK-specific, honest (labelled AI, material information present), built from the agent's own photos, delivered in days, and sold as a pitch asset to win instructions.
3. **Recommended demo: one fictional listing page, not a mini-portal.** Six sections, one signature scene: **day to dusk**, where the scroll relights the same house from daylight to golden hour to blue-hour dusk. I tested the hard part today (section 5): the image tool produced three pixel-aligned keyframes of one house. No video model is needed.
4. **Price to test: GBP 450 standard page, GBP 950 signature page with the dusk scene.** These are hypotheses, anchored to what agents already pay (section 6). A GBP 250 AI landing page exists, so below about GBP 400 you are competing with a commodity.
5. **Best pitch angle:** a listing appointment. Half of vendors see three agents before choosing (Zoopla/YouGov). A bespoke showcase page is something the agent can show a vendor on a phone in the valuation meeting.
6. **Two flags before any real outreach:** who signs contracts and gets paid (section 8), and email rules for sole-trader agents (section 7).

## 2. What happened to yesterday's work

- That repo is **public**. Do not put prospect names, prices you are quoting, or client details in it. Use a private repo.

## 3. Competitor teardown (live, 10 Oct 2026)

I loaded each page at 390px wide with a Samsung-style user agent.

| Site | What it does on a phone | What a solo builder can copy | What not to copy |
|---|---|---|---|
| **The Modern House** (themodernhouse.com) | Centred wordmark, full-bleed hero, serif headlines, swipeable image cards per home, price and tenure on one line each. Listing page: hero photo with "More photos", Floorplan / Map / Brochure tabs, title, price, tenure, two buttons, a pull-quote in italics, one narrative paragraph, a "The Building" collapsible, a black "Interested? Let's talk." block, related sales. | The editorial voice (a quote, then prose about how the house lives), restraint, serif plus clean sans, one phone number and two buttons, generous white space. Their own guide says photos are lit by natural light only and clutter is removed. | Their curation. Founders were editors at World of Interiors and Wallpaper*, and the brand sells only architecturally interesting homes. You cannot copy that taste at volume. Their 12M page views a year claim is self-reported. |
| **Inigo** (inigo.com), Modern House's companion brand for historic homes | Same system, warmer, "Park Life" style editorial headline, Prime and New sections. | A "story first" headline per home. Proves the model extends to period and country houses, which suits a pastoral register. | Nothing special technically. |
| **Sotheby's UK** (sothebysrealty.co.uk) | Swipe gallery "1/12", All photos / Floorplan / EPC tabs, a facts table (type, beds, baths, sq ft, ref), headline, truncated description with "Show more details", map, features icons, disclaimer. | The fact row (but make it nicer), floorplan and EPC as first-class tabs. | The portal feel. This is the "before" in your before and after. |
| **Knight Frank on Foleon** (interactive brochure example) | A magazine-style PDF replacement. | Shows large agents already pay for interactive brochures, so the category has budget. | Heavy publishing platform, not a single-listing experience. |
| **Template market** | Siteglade "Aurelia": WebP frame sequences on a canvas, three acts (arrival, pool, suite), GSAP, Lenis. SmartDuke "Arden" and "Villa Sereno": video and canvas scrub, free prompt, tested source code unlocked for 149 dollars. Mako "Scrollhouse": five chained AI clips scrubbed by scroll, separate 9:16 mobile film, licensable. | The three-act structure and the "media is the product" lesson. | Heavy video scrub on a phone. Aurelia and Scrollhouse both need a lot of frames or large video, which is risky on mobile data. |
| **AI package sellers** (spatialvista.co.uk) | AI listing video from photos, AI staging GBP 25 per room, social reels GBP 45, **single-property landing page GBP 250 first, GBP 80 extra**, copywriting GBP 35. | Their price ladder tells you the floor. | Their product is generic. It sits below what you would sell. |
| **Bespoke agency sites** (Property Wave, Made Simple Media) | Whole-agency websites: GBP 4,995 or GBP 9,995 one-off plus monthly support at Property Wave; GBP 3,000 to 5,000 plus VAT for a bespoke site without feed integration at Made Simple Media. | Shows agents do pay four figures for web work. | A full agency site needs CRM or feed integration. Not your first product. |

Reliability notes: Nakada Design's "20 best luxury real estate websites" is a design agency's marketing blog, so treat its property-page blueprint (strongest true photo first, fact row, 120 to 200 words on how the house lives, ordered media) as one opinion. The same blueprint agrees with what the Modern House actually does, which is why I kept it.


## 4. Demo design direction

### Decision: a single stunning listing page

Not a mini-portal. A portal needs search, data and volume, and it competes with Rightmove. A single page is what an agent buys, can show a vendor and can send to a buyer. If the demo works, a second and third page (different house types) become the portfolio.

### The page, in order (390px first)

1. **Hero.** Full-bleed daylight photograph, no text over the busiest part. Under it: house name, town, guide price, tenure, one line. Two actions: "Request a viewing" and "Floorplan".
2. **Signature scene: day to dusk.** The house sits pinned while the user scrolls about 3 screens. The light changes from morning to golden hour to blue hour, with the windows lighting up. Three short text beats appear on top of the pale or dark panel, not on the photo: "Morning", "Late afternoon", "After dark". It ends on a still of dusk with the CTA.
3. **The house, in a few lines.** A pull-quote and 120 to 150 words on how the house lives, in the Modern House register but original.
4. **Rooms in order.** Exterior, main reception, kitchen, principal bedroom, garden, details. Not shuffled. One caption each.
5. **Floorplan and the facts.** A clean floorplan block plus a fact row: beds, baths, size, tenure, council tax band, EPC rating. These are the legal basics (section 7).
6. **Visit.** Agent name, phone, "Request a viewing". In the demo these are inert and labelled placeholder.

### Apple-sleek and pastoral

Reuse the palette tokens from the 10 Oct local-business brief (same Apple-sleek pastoral register), which carry calculated contrast: warm paper `#F6F3EA`, porcelain `#FFFDF7`, soft sage `#CBD8C0`, deep leaf `#273D32` text, faded sky `#D9E6E6`. Deep leaf on warm paper is 10.52:1 (calculated in that brief). Display type: a serif for house names (Fraunces, SIL OFL), Inter for everything else, both free and licensed for bundling. One small frosted-glass bar at the top, nothing else glassy. A calm editorial tone fits the Modern House register. Apple's polish is a feeling to borrow, not a look to copy.

### The one signature scene, and why this one

Options considered:
- **Arrival flight** (camera moves toward the house): needs an AI video model, large frame sets, and risk of warped architecture. Most template sellers already do it.
- **Door and walk-through**: needs interior consistency across many images. Hard to make honest.
- **Day to dusk** (chosen): same camera, same house, three pixel-aligned keyframes, crossfaded by scroll position. Works on any phone, around 500 to 900 KB of images, no video, no canvas, no library needed. It also matches a real, paid product: photographers charge **GBP 395 to 600 for a twilight pass** (Luxury Property Films GBP 395; We Stream GBP 600 for a 2-hour session). A page that shows dusk without a second shoot has an obvious value story.

How it works technically (plan only):
- Three stacked `<img>` layers inside a sticky container. Scroll progress sets the opacity of layers 2 and 3.
- Chrome and Samsung Internet support `animation-timeline: scroll()` natively (Chrome for Android 115+, Samsung Internet 23+ per caniuse). Use it with a small IntersectionObserver plus `requestAnimationFrame` fallback for older browsers.
- `prefers-reduced-motion`: show the three images as three still frames in a row. No pinning.
- Budget: first screen under 200 KB, whole page under 2.5 MB at 390px, hero and scene images as AVIF/WebP with JPEG fallback.

Stretch scene (only if the first is done early): a "hours of light" strip on the floorplan showing which rooms get morning sun, based on orientation. It is data, not AI, and agents lack it.

## 5. Imagery strategy (no real listing photos)

**Rule:** the demo uses a fictional house and says so. It carries a visible label: "Concept page. Fictional property. Images AI-generated." No real address, no real agent name, no real postcode.


Prompting pattern that worked (for the sender's Gemini or Dreamina):
1. Generate the daylight hero with architecture, lens and "no people, no cars, no text".
2. Edit it twice with "same photograph, identical framing, every architectural detail unchanged. Change only the light to ...". Never regenerate from scratch for the other times of day.
3. Check by flicking between the three at the same size. Reject any that move a window.

Interior and room images: generate each room in its own prompt set and accept that rooms will not match the exterior. For a demo, use a restrained set (kitchen, reception, bedroom, garden) in one consistent style, or abstract details (door handle, stair rail, textile) that do not claim to be rooms of the house.

**When a real agent supplies photos:** the real daylight photo is the hero and stays untouched. The dusk and golden frames are AI "Enhanced Edits". Rightmove's January 2026 technical guidelines (section 10) say AI-generated or manipulated images are allowed only if they do not misrepresent the property, are clearly labelled as AI or otherwise enhanced, and are accompanied by current, accurate images of the room or property. The ASA says it has no AI-specific disclosure rule but applies the normal misleading-advertising rules to the overall impression. So the product has two non-negotiables: a visible label on the scene ("Illustrative lighting, AI-rendered from the agent's photograph") and the real photo shown alongside. Also never touch structure, trees, or neighbours' buildings.

## 6. The business case

### What agents already pay (verified)

| Item | Figure | Source |
|---|---|---|
| Rightmove agency ARPA (average revenue per advertiser) | GBP 1,530 a month (up GBP 90) for 2025 | Rightmove FY25 results presentation, 27 Feb 2026 |
| Standard property photography | GBP 80 to 300; photo plus floorplan about GBP 120 to 220 | Photoplan guide, 24 Jun 2026 |
| Matterport 3D tour | from about GBP 350 to 400 | 360virtualtours.co.uk, trustedphotography.co.uk |
| Listing video tour | GBP 150 to 400 | F9 Media, via We Stream |
| Cinematic property film, London | GBP 1,200 to 2,500 entry; GBP 3,500 to 7,500 luxury home | We Stream price page (15 Sep 2026) |
| Luxury Property Films packages | from GBP 895 (half day), GBP 1,650 (full day), GBP 2,450 (full day plus twilight) | luxurypropertyfilms.com |
| Estate agent commission, London sole agency | about 1.5% plus VAT | Property Tax Partners, Propelr |
| AI landing page for one listing | GBP 250, extra pages GBP 80 | spatialvista.co.uk |
| Single-property sites (US) | builders from about 25 dollars a month; Luxury Presence agent sites start around 500 dollars a month and include 20 single-property sites | theclose.com (Dec 2023, US source, old) |
| Vendors paying for premium marketing | One agent offered paid packages on 117 properties | Agent Response blog (see caveat) |

Caveat on that last row: the blog says 24% (16 vendors) took the premium package and 33% (39 vendors) took the basic. 16 of 117 is 14%, not 24%, and 39 of 117 is 33%. The source is also a vendor of the payment platform. Treat it as a hint that vendor-paid marketing exists, not as a conversion rate.

### Sizing

- About 3% of residential transactions are over GBP 1m (HMRC stamp tax statistics commentary, 2024 to 2025). With about 1.05 million residential transactions that year, that is roughly 31,000 sales, which matches the earlier figure.
- Rightmove says about 1 in 20 homes for sale in Britain is GBP 1m or more (Independent report). AgentWise counts more than 30,000 homes for sale between GBP 1m and GBP 5m across Great Britain (May 2026).
- A GBP 2m sale at 1.5% plus VAT is a GBP 30,000 fee plus VAT, so a GBP 450 to 950 page is about 1.5% to 3% of the fee. That is small, which is the argument, but it also means you are one of many things an agent can cut.

### Price ladder to test (hypotheses, not facts)

| Tier | Price per listing | What it is | Sits between |
|---|---|---|---|
| Pilot | free for 2 to 3 pages | Testimonial and permission to show it | Not applicable |
| Standard page | GBP 450 | Built from the agent's own photos and floorplan, editorial copy, fact row, Floorplan tab, enquiry button. 5 working days. | Above the GBP 250 AI landing page, below a GBP 895 half-day film |
| Signature page | GBP 950 | Standard plus the day-to-dusk scene (AI-labelled) | About the cost of a twilight add-on plus a day of editing |
| Retainer | GBP 390 a month for up to 3 pages | For an agent with a steady flow of prime stock | Under Rightmove ARPA, so it can be absorbed in a marketing line |

Revenue arithmetic, not a forecast: 3 agents at 1 signature page a month is about GBP 2,850 a month. 10 agents at 2 standard pages is about GBP 9,000 a month. The hard part is getting from 0 to 3 paying agents, not the build.

**Biggest commercial risk:** an agent compares you to GBP 250 for a page from an AI tool and to a free template. The answer has to be the finished, labelled, agent-ready package, not the scroll effect.

**Second risk:** agents often do not pay for marketing themselves. In practice the vendor pays on premium listings. So the offer should be a "vendor-paid upgrade" the agent can sell on top of their own fee.

## 7. Pitch angles, ranked

1. **Win the instruction.** "A page like this for your next listing, to show vendors at the valuation." Zoopla's YouGov research of 1,000 recent sellers (5 Aug 2025): 49% see three agents; most important factor is local presence (20%) followed by local reputation (13%). It means the valuation pitch matters. Offer to build one page from the agent's best past sale as a pitch exhibit.
2. **Vendor-paid premium upgrade.** The agent offers it as an extra at GBP 450 to 950, margin to them or to you.
3. **Twilight without a second shoot.** The dusk scene is the demo's best visual. Position it as an alternative to a GBP 395 to 600 twilight session, labelled as AI.
4. **Photographer partnership.** Property photographers work with agents every week and already sell twilight and film. Offer them a white-label showcase page to resell. This was the best warm route in the 9 Oct notes and still looks right.
5. **A sold-stock archive.** A "past sales" collection of showcase pages as a brand asset. Later, not first.

Where to find agents (recheck before use, from the 9 Oct notes): Rightmove, Zoopla and OnTheMarket For Sale at a GBP 1m minimum to see who lists the stock, then the agency's own site. Never pitch through a portal's "email agent" form, which is a buyer enquiry route. Warm routes first.

**Email rules.** ICO: PECR's rule on marketing emails does not apply to "corporate subscribers" (companies, LLPs, Scottish partnerships). **Sole traders and other partnerships are "individual subscribers"** and need consent. Many small independent agencies are partnerships. So check the legal form (Companies House) before any cold email. UK GDPR still applies to named individuals.

**Content rules.** Property listings must carry material information. National Trading Standards guidance (July 2022) lists Part A: council tax band or rate, purchase price and tenure, plus the EPC rating. Parts B and C were still to be announced at the time of that document, so check the current position before the first real page. Do not use "price on application".

## 8. Flags for the sender

- **Who signs and who gets paid.** Before the first paid page, decide who the contracting party is and who receives payment (a personal account, a sole-trader registration or a company). I have not checked this and have not assumed anything about it. It is not a reason to stop the demo.
- **Do not contact anyone yet.** All of section 7 is plan, not action.
- **Source reliability.** One fetched page (propertywebdesignpro.com, on AI-edited photos) carries a publication date of 15 Oct 2026, which is in the future from today's date, so I used only primary sources for the AI rules (Rightmove guidelines, ASA, Propertymark, Guild).

## 9. Build plan (for when the sender says go)

Static HTML, CSS and JS, phone-first at 390px, no framework. Private only. About 5 to 6 hours of build time.

| Step | Output | Check |
|---|---|---|
| 1. Imagery | 1 hero, 2 relit frames, 4 to 6 room or detail images, 1 floorplan drawing (SVG), all labelled fictional | Flick test: no window or chimney shifts between frames |
| 2. Content | Fictional house name and town, pull-quote, 140-word narrative, fact row with fake but plausible values, all marked as placeholder | No real postcode or agent |
| 3. Page shell | Sections 1, 3, 4, 5, 6 | Readable at 320px and 390px, no horizontal scroll |
| 4. Scene | Sticky three-layer day-to-dusk with CSS timeline and fallback | Works at 390px on Chrome and Samsung Internet; reduced-motion shows three stills |
| 5. Polish and checks | Focus rings, contrast, tap targets of 44px, alt text, weight under 2.5 MB | Screenshots at 390px of top, scene start, scene end, facts, visit |

Acceptance additions for this project: visible "Concept page, fictional property" label, scene label "Illustrative lighting, AI-rendered", no stock photo passed off as a real home.

## 10. Decisions for the sender

1. Single listing page as the demo? (Recommended: yes.)
2. Day-to-dusk as the one signature scene? (Recommended: yes. Alternative: an arrival flight, with more risk.)
3. Country or period house (pastoral register, Inigo-like) or a modern architectural house (Modern House-like) for the fictional listing? I tested the former, which suits the palette.
4. Hosting stays undecided. The Cloudflare Pages verdict from this morning stands.
5. Who contracts and gets paid, decided before any paid work.

## 11. Sources

- The Modern House home: https://www.themodernhouse.com/
- Modern House listing (Dorking Road): https://themodernhouse.com/sales-list/dorking-road
- Modern House selling guide: https://themodernhouse.com/guide-selling-your-home
- Modern House photography guide: https://themodernhouse.com/photography-guide
- Modern House, alternative to Rightmove: https://themodernhouse.com/journal/is-the-modern-house-the-perfect-alternative-to-rightmove
- Inigo: https://www.inigo.com/
- Sotheby's UK listing (Radnor Place): https://sothebysrealty.co.uk/properties/buy/townhouse-for-sale-london-bayswater-radnor-place-46375/
- Knight Frank on Foleon: https://www.foleon.com/examples/knight-frank-interactive-real-estate-brochure-example
- Siteglade Aurelia: https://siteglade.com/templates/aurelia
- SmartDuke Arden: https://studio.smartduke.com/templates/arden
- Mako Scrollhouse: https://makoai.studio/work/scrollhouse
- Spatialvista price ladder: https://spatialvista.co.uk/
- Property Wave pricing: https://propertywave.co.uk/pricing
- Made Simple Media costs: https://www.madesimplemedia.co.uk/property-website-design/cost
- Nakada Design luxury sites: https://nakadadesign.com/stories/20-best-luxury-real-estate-websites-2026
- Rightmove FY25 results presentation: https://plc.rightmove.co.uk/content/uploads/2026/02/260227-FY25-Presentation.pdf
- The Negotiator on Rightmove ARPA: https://thenegotiator.co.uk/news/marketing-news/rightmove-revenue-up-9-as-agent-spending-rises/
- Rightmove technical guidelines, Jan 2026: https://media.rightmove.co.uk/pdf/rightmove_technical_guidelines.pdf
- ASA on AI disclosure: https://www.asa.org.uk/news/disclosure-of-ai-in-advertising-striking-the-balance-between-creativity-and-responsibility.html
- Photoplan photography prices: https://www.photoplan.co.uk/guides/how-much-does-property-photography-cost
- We Stream property video prices: https://westream.uk/real-estate-prices
- Luxury Property Films packages: https://luxurypropertyfilms.com/
- Zoopla and YouGov on how sellers choose agents: https://www.zoopla.co.uk/press/releases/zoopla-identifies-whats-really-driving-how-sellers-choose-agents-in-2025-and/
- Agent Response vendor-paid marketing: https://blog.agentresponse.co.uk/vendors-are-willing-to-pay-for-premium-marketing-a-case-study/
- HMRC stamp tax statistics commentary: https://www.gov.uk/government/statistics/uk-stamp-tax-statistics/uk-stamp-tax-statistics-2023-to-2024-commentary
- National Trading Standards material information guidance (July 2022): https://www.nationaltradingstandards.uk/uploads/Industry%20guidance%20for%20material%20information%20on%20property%20listings%20-%20July%202022.pdf
- ICO on business-to-business marketing: https://ico.org.uk/for-organisations/direct-marketing-and-privacy-and-electronic-communications/business-to-business-marketing/
- Chrome scroll-driven animations: https://developer.chrome.com/docs/css-ui/scroll-driven-animations
- caniuse scroll-driven animations: https://caniuse.com/wf-scroll-driven-animations
- CSS-Tricks on Apple-style frame scroll: https://css-tricks.com/lets-make-one-of-those-fancy-scrolling-animations-used-on-apple-product-pages/

## 12. Direction update, 10 Oct 10:42: desktop-first

the sender's decision: the demo is desktop-first. The day-to-dusk scene is designed for desktop viewing. Mobile gets a lighter cut (stills or a short clip). This supersedes the phone-first and 390px-first wording in sections 4, 5 and 9. Still research and planning only; nothing built.

**What changes**

| Area | Was | Now |
|---|---|---|
| Primary viewport | 390px phone | 1440 x 900 desktop, checked also at 1920 x 1080 and a 1280 x 720 laptop |
| Scene frames | 4:5 | 16:9 wide frames (2K source), served as AVIF/WebP at about 1600 to 2000px wide |
| Scene layout | Pinned image with text beats over a panel | Full-viewport sticky scene, about 300vh of scroll. Text beats ("Morning", "Late afternoon", "After dark") sit in a calm side column on a porcelain panel, not over the busiest part of the photo. A small frosted-glass fact chip (guide price, tenure) can sit over the sky |
| Mobile | Same scene pinned | Lighter cut: a swipeable strip of the same three frames with captions, no pinning. Optional short muted clip (6 to 8 seconds, lazy-loaded) only after the stills work. Respect `prefers-reduced-motion` and Save-Data where the browser reports it |
| Weight budget | Under 2.5 MB at 390px | Desktop page under about 4 MB, scene frames about 300 to 450 KB each. Mobile under 2.5 MB because it loads the smaller crops |
| Phone-first rule | Core rule | Mobile must still be clean and fast, but it is a lighter cut, not the design target |

**Why desktop-first suits the business.** Agents and vendors will often view the page on a laptop in a valuation meeting or an office, and a wide 16:9 relight reads far better than a portrait crop. Scroll-scrubbed property templates (Siteglade Aurelia, Mako Scrollhouse) are also designed for desktop first, and Mako composes separate desktop 16:9 and mobile 9:16 films rather than cropping one.


**Mobile crops.** Do not crop the 16:9 frame to 4:5. The house sits right of centre, so a centre crop would cut it. Generate or edit a separate 4:5 daylight frame, then relight that, as done in the first test. For a real client photo this means two crops from the original, with a note to the photographer.


**Updated build steps** (replaces the table in section 9, about 6 to 7 hours)

| Step | Output | Check |
|---|---|---|
| 1. Imagery | 16:9 day frame plus two relit frames, 3 matching 4:5 frames for mobile, 4 to 6 room or detail images, an SVG floorplan, all labelled fictional | Flick test at 1920 wide: no window or chimney shifts between frames |
| 2. Content | Same as section 9 | No real postcode or agent |
| 3. Desktop shell | Sections 1, 3, 4, 5, 6 at 1440 | No horizontal scroll at 1280, 1440, 1920 |
| 4. Desktop scene | Sticky three-layer scene, CSS scroll timeline with a JS fallback, text beats in the side column | Smooth at 60 fps on a mid laptop; reduced-motion shows three stills |
| 5. Mobile cut | Swipe strip of stills with captions; optional short clip | Works at 390px and 320px; under 2.5 MB |
| 6. Review pack | Desktop screenshots, scroll-through MP4, 390px screenshots | Visual check of every frame before delivery |

Acceptance additions stay as before: visible "Concept page, fictional property" label; scene label "Illustrative lighting, AI-rendered"; no real listing photos.

**Open question for the sender (small).** For the lighter mobile cut, stills first (my recommendation) or a short clip? A clip adds weight and one more thing to keep honest and aligned.

## 13. Feasibility: how an agent would use it, whether it helps sell, the pipeline, the viewing request (10 Oct, 11:05)

Research only. Nothing built, no contact with any agent. "Evidence" means a source I read this session. "Hypothesis" means my reasoning, not tested. Several figures come from vendors or portals selling something, so treat them as directional.

### 13.1 Short answer

- The page cannot sit inside the portal listing. It is a link the agent adds, so its job is to win clicks from the portal, social, email and the valuation table, and to turn them into a viewing request.
- The honest mechanism is attention, trust and fewer wasted viewings. It is not magic. No source I found proves a cinematic page raises sale price. The best evidence is that richer listings (more photos, floorplan, video) get more leads.
- Most likely buyer of the service: the agent for a £1m+ home, at the instruction stage (to win the instruction), and for the 1-2 listings a month where the vendor expects something special.

### 13.2 Where an agent would use a single-property page (day to day)

| Use | How it works | Status |
|---|---|---|
| Portal listing | Add the page as a link under Rightmove "Additional media". YouTube/Vimeo play inside the listing. Any other link shows as a separate pop-up window. Feed users add it through the data feed. Rightmove sales guide: videos and tours sit in the 4th slot of the carousel. | Evidence (Rightmove FAQ, Rightmove Hub guide) |
| Listing launch | Send to the agent's own applicant list and register of buyers on day one. Zoopla data (2019, via an agent blog): most leads arrive in the first 6 minutes the listing is live, about a third of sales leads in week one. So the page must be ready at launch, not a week later. | Evidence, but secondary and 2019 |
| Social | Paid or organic Instagram/Facebook posts of the day-to-dusk scene as a clip, linking to the page. Agents already buy ad-ready visuals for this (spatialvista sells it). | Evidence that the market exists. Effect on this service: hypothesis |
| Email alerts / mailers | Link in the agent's own applicant emails and the "just launched" email. The portal's own alerts show only the photos, not the page. | Hypothesis on click rates |
| Valuation / pitch leave-behind | A fictional or past-sale page shown on the valuer's tablet or sent after the appointment. Vendors usually see 2-3 agents, so this is where a premium agent can look different. | Evidence on the process (QuiteRight, Rightmove "Winning Instructions" guide). The page as differentiator: hypothesis |
| Window screen / QR / brochure | QR on the window card, a screen playing the dusk clip, QR on the printed brochure. | Hypothesis, low cost to try |
| Overseas / remote buyers | Send to buyers abroad who cannot view quickly. | Evidence of demand: 22% of 2020 prime central London acquisitions were by overseas buyers who had not viewed (LCP, via The National). Page effect: hypothesis |

Rightmove also lets agents offer "Online Viewings": an orange label, a lead notification when a buyer wants one, and a video sent by email with tracking. This works only through Rightmove Plus, not through data feeds. Our page is an alternative or a companion to the video, not a replacement.

### 13.3 How it helps sell the house: evidence vs hypothesis

Evidence (what the sources say):
1. More photos, more leads. Rightmove sales guide (2022): branches that add 5+ photos get 11% more leads on average. Floorplans: 12% more leads. Videos: 8% more views and 6% more leads (2022). An earlier 2020 edition said 36% and 31%, so the figures vary by year. Top 5% of agents get 55% more leads per property.
2. Only the first photo shows in mobile search. Over 70% of Rightmove traffic is on mobile (2021).
3. Buyers read the photo count and click on it. Image Foundry / Lancaster University eye-tracking study (2021, a CGI vendor with a stake): buyers want at least 8 images, most look at about 8, and day, night, lived-in and pristine views appeal to different people. Night-time shots fill a gap in what buyers see.
4. Viewings are short. Zoopla eye-tracking (Aug 2024): a fifth of buyers spend under 20 minutes viewing before making an offer, and about 34 seconds in a bedroom. First impressions carry weight.
5. Richer listings sit at higher asking prices (Benham and Reeves, Feb 2026): 5+ photos, average £280k, versus 4 or fewer, £200k. This is correlation only. Cheaper homes are probably marketed more thinly.
6. Video helps remote and overseas buyers cut wasted trips (Property Investor Today, June 2026, a trade blog).

Hypothesis (no direct evidence found):
- A scroll page lifts click-through from the portal. No source measures this.
- Day-to-dusk lifts viewings or the price. Photographers sell twilight shots at £395-600 and open-homes.com argues it helps hard-to-sell homes, but I found no controlled study.
- A page makes vendors choose the agent. This is the pitch angle, and it needs testing with real agents.

Mechanism, stated plainly (hypothesis built on the evidence above):
1. It adds more variety than 8 photos can, including the evening and the grounds, so a buyer who cannot get to the house forms a view faster.
2. It sets the tone for a £1m+ home before the first call.
3. It screens: a buyer who has watched the whole scene and still asks is warmer, so fewer tyre-kickers reach the viewing.
4. For the vendor it shows effort. That wins instructions, which is where the money is.

What it will not do: fix a wrong asking price. Rightmove's own guide says that if presentation is right and detail views are still low, look at the price.

### 13.4 Pipeline: yes to live page

What the agent supplies (all agents already hold most of this for the portal):
- Photos: the photographer's final set. Our service must not use portal photos without the photographer's licence and the vendor's consent (copyright sits with the photographer unless assigned). Check this per job.
- Floorplan and EPC. An EPC must be commissioned before marketing starts, valid for 10 years (GOV.UK guide).
- Copy: the description, key features and the material information (council tax band, price, tenure; type, build, rooms, utilities, parking; flood risk and covenants where they apply, per the National Trading Standards guidance). We use their text and must not invent facts.
- Vendor approval of the page, in writing, as with brochure proofs. Instruction paperwork and AML checks come first, so the page can only start after the instruction is signed (AvaroAI, UK pre-marketing gate).
- Any AI or generated imagery must be labelled, with a real photo beside it, if it appears on the portal (Rightmove guidelines, covered in section 7).

Typical timeline (hypothesis built from three data points: agent web builders advertise "live in 5-12 days" and "live in 7 days" for a whole site, and one agent runs a 14-day instruction-to-open-house plan):
| Day | Step | Owner |
|---|---|---|
| 0 | Instruction signed, AML started | Agent |
| 1-3 | Photographer, floorplan and EPC booked and done | Agent |
| 3 | Assets handed over (a shared folder) | Agent |
| 3-5 | Page built from template, vendor copy and photos | Us |
| 5-6 | Agent and vendor proof, one round of changes | Agent and vendor |
| 6-7 | Live, link added to portal, social and mailer ready | Agent |

Target to test: first draft within 48 hours of assets, live within 5 working days. Because the first hours of a listing matter, the page should be ready on launch day. The service therefore works best if the agent books us at the valuation, not after.

What can go wrong:
- Late or missing assets (the most likely delay).
- Vendor not signed up or not agreeing to the page.
- Photo licence unclear.
- Material information missing, which exposes the agent under the Consumer Protection Regulations.
- Generated twilight images that mislead (a different house colour, extra features). The label and the real day photo need to stay.
- Price change or withdrawal after the page is live: the page must be updated or taken down quickly. Stale pages are a risk for the agent.
- The portal pop-up and a mobile link may be missed, so the page must also be promoted off-portal.
- Hosting and speed on a phone (see the mobile note in section 12).
- Who is the contracting party for the page: the agency, not the vendor. A sole trader contact needs PECR care in cold outreach (section 7).

### 13.5 Converting interest into a viewing request

Design (hypothesis, to test in the demo):
- One clear action all the way down: "Request a viewing", pinned in the header and repeated at the end of the day-to-dusk scene, after the floorplan and after the key facts.
- Price, tenure, council tax, EPC and floorplan on the page, so the buyer is qualified before they ask (this is also the material information).
- Add UTM tags per channel (portal, email, social, QR) so the agent sees where requests came from.
- Where the page forwards to Rightmove or Zoopla: the portal's own lead tracking will not see page-only requests. Agents need to log them in their CRM, otherwise their portal stats look worse. This is a real objection to plan for in the pitch.
- Data: the page collects personal data, so a privacy notice and the agent as data controller are needed.

What to measure for the first real pilot (not yet run): page views from each channel, % who reach the form, requests per 100 views, viewings booked, and offers. Compare with the same agent's listings of similar value without a page. Do not promise a lift to agents until a pilot has data.

### 13.6 Things I could not confirm

- Any independent number for conversion from a bespoke single-property page in the UK. None found.
- Real UK turnaround for premium agent microsites. I found only general web design claims.
- Whether Rightmove shows the page link prominently on the mobile app. The FAQ says pop-up window for non-YouTube/Vimeo links.
- Sources that are vendors or blogs (Image Foundry, QuiteRight, Roomagen, Seven Keys) have a commercial interest or are second-hand.

### 13.7 Sources for section 13
- Rightmove, Create the Ultimate Sales Listing (2022): https://hub.rightmove.co.uk/content/uploads/2022/04/Sales_Ultimate-Listing_2022.pdf
- Rightmove, earlier edition (2020): https://hub.rightmove.co.uk/content/uploads/2020/11/Create-the-Ultimate-Sales-Listing.pdf
- Rightmove FAQ, how to add a virtual tour: https://customerfaq.rightmove.co.uk/support/solutions/articles/7000056349-how-do-i-add-a-virtual-tour-
- Rightmove FAQ, online viewings: https://customerfaq.rightmove.co.uk/support/solutions/articles/7000057371-tell-me-more-about-online-viewings
- Zoopla eye-tracking press release (8 Aug 2024): https://www.zoopla.co.uk/press/releases/zoopla-trials-cutting-edge-eye-tracking-technology-to-reveal-what-british/
- Image Foundry / Lancaster University study: https://www.imagefoundry.co.uk/insights/research-what-images-work-best-for-marketing-properties/
- Seven Keys, citing Zoopla first-hour data (2019): https://sevenkeys.co.uk/revealed-the-first-hour-on-rightmove-and-zoopla-is-the-fastest-for-property-leads/
- Estate Agent Today, Benham and Reeves photo count (Feb 2026): https://www.estateagenttoday.co.uk/breaking-news/2026/02/revealed-how-many-photos-a-property-listing-needs-to-boost-the-sale-price/
- National Trading Standards, material information guidance: https://www.nationaltradingstandards.uk/news/full-material-information-guidance-published/
- GOV.UK, EPC guide for marketing: https://www.gov.uk/government/publications/energy-performance-certificates-for-the-construction-sale-and-let-of-dwellings/a-guide-to-energy-performance-certificates-for-the-marketing-sale-and-let-of-dwellings
- AvaroAI, UK instruction and AML gate (May 2026): https://avaroai.com/blog/before-uk-instruction-becomes-listing
- Property Investor Today, overseas buyers (June 2026): https://www.propertyinvestortoday.co.uk/article/2026/06/why-overseas-property-buyers-need-more-than-pretty-listing-photos/
- The National, sight-unseen prime London purchases (Nov 2020): https://www.thenationalnews.com/business/property/over-a-fifth-of-prime-central-london-homes-bought-sight-unseen-by-overseas-buyers-1.1105115
- QuiteRight, market appraisal presentation: https://www.quiteright.co.uk/guides/market-appraisal-presentation
- Rightmove Hub, Winning Instructions guide: https://hub.rightmove.co.uk/content/uploads/2018/10/Winning-Instructions-Exceptional-Agents-Guide.pdf

## 14. Service workflow, deepening section 13 (10 Oct, 14:30)

Research and planning only. No build, no prospect contact. Labels: E = evidence from a source I read, H = hypothesis. Nothing here is a promise of results to any agent.

### 14.1 The workflow in seven steps

| # | Step | What happens | Who decides | Status |
|---|---|---|---|---|
| 1 | Listing-media permission | Before we touch any listing image, the agent confirms in writing that they hold the right to use it for this purpose, and the vendor agrees to the page. | Agent (and vendor) | E for the rule, H for our wording |
| 2 | Supplied accurate property facts | The agent sends the facts. We do not research or invent them. | Agent | E |
| 3 | Fictional demo first | The agent sees a fictional-house demo before any real property is used. | Us, then agent | Our plan |
| 4 | Review | We build the real page from the agent's assets. Agent and vendor check every fact and image. | Agent, vendor | H |
| 5 | Agent-approved publication | Nothing goes live until the agent approves in writing. The agent adds the link themselves, or approves us doing it. | Agent | E for the portal rules |
| 6 | Viewing enquiry | A visitor requests a viewing. It goes to the agent, who owns the lead. | Agent | H |
| 7 | Measurement | Page views, form starts, requests per 100 views, viewings booked, by channel. | Agent and us | H, not yet run |

### 14.2 Step 1: listing-media permission (evidence)
- Copyright in a photograph, video, floorplan and written description belongs to its creator from the moment it is made, and others need permission to use it (Copyright, Designs and Patents Act 1988, summarised by a photographer's guide aimed at agents: through-the-lens.co.uk). E, secondary source.
- Photographers' own terms show the usual deal: copyright stays with the photographer, the client gets a limited licence for set uses (for example propertyphotoguy.co.uk terms, clause 3 and the licence definition). Whether a licence covers a third-party page is not clear from these, so we must ask. E for the usual pattern, H for any single job.
- Rightmove makes the agent responsible. Its Technical Guidelines (Jan 2026), section 10, say the agent warrants it has "all necessary permissions to use such images and videos (including but not limited to the copyright in such images and videos)", and that images are only of the property, the immediate locale and not misleading. Rightmove's FAQ also says agents are responsible for photo permissions and Rightmove is not a regulator. E, primary sources.
- Practical rule for us: the agent sends the photographer's licence terms or a short written confirmation that the licence covers use on a showcase page. No confirmation, no real photos. A photo that shows a living person cannot go in a Rightmove sales advert (guidelines, section 10), so the same caution applies to the page. E for the portal rule, H for applying it to the page.
- Hypothesis to test with an agent: a one-line consent clause in our agreement ("agent confirms rights to supplied media and vendor consent"), so the responsibility is clear and stays with the agent.

### 14.3 Step 2: supplied accurate property facts (evidence)
- The agent is already bound by UK consumer law not to mislead or omit material information. The Digital Markets, Competition and Consumers Act 2024 replaced the old CPRs on 6 April 2025, per a vendor blog (miravely.com, secondary). The statute is at legislation.gov.uk (sections 225 and 227: unfair practices and misleading omissions). The CMA guidance is CMA207 (Nov 2025). I read the section headings, not the full law. E for the existence, H for how a regulator would treat a showcase page.
- National Trading Standards guidance sets the list: Part A (price, tenure, council tax), Part B (type, construction, rooms, utilities, parking) and Part C (flood risk, covenants and similar, only if relevant). E.
- Our rule: we only publish facts the agent supplied, and we mirror the agent's own portal listing for price, tenure and council tax. The agent signs a fact sheet. We never fill a gap ourselves. H.
- Generated or altered imagery: Rightmove's own Technical Guidelines (Jan 2026), section 10, say enhanced edits that could be taken as authentic must be "accompanied by current, accurate images of the room and/or property" and "clearly labelled as being AI or otherwise enhanced". I checked this in Rightmove's PDF itself, not only in a third-party blog. The guidelines also say images "must not contain text", so on the portal the label goes in the caption. E. Our day-to-dusk scenes are edits of the real exterior, so on the page they carry a visible "Evening view: digitally created" label, with the real daytime photo shown. For anything pushed to a portal, follow the caption rule. H for our label wording.

### 14.4 Step 3: fictional demo first
- The demo uses a fictional house with generated imagery only, labelled as fictional. It is shown privately to agents only after the sender decides to approach anyone, which has not happened. No real listing, address or photo is used. Our plan.
- The demo lets an agent judge the format without us holding any of their data or media. H.

### 14.5 Steps 4 and 5: review and agent-approved publication
- Two review gates: (a) fact sheet matched against the page, line by line, (b) image check: licence confirmed, labels present, no living people, nothing altered beyond the labelled edits. H, modelled on how brochure proofs work.
- Publication is the agent's decision. They approve the live URL in writing, then add it to the portal themselves under "Additional media" (Rightmove Plus) or through their feed (E, Rightmove FAQ). Rightmove's guidelines (section 11) also govern online viewings, virtual tours and videos. I read only the heading of section 11. Read it fully before any pilot.
- Take-down: the agent can ask us to take the page down at once, for a price change, withdrawal or sale. Target: same working day. H.
- Data: the page's enquiry form collects personal data. The agent is the controller and the form needs a privacy notice (ICO consent and PECR guidance). We act as their processor, so a written processor agreement is needed before any pilot. Sources: ico.org.uk consent guide and PECR guide. E for the principle, H for the exact set-up, and it needs a legal check.

### 14.6 Step 6: the viewing enquiry

### 14.7 Step 7: measurement
- Per page: views by channel, scroll-through rate of the day-to-dusk scene, form starts, requests per 100 views, viewings booked, offers. H.
- Honest comparison: the same agent's similar-value listings with no page. One agent and a few listings will not prove anything, so call it a pilot, not a result.
- Do not quote the Rightmove averages (13.3) as the page's effect. They describe photos, floorplans and videos, not our format.

### 14.8 Mobile direction: stills vs short clip (both, with evidence)

| | Stills (swipe strip of 4:5 frames) | Short clip (6-8s) |
|---|---|---|
| Evidence for | NAR 2025 survey (US buyers, 5,390 responses): 83% rated listing photos "very useful", 41% virtual tours, 29% videos. Rightmove: over 70% of its traffic is mobile and only the first photo shows in search (2021). The Image Foundry eye-tracking study (2021, CGI vendor) found most buyers look at about 8 images and like day and night variety, which stills deliver. Light on data, so it suits the sender's phone, where heavy sites don't load. | Rightmove's 2022 sales guide: listings with video average 8% more views and 6% more leads (2020 edition: 36% and 31%). Chrome on Android supports muted autoplay, so a short clip can run without a tap (Chrome for Developers). Clips fit social feeds, where the Machina analysis says video competes. Trade blog (PIT, 2026): video helps remote and overseas buyers cut wasted trips. |
| Evidence against | Static frames lose the day-to-dusk motion that is the point of the scene. No study isolates the effect of a stills sequence. | Machina (2026) notes no study isolates a linear listing video's effect, and the big studies measured navigable virtual tours. The "403%" claim attributed to NAR cannot be traced. A US NBER paper found about a 1% price effect from virtual tours, shrinking after COVID. Video adds page weight and slow loads (web.dev video performance guide: use a poster image, compress, and avoid heavy autoplay). A 2017 Medium post claimed 87% click-play on Zoopla versus 12.5% on Rightmove. That is one person's observation, not a study. |
| Cost to build | Lowest. Frames already exist from the relight test. | More work: export, compress, poster frame, test on a mid-range Android phone. |
| Main risk | Looks flat next to rivals who use video. | Slow or failing playback on a weak phone, and data use. |

What this means: the evidence supports neither as proven. Stills are the safer fit for page speed and the slow-phone constraint. A clip has the better case for social and overseas buyers. The decision stays with the sender. If he wants data, test both: build the strip first, add a clip as a variant, and compare scroll depth and form starts in the pilot. Most of this evidence is US survey data or vendor content, so read the table as direction only.

### 14.9 Not confirmed
- UK-specific proof that a showcase page, stills or clip moves viewings or offers.
- Whether a photographer's standard licence covers a third-party page. Needs asking per job.
- Whether Rightmove treats the day-to-dusk edits as "Enhanced Edits" on the page, which is not a portal listing. I applied the stricter rule to be safe.
- The full text of Rightmove guidelines section 11.
- Legal advice: the DMCC, copyright and data-protection points need a solicitor's check before any paid work.

### 14.10 Sources for section 14
- Rightmove Technical Guidelines, Jan 2026 (sections 10 and 11): https://media.rightmove.co.uk/pdf/rightmove_technical_guidelines.pdf
- Rightmove FAQ, another agent using my images: https://customerfaq.rightmove.co.uk/support/solutions/articles/7000083606-another-agent-is-using-my-images-on-their-rightmove-listing
- Copyright guide for estate agents (photographer): https://www.through-the-lens.co.uk/blog/copyrightestateagents
- Photographer terms, example: https://propertyphotoguy.co.uk/terms
- Miravely, DMCC and AI photos (secondary): https://miravely.com/blog/uk-dmcc-act-digitally-altered-listing-photos
- DMCC Act 2024, s.225: https://www.legislation.gov.uk/ukpga/2024/13/section/225/enacted
- DMCC Act 2024, s.227: https://www.legislation.gov.uk/ukpga/2024/13/section/227/enacted
- CMA207 guidance, Nov 2025: https://assets.publishing.service.gov.uk/media/691b9bd821ef5aaa6543ee6f/Unfair%5Fcommercial%5Fpractices%5FCMA207%5F18%5FNov%5F2025%5F%5F2%5F.pdf
- National Trading Standards material information: https://www.nationaltradingstandards.uk/news/full-material-information-guidance-published/
- ICO consent guide: https://ico.org.uk/for-organisations/uk-gdpr-guidance-and-resources/lawful-basis/a-guide-to-lawful-basis/consent/
- ICO PECR guide: https://ico.org.uk/for-organisations/direct-marketing-and-privacy-and-electronic-communications/guide-to-pecr/electronic-and-telephone-marketing/
- Machina, listing video vs photography (cites NAR 2025 and NBER 33204): https://wearemachina.com/insights/listing-video-vs-photography
- web.dev video performance: https://web.dev/learn/performance/video-performance
- Chrome for Developers, muted autoplay on mobile: https://developer.chrome.com/blog/autoplay-2
- Rightmove sales guide 2022: https://hub.rightmove.co.uk/content/uploads/2022/04/Sales_Ultimate-Listing_2022.pdf
- Image Foundry study: https://www.imagefoundry.co.uk/insights/research-what-images-work-best-for-marketing-properties/
- Property Investor Today, overseas buyers: https://www.propertyinvestortoday.co.uk/article/2026/06/why-overseas-property-buyers-need-more-than-pretty-listing-photos/
- Medium, Rightmove video views (2017, anecdotal): https://medium.com/@alextench/rightmove-missing-out-on-millions-of-video-views-12fd304678b5

