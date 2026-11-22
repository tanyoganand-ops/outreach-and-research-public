# Dare UGC format sweep — format cards (v3, 2026-11-18)

## Scope and method

Goal: find existing short-form videos matching three "make money with AI video" formats that promote the Dare app (trydare.com), for studying on-screen visuals and captions. Formats 1 and 2 are Dare-specific; Format 3 allows any AI tool, not only Dare.

- Collection used public, logged-out pages and direct cookieless fetches of public files. During collection, some account-access mistakes occurred on shared routes; these were separately disclosed and the affected routes were stopped.
- Verification standard: a mechanic is called verified only where frames of the downloaded file were inspected ("frames-inspected" in videos.csv). Captions and search listings are treated as leads ("source-caption-only"), not proof. Where frames contradicted a source description, the row says so.
- The brief's specific scripts (quoted below as "reported brief") were the match bar. Generic Dare promotion, generic AI-money funnels, and same-tool-different-mechanic videos are labeled adjacent, never matches.
- Earnings figures spoken or shown in these videos are unverified creator claims.
- Downloads are reference-only; no repost rights.

## Format 1 — "deleting this in 24 hours" AI colouring-book / KDP gatekeeping hook

Reported brief (not found): a creator says the video will be deleted in 24 hours, then shows an AI colouring-book / Amazon KDP workflow, with Dare as the tool.

- Exact matches found: 0.
- Candidate pool: 58 keyword-search leads. Verification levels: 1 viewed in full (adjacent; different tool, no Dare), 6 checked via stills/descriptions (adjacent at best), 51 keyword-only and uninspected. No inspected lead showed a Dare-branded instance; the 51 uninspected leads are unknowns.
- Status: unverified whether this format exists for Dare in public content. TikTok/Instagram search require login and were out of scope.

## Format 2 — paste a viral video link into Dare (GTA 6 hook)

Reported brief (not found): "GTA 6 videos are blowing up" hook; creator pastes a link to a viral video into Dare; Dare regenerates it.

- Exact matches found: 0. No inspected video shows a viral-video link pasted into Dare, and no GTA 6 hook appeared in inspected Dare content.
- Verified adjacent mechanics (frames-inspected, Dare UI visible on-screen):
  1. Prompt-to-video funnel: hook cites daily earnings from YouTube Shorts, creator types a prompt (often drafted in Claude), pastes it into Dare, shows the generated video. Top example: https://www.tiktok.com/@jakedevelops/video/7690710309647977749 (441.5K views). Also https://www.tiktok.com/@jakedevelops/video/7690710119125880084.
  2. Viral kids-channel screenshot + prompt: creator opens a popular kids YouTube channel, screenshots it, pastes the screenshot plus a prompt (via Claude) into Dare, generates similar content, "Comment LINK" funnel. Four verified examples: https://www.tiktok.com/@jakedevelops/video/7681170191111441685, https://www.tiktok.com/@jakedevelops/video/7685561224926448916, https://www.tiktok.com/@jakedevelops/video/7682595636700613909, and https://www.tiktok.com/@gabe.buildss/video/7706983878992350495.
  3. Paste a product-website URL into Dare to generate a UGC ad: https://www.tiktok.com/@jakedevelops/video/7681130126041484565. Closest verified relative of the requested paste-a-link mechanic, but the pasted link is a product site, not a viral video.
- Counts: 7 frames-inspected F2-family videos. Further Dare-family videos with other mechanics are in the CSV; unverified rows are marked source-caption-only.

## Format 3 — Google Maps roulette blind-click + AI assets + cold call

Reported brief (not found): creator blind-clicks a random business on Google Maps, reacts to its bad photos, generates AI assets, then cold-calls the business. The request allows any AI tool here, not only Dare.

