# Free-perks v22: production assets without a credit clock

Historical source date: 16 October 2026. Re-edited 16 November 2026. Not refreshed. Prices, terms, availability, interface labels and requirements are historical claims, not an offer, eligibility decision or permission to act. Source quality and gaps are retained.

Historical source/licence shortlist, 16 October 2026, 17:25 BST. This is not an asset manifest or clearance for any included project or media file.

For render/video work, correctly licensed assets can be more useful than expiring startup credits. Poly Haven and ambientCG offer commercial-use CC0 assets; API access has separate rules. Quaternius has a source-date redistribution restriction alongside older CC0 pack wording. Fab's free products are not public domain, and NASA/BBC media are not blanket free advertising libraries.

## Ranked sources

| Rank | Source | Useful benefit | Important boundary |
| --- | --- | --- | --- |
| 1 | Poly Haven | HDRIs, textures and 3D models under CC0, including commercial projects | Asset licence differs from live API service and website preview/copy rights |
| 2 | ambientCG | CC0 materials and assets with commercial reuse/raw-file inclusion | Special-access remote library/batch features are separate; do not infer all delivery routes are uncapped |
| 3 | Kenney | CC0 game assets, commercial use with no attribution requirement | Check included licence per pack; logo is not part of the grant |
| 4 | Quaternius | Commercial models/animation packs, free portions | Source-date QAL forbids asset redistribution; older pack pages still say CC0 |
| 5 | Fab | Free/temporarily free licensed assets | Correct acquisition tier, actual product licence and project-only sharing; no automatic claim |
| Conditional | Freesound | Individual CC0 or attribution sounds | Mixed licences, account needed to download, provenance/Content ID risk |
| Not blanket commercial free | NASA/JPL, BBC Sound Effects (not blanket commercial free) | Publicly accessible media | Credit, third-party/people/logo/advertising or paid commercial-licence restrictions |

The ranking is based on practical commercial-project use and low account/expiry friction. No asset quality, file compatibility or final project fit has been tested in this version. All source claims checked 16 October 2026.

## Poly Haven: CC0 assets and a now-free API are distinct permissions

Asset licence: https://polyhaven.com/license

API announcement and operating conditions: https://polyhaven.com/our-api

Linked full API terms: https://github.com/Poly-Haven/Public-API/blob/master/ToS.md

Corporate options: https://polyhaven.com/corporate

HDRIs, textures and models are CC0. The asset licence permits commercial use, modification, sharing and inclusion in sold products, without required attribution. It does not make every part of the website CC0: logo, copy, avatars, example renders and user-submitted renders have separate rights.

The source-date API page dates the change to **18 July 2026** and says basic public API access is free for personal/academic/commercial use, with no account or API key needed for default endpoints. The linked formal terms confirm no commercial-access fee. This removes the need to invent a paid commercial API subscription.

But a product using the **live API** must visibly identify Poly Haven as the asset source and send a distinctive application User-Agent or Referer. The page says User-Agent; the formal terms allow matching Referer or User-Agent. Attribution is a condition of the service, not of already downloaded/self-hosted CC0 files. Do not confuse the two and add false mandatory attribution to an offline render.

The website terms prohibit unauthorized scraping/data mining. Use the documented API for a legitimate integration rather than crawling the web pages. API service is best-effort with no uptime guarantee. Optional paid provenance attestation or bulk snapshots are operational services, not a mandatory asset licence.

For a future project: save the asset page/licence, exact filename/version and local original; choose the appropriate resolution rather than a huge default. 

## ambientCG: raw-file inclusion allowed, delivery extras are separate

Licence: https://docs.ambientcg.com/license/

Special-access page: https://ambientcg.com/activate

Source-date API docs: https://docs.ambientcg.com/api/v3/

The official CC0 licence covers downloadable assets **and their material preview renders**. It permits commercial use/modification/distribution and inclusion of raw files in a game/project. Attribution is appreciated but not required.

The special-access page advertises a batch downloader, Blender Remote Library and original Substance project files. It explicitly limits **free Blender Remote Library access to 1K**. That is not a blanket 1K limit on ordinary website texture downloads, nor proof every delivery extra is free. Optional Patreon/Ko-fi support should not be confused with the CC0 copyright permission.

Source-date docs describe v3 API read-only GET endpoints. Older indexed v2 docs say v2 no longer receives updates. New integrations should not be designed from a legacy v2 example without checking the documentation in force for the new integration. No end-to-end technical test is established by the source research.

## Kenney: useful CC0, not permission to use the brand

Official support/licence explanation: https://kenney.nl/support

Asset catalogue: https://kenney.nl/assets

Kenney says game assets on its asset pages are CC0, including commercial projects, with no attribution requirement. The included pack licence or asset page remains the record to keep. Its logo is reserved for official studio projects and should not be used as a third-party endorsement badge.

