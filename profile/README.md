# Orbis Geographical Internet (GeoNet)

**[Orbis](https://orbis.social)** is a [geo-social network](https://en.wikipedia.org/wiki/Geosocial_networking) in which communities collaboratively map their cultural identity over physical space: tribal territories are amorphous polygons computed in real time from collective territorial claims. It is an applied computer-science research program in geospatial computing and decentralized cultural infrastructure, funded by [FAPESP PIPE I and II](https://bv.fapesp.br/en/auxilios/111929/orbis-geolocation-social-network-and-collaborative-urban-mapping/).

Orbis is an incipient prototype for the territorialization of a network society ([Carnoy & Castells, 2001](https://onlinelibrary.wiley.com/doi/10.1111/1471-0374.00002); [Srinivasan, 2022](https://thenetworkstate.com/)) and a **GeoNet** — a geographical layer of the internet ([Graham, 2013](https://doi.org/10.1111/geoj.12009); [Kitchin & Dodge, 2011](https://direct.mit.edu/books/oa-monograph/5039/Code-SpaceSoftware-and-Everyday-Life)), in the lineage of [Vernadsky's noosphere (*ноосфера*, 1944)](https://vernadsky.lib.ru/e-texts/archive/noos.html). It supplies the spatial substrate the network-society literature presupposes: the cartographic primitives by which a digitally-constituted community claims physical ground without administrative inscription — [Milton Santos's (1996)](https://www.edusp.com.br/livros/natureza-do-espaco/) coupling of systems of objects and systems of actions (*sistemas de objetos e sistemas de ações*); [Sundaram's (2010)](https://www.routledge.com/Pirate-Modernity-Delhis-Media-Urbanism/Sundaram/p/book/9780415611749) re-territorialization from below. The territory-fusion algorithm operationalizes [Deleuze & Guattari's (1980)](https://www.leseditionsdeminuit.fr/livre-Capitalisme_et_schizophr%C3%A9nie_2___Mille_plateaux-2015-1-1-0-1.html) *territorialisation / déterritorialisation* dialectic as a [cosmotechnics (Hui, 2016)](https://www.urbanomic.com/book/question-concerning-technology-china/) of collective mapping.

---

## Computing territory, federating the map

The [territory-fusion research](https://github.com/orbis-geonet/research) is what makes this concrete. Each community stakes claims to real-world places, and thousands of claims are fused in real time into organic tribal polygons — tangent bridges connect nearby claims, collisions between rival groups reject a merge, and the hole-preserving union keeps interior gaps intact. A territory is addressed by the claims it contains, and fusion and split are first-class idempotent operations. These are the cartographic primitives of a *geographical* internet: where the internet addresses information by IP, a GeoNet addresses **ground by claim** — a community draws, holds, and federates territory directly on the map, with no central cadastre. In the [orbis-geonet protocol](https://orbis.social/network), those territories become permissionlessly federable: proofs and geo-tagged pointers live in ZK-compressed Merkle trees on Solana, discovery is by location-prefix, and independent clones sync ground-to-ground in a [native token](https://orbis.social/exchange) — the geographical layer of the internet, run by its inhabitants.

<p align="center">
  <img src="https://raw.githubusercontent.com/orbis-geonet/.github/main/profile/imgs/app-map-1.png" height="440" alt="Tribe territories live on the map" />
  &nbsp;
  <img src="https://raw.githubusercontent.com/orbis-geonet/.github/main/profile/imgs/app-map-2.png" height="440" alt="Nearby tribes and their claimed regions" />
  &nbsp;
  <img src="https://raw.githubusercontent.com/orbis-geonet/.github/main/profile/imgs/app-map-3.png" height="440" alt="A single tribe's claimed territory" />
</p>
<p align="center">
  <img src="https://raw.githubusercontent.com/orbis-geonet/.github/main/profile/imgs/research-connect.png" height="175" alt="Research: nearby claims connected by tangent bridges" />
  <img src="https://raw.githubusercontent.com/orbis-geonet/.github/main/profile/imgs/research-collision.png" height="175" alt="Research: a collision between rival tribes rejects a merge" />
  <img src="https://raw.githubusercontent.com/orbis-geonet/.github/main/profile/imgs/research-polygons.png" height="175" alt="Research: claims fused into amorphous polygons" />
  <img src="https://raw.githubusercontent.com/orbis-geonet/.github/main/profile/imgs/research-territories.png" height="175" alt="Research: tribal territories with computed centers" />
</p>

<p align="center"><em>Top — tribal territories live on the map in the Orbis app. Bottom — the <a href="https://github.com/orbis-geonet/research">territory-fusion research</a> behind them: nearby claims connect by tangent bridges, a collision between rival tribes rejects a merge, the union fuses them into amorphous polygons, and each territory gains a computed center.</em></p>

---

## Become an Orbis clone node operator

This organization exists to help **clone operators** create their own **branded** clone of the Orbis app and connect it to the [**orbis-geonet**](https://orbis.social/network) — the permissionless, federated network where independent clones share one map protocol and sync territory to one another. It is equally where operators and contributors improve the common project: suggest features, report and fix bugs, and refine the protocol together. [orbis.social](https://orbis.social) is the Genesis reference instance; the repositories below — iOS, Android, web, backend — are what you fork to run your own, and the *Clone* rows in the table await federated operators.

```mermaid
graph TD
    GN(["<b>orbis-geonet</b> — one shared map protocol<br/>Solana · ZK-compressed Merkle trees · location-prefix discovery"])
    G["<b>Genesis</b><br/>orbis.social"] <--> GN
    A["Clone<br/>your brand"] <--> GN
    B["Clone<br/>another brand"] <--> GN
    C["Clone<br/>another brand"] <--> GN
```

<p align="center"><em>Independent, branded clones federate through one shared map protocol — syncing territory to one another to form the GeoNet.</em></p>

**Accessible, and priced at the network minimum.** Spinning up a clone needs no permission: fork the stack below, rebrand it, deploy it, and register your clone on-chain — a one-time **50 [$ORBIS](https://orbis.social/exchange) (≈ $50)** — to join the federation. From then on, writes are **batched**: the worker bundles up to **200 user actions (plus 32 collection updates) into a single on-chain write**, which costs a flat **0.0001 $ORBIS** ($0.0001, since $ORBIS is pegged to $1.00) plus the Solana network minimum (~0.000005 SOL per batch). No tiers — the same for a hobby clone and a global one.

| Users on your clone | Actions / month | Batches (~200 each) | Protocol fee ($ORBIS) | Network (SOL) | ≈ Total / month |
|---|---|---|---|---|---|
| 1,000 | ~50K | ~250 | 0.025 $ORBIS · $0.03 | ~0.00125 SOL · ~$0.10 | **~$0.13** |
| 10,000 | ~500K | ~2,500 | 0.25 $ORBIS · $0.25 | ~0.0125 SOL · ~$1 | **~$1.25** |
| 100,000 | ~5M | ~25,000 | 2.5 $ORBIS · $2.50 | ~0.125 SOL · ~$10 | **~$12.50** |
| 1,000,000 | ~50M | ~250,000 | 25 $ORBIS · $25 | ~1.25 SOL · ~$100 | **~$125** |

<p align="center"><em>Assumes ~50 actions per active user / month, batched at ~200 actions per on-chain write (per the <code>sync_collection_batch</code> contract). Fees from the <a href="https://orbis.social/network">network dashboard</a> at 1 $ORBIS = $1.00 and SOL ≈ $80. A million-user clone costs about <strong>$125 / month — roughly $0.000125 per active user</strong>. Cost is never a barrier to running a clone.</em></p>

**Clones pay each other for data — so the network funds its own hosting.** Each clone stores its own users' posts and media and serves them to the rest of the federation on demand. When one clone's users encounter data or media hosted by another, the requesting clone pays the **clone operator** in **$ORBIS** through an on-chain **streaming escrow**: the requester locks $ORBIS naming the clone operator (`init_streaming_escrow`), and the clone operator draws payment **metered per MB actually served** (`claim_streaming_payment` — `mb = data_size / 1 MB`, `fee = mb × fee_per_mb` at **0.0001 $ORBIS/MB**, minimum 0.0001 $ORBIS), each claim signed by the requester so no one overpays. The clone operator keeps **99%**; the remaining **1% funds the protocol treasury — which pays for the continued open-source development of these repositories** (the clients, backend, and protocol every operator forks). Only clone operators with an on-chain **trust score ≥ 500** can be paid, so reliable hosting is rewarded.

Crucially, a clone **only pays for the content its own users actually open** — each item is fetched once, cached, and never charged again — **not for the whole network.** Mirroring everything is optional (running a full **genesis** clone) and is not required to operate. So a clone's data cost tracks only what its users view, while hosting the content those users create becomes a revenue stream — which is what keeps information and media available across the GeoNet with no central CDN.

*Example — what a **clone operator** earns when other clones' users pull media it stores (0.0001 $ORBIS/MB, 1 $ORBIS = $1.00; clone operator keeps 99%):*

| Media pulled from a clone operator / month | Requesters pay | Operator keeps (99%) | Treasury (1%) |
|---|---|---|---|
| 10 GB | ~1.0 $ORBIS · ~$1 | ~$1.01 | ~$0.01 |
| 100 GB | ~10.2 $ORBIS · ~$10 | ~$10.14 | ~$0.10 |
| 1 TB | ~105 $ORBIS · ~$105 | ~$103.80 | ~$1.05 |
| 10 TB | ~1,049 $ORBIS · ~$1,049 | ~$1,038 | ~$10.49 |

<p align="center"><em>Metered per the <code>claim_streaming_payment</code> contract. A clone pays only for what its own users encounter (cached, paid once); a clone operator earns $ORBIS whenever the federation pulls its content — so hosting pays for itself.</em></p>

**Cache it once, then earn from it.** When a clone fetches foreign content it keeps a local copy and registers as an additional **source** for it (`register_clone` + `sync_collection_batch`, discoverable network-wide through its on-chain `CloneInfo`), so it **never pays for that content twice**. Every cached copy is also a **fallback**: if the operator that first hosted a piece of content goes offline, requesters pull it from any other clone that holds it — `proxyToProvider` walks the list of sources until one answers — so **nothing 404s out of existence because a single host disappeared.** The more a piece of content is viewed, the more clones mirror it and the more resilient it becomes. The economy runs both ways: a clone **spends $ORBIS to capture content** its users want, and **earns $ORBIS** whenever another operator's users pull content it created or cached. Replicating the whole network is optional (Mirror-full or Genesis modes) and never required to run a clone — and the $ORBIS earned is liquid, swapping to **SOL** any time on the [$ORBIS exchange](https://orbis.social/exchange).

---

| | Name | Provenance | Website | iPhone App | Android App | Contact |
|---|---|---|---|---|---|---|
| Genesis | Orbis Digital Tribes | Brazil | [orbis.social](https://orbis.social) | [App Store](https://apps.apple.com/ca/app/orbis-digital-tribes/id1453025529) | [Google Play](https://play.google.com/store/apps/details?id=com.orbis.orbis) | [info@orbis.social](mailto:info@orbis.social) |
| Clone 1 | | | | | | |
| Clone 2 | | | | | | |
| Clone 3 | | | | | | |

<p align="center"><em>Running your own Orbis clone? To have it listed in this registry, open a pull request on <a href="https://github.com/orbis-geonet">orbis-geonet</a> or email <a href="mailto:info@geonetinternet.com">info@geonetinternet.com</a>.</em></p>

---

## Research

| Repository | Description |
|---|---|
| [research](https://github.com/orbis-geonet/research) | The territory-fusion research — how overlapping place-claims become smooth tribal territory polygons (tripwires, tangent bridges, hole-preserving union, and pole-of-inaccessibility centers), worked example by example. |

## Smart Contract

| Repository | Description |
|---|---|
| [smart-contract](https://github.com/orbis-geonet/smart-contract) | The Orbis Protocol — the Solana / Anchor program behind the orbis-geonet: state-compressed map writes, the clone registry and reputation system, and metered $ORBIS clone-to-clone payments. Includes a detailed breakdown of every instruction, account, and fee. |

## Front End — Mobile

| Repository | Description |
|---|---|
| [ios-app](https://github.com/orbis-geonet/ios-app) | Lorem ipsum dolor sit amet, consectetur adipiscing elit. |
| [android-app](https://github.com/orbis-geonet/android-app) | Native Android client (Kotlin) — the map, tribes, territory claiming, feed, stories, events, and messaging. |

## Front End — Web

| Repository | Description |
|---|---|
| [website](https://github.com/orbis-geonet/website) | Quis autem vel eum iure reprehenderit qui in ea voluptate velit. |
| [user-management-dashboard](https://github.com/orbis-geonet/user-management-dashboard) | User management dashboard. |
| [dynamic-site-map](https://github.com/orbis-geonet/dynamic-site-map) | Orbis dynamic site map. |

## Back End

| Repository | Description |
|---|---|
| [backend](https://github.com/orbis-geonet/backend) | Back-end services and blockchain integration (node and Java workers). |
| [polygon-creator](https://github.com/orbis-geonet/polygon-creator) | Neque porro quisquam est qui dolorem ipsum quia dolor sit amet. |

## Marketing

| Repository | Description |
|---|---|
| [marketing](https://github.com/orbis-geonet/marketing) | Social media short-form video marketing pipeline. |
