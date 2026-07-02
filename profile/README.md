# Orbis Geographical Internet (GeoNet)

**[Orbis](https://orbis.social)** is a [geo-social network](https://en.wikipedia.org/wiki/Geosocial_networking) in which communities collaboratively map their cultural identity over physical space: tribal territories are amorphous polygons computed in real time from collective territorial claims. It is an applied computer-science research program in geospatial computing and decentralized cultural infrastructure, funded by [FAPESP PIPE I and II](https://bv.fapesp.br/en/auxilios/111929/orbis-geolocation-social-network-and-collaborative-urban-mapping/).

Orbis is an incipient prototype for the territorialization of a network society ([Carnoy & Castells, 2001](https://onlinelibrary.wiley.com/doi/10.1111/1471-0374.00002)) and a **GeoNet** — a geographical layer of the internet ([Graham, 2013](https://doi.org/10.1111/geoj.12009); [Kitchin & Dodge, 2011](https://direct.mit.edu/books/oa-monograph/5039/Code-SpaceSoftware-and-Everyday-Life)), in the lineage of [Vernadsky's noosphere (*ноосфера*, 1944)](https://vernadsky.lib.ru/e-texts/archive/noos.html). It supplies the spatial substrate the network-society literature presupposes: the cartographic primitives by which a digitally-constituted community claims physical ground without administrative inscription — [Milton Santos's (1996)](https://www.edusp.com.br/livros/natureza-do-espaco/) coupling of systems of objects and systems of actions (*sistemas de objetos e sistemas de ações*); [Sundaram's (2010)](https://www.routledge.com/Pirate-Modernity-Delhis-Media-Urbanism/Sundaram/p/book/9780415611749) re-territorialization from below. The territory-fusion algorithm operationalizes [Deleuze & Guattari's (1980)](https://www.leseditionsdeminuit.fr/livre-Capitalisme_et_schizophr%C3%A9nie_2___Mille_plateaux-2015-1-1-0-1.html) *territorialisation / déterritorialisation* dialectic as a [cosmotechnics (Hui, 2016)](https://www.urbanomic.com/book/question-concerning-technology-china/) of collective mapping.

---

## From polygons to a GeoNet

The [territory-fusion research](https://github.com/orbis-geonet/research) is what makes this concrete. Each community stakes claims to real-world places, and thousands of claims are fused in real time into organic tribal polygons — tangent bridges connect nearby claims, collisions between rival groups reject a merge, and the hole-preserving union keeps interior gaps intact. A territory is addressed by the claims it contains, and fusion and split are first-class idempotent operations. These are the cartographic primitives of a *geographical* internet: where the internet addresses information by IP, a GeoNet addresses **ground by claim** — a community draws, holds, and federates territory directly on the map, with no central cadastre. In the [orbis-geonet protocol](https://orbis.social/network), those territories become permissionlessly federable: proofs and geo-tagged pointers live in ZK-compressed Merkle trees on Solana, discovery is by location-prefix, and independent clones sync ground-to-ground in a [native token](https://orbis.social/exchange) — the geographical layer of the internet, run by its inhabitants.

<p align="center">
  <img src="https://raw.githubusercontent.com/orbis-geonet/.github/main/profile/imgs/territory-polygons.png" height="300" alt="Territory-fusion polygons from the research" />
  &nbsp;&nbsp;
  <img src="https://raw.githubusercontent.com/orbis-geonet/.github/main/profile/imgs/app-territories.jpg" height="300" alt="Tribal territories on the map in the Orbis app" />
</p>

<p align="center"><em>The territory-fusion algorithm (left, from the <a href="https://github.com/orbis-geonet/research">research</a>) rendered live as tribal territories on the map in the app (right).</em></p>

---

## Run your own Orbis

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

**Accessible, and priced at the network minimum.** Spinning up a clone needs no permission: fork the stack below, rebrand it, deploy it, and register your clone on-chain — a one-time **50 ORBIS** — to join the federation. Orbis settles on **Solana**, so every action pays the network's absolute minimum: a base fee of **~0.000005 SOL** per transaction. On top of that, the [live protocol](https://orbis.social/network) charges a flat **0.0001 [ORBIS](https://orbis.social/exchange) per write** (and per MB of media) — the same price for a hobby clone and a global one, with **no tiers**.

| Users on your clone | Writes / month (~50 each) | Protocol fee / month | Per user |
|---|---|---|---|
| 1,000 | ~50K | 5 ORBIS | 0.005 ORBIS |
| 10,000 | ~500K | 50 ORBIS | 0.005 ORBIS |
| 100,000 | ~5M | 500 ORBIS | 0.005 ORBIS |
| 1,000,000 | ~50M | 5,000 ORBIS | 0.005 ORBIS |

<p align="center"><em>Live fees from the <a href="https://orbis.social/network">network dashboard</a> — a flat 0.0001 ORBIS per write at any scale, so the per-user cost stays 0.005 ORBIS/month from a thousand users to a million, on top of Solana's minimal network gas. Cost is never a barrier to running a clone.</em></p>

---

|  | Website | iPhone App | Android App |
|---|---|---|---|
| Genesis | [orbis.social](https://orbis.social) | [App Store](https://apps.apple.com/ca/app/orbis-digital-tribes/id1453025529) | [Google Play](https://play.google.com/store/apps/details?id=com.orbis.orbis) |
| Clone 1 | | | |
| Clone 2 | | | |
| Clone 3 | | | |

---

## Research

| Repository | Description |
|---|---|
| [research](https://github.com/orbis-geonet/research) | Lorem ipsum dolor sit amet, consectetur adipiscing elit. |

## Front End — Mobile

| Repository | Description |
|---|---|
| [ios-app](https://github.com/orbis-geonet/ios-app) | Lorem ipsum dolor sit amet, consectetur adipiscing elit. |
| [android-app](https://github.com/orbis-geonet/android-app) | Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. |

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
| [email-marketing-dashboard](https://github.com/orbis-geonet/email-marketing-dashboard) | Email marketing software dashboard. |
| [marketing](https://github.com/orbis-geonet/marketing) | Social media short-form video marketing pipeline. |