- Exact matches found: 0. No inspected candidate combined blind pick + AI asset generation + cold call, and no inspected candidate in this genre showed Dare branding.
- Frames-inspected candidates (downloaded cookieless and verified):
  1. https://www.instagram.com/reel/Dd34t9PGQGp/ (@scalingwithalex): "grab a real business off Google Maps"; Claude + CodeWords build a WhatsApp agent for the business; comment-AGENT funnel. Verified Maps pick + AI + funnel; the asset is a chat agent, not visuals; no cold call on-screen.
  2. https://www.instagram.com/reel/DfiJn_TtBlq/ (@angus.sewell, 1,693 likes / 657 comments): "How to cash a dead starbucks" — Google Places data on closed businesses, Claude-built geofenced ad proposal ($600 setup / $350 per month shown), email outreach, comment-"map" funnel. Verified; no blind pick, no cold call.
  3. https://www.tiktok.com/@valeridoesai/video/7699896656136998146: "Claude killed cold outreach" — Maps businesses with dated websites, Claude builds a live preview site, outreach via contact form/email/DM. Verified; no cold call.
  4. https://www.instagram.com/reel/DfhvlxmN_Wv/ (@angus.sewell): Maps pins + AI chat "Flag closed businesses" with spreadsheet export + email-the-owner outreach. Verified; no cold call.
  5. https://www.instagram.com/reel/De_0lfWkixP/ (@thesiteaudit.uk): "Google Maps Roulette - roofers in leeds" — spin-the-map lands on a roofer, automated DOM site audit (score 41/100, 3 bugs), comment-"AUDIT" funnel. Closest to the roulette mechanic; audit replaces AI assets and the funnel replaces the cold call.
  6. https://www.instagram.com/reel/DWyq-2xjscJ/: "Stop scrolling if you're still sending generic cold emails" — Maps lead scrape into AI-written personalized emails (mapileads.com). Verified.
  7. https://www.instagram.com/reel/DekIH7VCQ36/ (@jarvis_daily_ai): "Claude + Google Maps can find you clients" carousel — target old sites from Maps, Claude rebuilds from template, finds the contact form, sends the message; comment-"JARVIS" funnel. Verified.
  8. https://www.instagram.com/reel/DeGUpovSLpe/: Maps business search + AI receptionist pitch with a revenue-leak report ("$15,000/mo" figure is an unverified creator claim). Verified.
  9. https://www.instagram.com/reel/DdIBVdnBuLb/: Maps "Houston roofing" search + Coderick AI "Rebuild from URL" + website-checklist outreach. Verified.
  10. https://www.instagram.com/reel/DeptPL2iht7/ (@WealthFlowDaily): "The 20-Minute Google Maps AI Audit ($150 Client Hustle)" carousel — Maps target, ChatGPT audit of the listing, Canva package, comment-"AUDIT" funnel. Price figure is an unverified creator claim. Verified mechanic.
  11. https://www.instagram.com/reel/DfP0L20Fmg8/: "Claude + Google Maps = an automated client pipeline" carousel — Claude scouts Maps, flags outdated site, rebuilds from template, locates contact form, sends personalized outreach; comment-"MAKEOVER" funnel. Verified.
- Inspected and rejected (no Maps+AI mechanic in frames, kept in the CSV labeled off-format): Dd0mrhhz8aV (website-sales talking head), DfD_4ehO0o0 (freelancer outreach skit), DfqoCHeMFxL (cold-call comedy clip).
- Source-listing candidates not frame-verified (7 rows left in videos.csv): 6 YouTube videos are behind a sign-in bot check for cookieless download, 1 Instagram post (DfcL4OYEaDm) is image-only. These remain unknowns.
- Two source-listed TikTok IDs were downloaded and did not contain the described Maps content (https://www.tiktok.com/@theaiimpact/video/7655157230508985621 is a prompt-loop tutorial; https://www.tiktok.com/@theaiimpact/video/7563650763340188949 is a ChatGPT ad-creative tutorial). They are kept in the CSV labeled as mismatches.
- Whether the exact blind-pick-plus-cold-call variant exists behind logged-in TikTok/Instagram search is unknown; those searches were out of scope.

## Top adjacent references (not exact matches)

1. https://www.tiktok.com/@jakedevelops/video/7690710309647977749 — prompt-to-video funnel, 441.5K views (F2-family)
2. https://www.tiktok.com/@jakedevelops/video/7681170191111441685 — kids-channel screenshot + prompt (F2-family)
3. https://www.instagram.com/reel/Dd34t9PGQGp/ — Maps pick + AI agent build (F3-family)
4. https://www.instagram.com/reel/DfiJn_TtBlq/ — Maps data + AI + outreach, 1,693 likes (F3-family)
5. https://www.tiktok.com/@jakedevelops/video/7681130126041484565 — paste product-website URL into Dare (F2-family)

## Package contents

- videos.csv — 66 rows, ranked by views where view counts are exposed (TikTok exposes views; Instagram exposes likes/comments only, so those rows rank by no view count). Columns include duration, orientation, burned-in captions, Dare screen/branding visibility, on-screen evidence, and per-row verification level: 34 frames-inspected, 2 inspected but content differs from the source description, 30 source-caption-only.
- videos/ — 59 downloaded files referenced by the CSV (43 Dare-related TikToks, 11 verified F3-family clips, 2 mismatches and 3 off-format rejections kept for transparency).
- screenshots/ — 11 frame grids from inspected videos.

## Open gaps

- No exact match for any of the three formats as briefed. A seed example URL or handle would unblock targeted verification.
- 51 F1 keyword-only leads uninspected; 7 F3 candidates still rest on source listings (6 YouTube downloads blocked by a sign-in bot check, 1 Instagram image-only post, all out of cookieless reach); 30 CSV rows overall are source-caption-only rather than frame-verified.
- Google Drive delivery remains blocked (account over quota), so this package is delivered as files.