This is a source lead for UI/game prototyping and stylised scenes, not a statement about a project's chosen visual direction. Bulk All-in-1 bundles are a separate offer; individual free assets do not mean every bundle/store product costs zero. 

## Quaternius: an actual licence conflict, not a universal CC0 library now

Source-date QAL v1.0, last updated 28 August 2026: https://quaternius.com/license.html

Older pack pages still carrying CC0 language:
https://quaternius.com/packs/universalanimationlibrary.html
https://quaternius.com/packs/universalbasecharacters.html

The source-date **Quaternius Asset License** allows commercial games, apps, films, videos, artworks and renders without royalties or required credit. Collaborators/contractors may use assets solely to work on the product.

It forbids redistributing original **or modified** assets as standalone assets, packs, stock files, templates or similar products, for free or payment. A completed product incorporating the assets is different from an asset/template giveaway. Do not put raw QAL content in a public starter/template repository merely because a render using it is allowed.

The two pack pages above still call their material CC0. This conflict needs the **actual downloaded pack's licence and acquisition date** before asserting raw redistribution rights. The QAL says later versions apply only to future releases, not retroactively to assets obtained under an earlier version. That supports preserving dated licence evidence, not guessing that every new download is CC0 or every old copy is now restricted.

Pack marketing also distinguishes free partial versions from additional/source/engine-project versions. "120+ animations in the library" is not a promise that every file/source project is in the free download. 

## Fab: free price does not mean unrestricted sharing

Official summary: https://www.fab.com/eula

Official pricing/licence docs: https://dev.epicgames.com/documentation/en-us/fab/licenses-and-pricing-in-fab

Fab offers CC-BY and Standard licences, with some listings retaining a legacy Marketplace licence. Check the specific listing and acquired version, not just the site's brand.

Standard permits commercial projects, modification, compatible tools outside Unreal and sharing with project collaborators, including via a **private** project repository. It forbids standalone resale/redistribution. A public asset dump is not project collaboration.

Personal and Professional are pricing tiers with the same rights, not "non-commercial versus commercial". Selection depends on prior twelve-month gross commercial revenue: Personal at no more than $100,000, Professional above. The summary says crossing the threshold after acquisition does not force a retroactive tier upgrade. Pricing-tier selection needs actual revenue facts; no tier is selected here.

Reference-Only content does not provide source files. A free listing or promotion must still be acquired under the right terms; old free price does not prove it remains free today. 

## Sound: per-file licence matters more than "free library"

Freesound official FAQ: https://freesound.org/help/faq/

Its library mixes CC0, CC-BY, CC-BY-NC and older Sampling+ files. For commercial work, do not download a non-commercial file or omit a CC-BY credit. The FAQ warns user uploads may sometimes contain unauthorized material, and it explains how otherwise valid reuse can still receive automated Content ID claims. Save the source page, licence and upload date; "royalty-free" is not an assurance of no claims.

BBC's own answer: https://www.bbc.co.uk/contact/questions/using-bbc-content/use-sound-effects

The publicly accessible BBC collection is BBC copyright and the free permission is personal/educational/research subject to its licence. It is not a free sound bed for a paying client's promotional video. Commercial licensing is separate; no paid quote is treated as free.

New account-gated alternative, not tested: https://www.lotsofsounds.com/

This site claims CC0 commercial sound downloads, but downloads require an account and its API/MCP access is paid.  It is not established as a no-account production source.

## NASA/JPL: not a blank cheque for brand advertising

NASA media rules: https://www.nasa.gov/nasa-brand-center/images-and-media/

JPL policy: https://www.jpl.nasa.gov/jpl-image-use-policy/

NASA says much informational/editorial material generally is not subject to US copyright, but marks third-party copyrighted content separately. Media access does not transfer those third-party rights. Logos, identifiers, identifiable people and endorsement implications require separate checks, especially in advertising, products and promotional cover art.

JPL asks for the specified credit line, normally "Courtesy NASA/JPL-Caltech", and also identifies exceptions for logos, people and third-party copyright. NASA's current-employee likeness restrictions do not disappear just because the face is partly hidden by a spacesuit. Do not use a famous astronaut image as a casual free client advert or turn a NASA logo into a brand-association claim.

NASA's media page also has AI-output/source-attribution conditions. It is not appropriate to replace those specifics with "all NASA images public domain, do whatever". Actual item caption, source rights and use context control. 

## Evidence to keep for any selected asset

Keep a dated manifest with source item URL, author/provider, download date, exact licence, filename/version, any required credits and intended deliverable. Keep unmodified originals outside the live project. Test in a duplicate and verify export/appearance before adopting.
