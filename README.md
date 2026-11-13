# DDoS Protected VPS: Is Built-In Protection Enough, Which JustHost Plan Fits, and What It Costs (Full Plan Table + 3 Questions to Ask Before You Pay)

JustHost sells a DDoS protected VPS from **$2.25 per month** on 12-month billing, or $2.81 month-to-month. That entry plan, Sirius Special, gives you 1 core, 1 GB RAM and 20 GB NVMe. Protection is listed as included on every VPS rather than sold as a paid add-on tier.

What the plan page never states is how much attack traffic that protection absorbs before it stops helping. That number decides whether a cheap box is a real answer to a flood or a label on a product page. Below: the full JustHost lineup with both billing prices, the three questions to put to any host selling "DDoS protected" hosting, plan picks by workload, and the hardening work that stays yours no matter who you buy from.

> **Quick pick:** the **Vega Special at $6.23/month** on 12-month billing ($7.79 monthly) covers most single-site and single-app deployments: 2 cores, 4 GB RAM, 80 GB NVMe, 500 Mbit fair-share port. Take Sirius at $2.25 only if you need a VPN endpoint, a monitor, or a static page with almost no traffic.
>
> 👉 [See the current JustHost VPS lineup and both billing prices](https://justhost.asia/en/vps?ref=196392)

## All JustHost VPS plans and what each one costs

Two prices appear against every plan. The first is what you pay month-to-month; the second is the effective monthly rate when you prepay 12 months, which JustHost lists as 20% off. All figures below are as shown on the provider's VPS page.

| Plan | CPU / RAM | NVMe | Fair-share port | Monthly / 12-month rate | Order |
| --- | --- | --- | --- | --- | --- |
| Sirius Special | 1 core / 1 GB | 20 GB | 300 Mbit (~93+ TB) | $2.81 / $2.25 | [Order Sirius](https://justhost.asia/en/vps?ref=196392) |
| Arcturus Special | 1 core / 2 GB | 30 GB | 300 Mbit (~93+ TB) | $4.01 / $3.21 | [Order Arcturus](https://justhost.asia/en/vps?ref=196392) |
| Vega Special | 2 cores / 4 GB | 80 GB | 500 Mbit (~155+ TB) | $7.79 / $6.23 | [Order Vega](https://justhost.asia/en/vps?ref=196392) |
| Yildun Special | 4 cores / 8 GB | 200 GB | 750 Mbit (~232+ TB) | $16.20 / $12.96 | [Order Yildun](https://justhost.asia/en/vps?ref=196392) |
| Betelgeuse Special | 6 cores / 12 GB | 400 GB | 750 Mbit (~232+ TB) | $26.40 / $21.12 | [Order Betelgeuse](https://justhost.asia/en/vps?ref=196392) |
| Altair Special | 8 cores / 24 GB | 600 GB | 750 Mbit (~232+ TB) | $47.40 / $37.92 | [Order Altair](https://justhost.asia/en/vps?ref=196392) |

The bandwidth column deserves a second look. "Unmetered" here means unmetered inside a capped port speed, and the provider itself translates each port into a monthly volume: roughly 93 TB at 300 Mbit, 155 TB at 500 Mbit, 232 TB at 750 Mbit. That ceiling is the number that matters during a volumetric attack. A 300 Mbit port has less room to absorb junk traffic before legitimate requests queue behind it.

### The 12-month discount in actual money

Annual prepay saves a flat 20%, which is easy to underestimate at the low end and easy to overestimate at the high end:

| Plan | Monthly billing, 12 months | 12-month prepay | Saved |
| --- | --- | --- | --- |
| Sirius | $33.72 | $27.00 | $6.72 |
| Arcturus | $48.12 | $38.52 | $9.60 |
| Vega | $93.48 | $74.76 | $18.72 |
| Yildun | $194.40 | $155.52 | $38.88 |
| Betelgeuse | $316.80 | $253.44 | $63.36 |
| Altair | $568.80 | $455.04 | $113.76 |

For Vega, prepaying is worth about one and a half months of free service. For Sirius, the discount is smaller than a sandwich. If you are still deciding whether the platform is stable enough for your project, pay monthly on the first plan and move to annual billing once you have run a full month without surprises.

## The storage-picker plans (HDD, SSD or NVMe, 5 GB to 50 GB)

JustHost also runs a configurable line where you choose the disk type. HDD is cheapest per gigabyte, SSD sits in the middle, NVMe costs most and performs best. Same 20% annual discount applies.

| Plan | CPU / RAM | Disk | Monthly / 12-month rate |
| --- | --- | --- | --- |
| HDD VPS Start | 1 core / 512 MB | 5 GB HDD | $3.25 / $2.60 |
| SSD VPS Start+ | 1 core / 512 MB | 5 GB SSD | $3.90 / $3.12 |
| NVMe VPS Start++ | 1 core / 512 MB | 5 GB NVMe | $4.22 / $3.38 |
| HDD VPS Standard | 2 cores / 2 GB | 25 GB HDD | $11.00 / $8.80 |
| SSD VPS Standard+ | 2 cores / 2 GB | 25 GB SSD | $13.20 / $10.56 |
| NVMe VPS Standard++ | 2 cores / 2 GB | 25 GB NVMe | $14.30 / $11.44 |
| HDD VPS Super | 4 cores / 4 GB | 50 GB HDD | $22.00 / $17.60 |
| SSD VPS Super+ | 4 cores / 4 GB | 50 GB SSD | $26.40 / $21.12 |
| NVMe VPS Super++ | 4 cores / 4 GB | 50 GB NVMe | $28.60 / $22.88 |

IPv6-only configurations start lower still, from $1.60 per month at the 12-month rate, and IPv4 plus IPv6 setups begin at $2.60. Running the numbers, the Special lineup usually beats the picker on value: Vega Special gives you 4 GB RAM and 80 GB NVMe for $6.23, while NVMe VPS Standard++ gives 2 GB and 25 GB for $11.44. The picker only wins when you specifically need an HDD volume for cold storage or backups.

👉 [Compare the configurable HDD, SSD and NVMe plans](https://justhost.asia/en/vps?ref=196392)

## What "built-in DDoS protection" means on JustHost's page

JustHost states that every VPS includes filtering against malicious traffic, and describes a multi-layered approach that pairs traffic monitoring with mechanisms intended to stop attacks as they begin. It also says the protection covers "the main types of DDoS attacks."

That is a fair description of intent and a thin description of capability. There is no published Gbps ceiling, no statement of which layers (network, transport, application) are covered, and no mention of scrubbing capacity. Plenty of hosts word it the same way. The difference between a $2.25 plan and a $99/month mitigation add-on elsewhere usually sits exactly in those missing numbers.

## The three questions that separate real protection from a checkbox

Hosts describe DDoS protection in two broad models, and the gap between them is large enough to change your buying decision.

Liquid Web, as listed on its VPS pricing page, gives every VPS free volumetric Layer 4 filtering capped at **2 Gbps**, then sells Advanced at **$99/month per server** for attacks up to 10 Gbps and Premium at **$499/month per account** for complex or sustained attacks. OVHcloud takes the opposite approach and advertises unmetered mitigation on all VPS at no extra charge, positioning it as part of the network rather than a product tier.

Neither model is automatically better. What matters is that you know which one you are buying. Three questions get you there:

1. **What is the mitigation ceiling in Gbps?** A 2 Gbps filter handles script-kiddie floods and folds against a serious volumetric attack. "Unmetered" claims need the same scrutiny: ask what capacity sits behind the claim.
2. **Is mitigation always on and automatic, or does it require a ticket?** If you have to open a support request while your site is down, the clock starts late.
3. **Is the layer you are attacked on actually covered?** Network-layer filtering will not stop an HTTP flood that looks like ordinary requests. That needs a WAF or a CDN in front.

JustHost answers question three partially (included, no add-on tier listed) and question two reasonably well with its always-on filtering language. Question one is unanswered on the site. If your project earns money and an hour offline costs more than the server, send support that question in writing before you pay.

## Which attack types should decide your purchase

Four categories cover most of what small and mid-sized projects actually face:

- **SYN floods and other protocol attacks** exhaust connection tables rather than bandwidth. Cheap to launch, effective against unpatched stacks.
- **UDP floods** are the standard weapon against game servers, where latency matters more than raw throughput.
- **DNS amplification** turns third-party resolvers into a traffic cannon aimed at your IP.
- **HTTP floods and application-layer attacks** look like normal requests and slip past pure network filtering.

JustHost's page does not break its coverage down by category. That is a reason to add your own layer rather than a reason to skip the plan. A CDN in front of the origin, a WAF with rate limits on login endpoints, and a hidden origin IP will absorb or deflect most application-layer traffic regardless of what the host filters upstream.

## Pick a plan by what you're running

**Static site, blog, VPN endpoint, uptime monitor.** Sirius Special, $2.25/month on annual billing. 1 GB RAM runs a lightweight stack fine. Skip it if you plan to install a control panel plus MySQL plus WordPress, since that combination wants more memory than 1 GB comfortably provides.

**One WordPress or WooCommerce store, or a small SaaS app.** Vega Special, $6.23/month. 2 cores and 4 GB handle a database, PHP workers and a panel without swapping. The 500 Mbit port gives ~155 TB of headroom, which matters more than CPU when a flood arrives.

**Game server or anything latency-sensitive on UDP.** Yildun Special, $12.96/month. 4 cores and the 750 Mbit port give you room to ride out volumetric attacks while players stay connected. Ask support whether game-protocol filtering is part of the package, because the public page does not say.

**Agency running several client sites.** Betelgeuse Special, $21.12/month, or better, two Vega boxes at $12.46 combined. Splitting clients across two servers means one attack takes down half your portfolio instead of all of it. That redundancy costs less than moving up a tier.

**Backups and media storage.** HDD VPS Super at $17.60/month for 50 GB spinning disk, or NVMe VPS Super++ at $22.88 for the same capacity on flash. Pay the extra five dollars if anything reads from that disk on page load.

One practical note: JustHost lets you add CPU cores, RAM or disk to an existing VPS without migrating data to another server, so starting small and scaling up is a supported path rather than a rebuild.

## What you still have to do after the server is online

A protected VPS filters junk before it reaches your machine. It does nothing about a weak SSH password, an outdated plugin, or an origin IP published in a DNS history database. The basics, in rough order of payoff:

- Switch to SSH key authentication and disable password logins entirely.
- Move SSH and admin panels off default ports.
- Put the origin IP behind a reverse proxy, VPN tunnel or CDN so attackers cannot aim directly at the server.
- Whitelist IPs or apply geo-blocking on admin interfaces and APIs.
- Run a WAF with automated blocking rules, and rate-limit login endpoints.
- Close ports and services you do not use.
- Keep the OS, panel and every dependency patched.
- Watch traffic logs for spikes that do not match your normal pattern.
- Schedule off-site backups and actually test a restore.

That last item matters more than it sounds. If an attack succeeds, or a provider suspends a server during an abuse investigation, the backup is the only thing standing between you and a very long week.

## Nobody can promise 100% mitigation

OVHcloud's own product material states that no mitigation setup guarantees complete success in every case, with outcomes depending on attack size, mitigation capacity and vulnerabilities in the targeted application. That is an unusually honest line from a host selling protection, and it applies across the industry.

A DDoS protected VPS is usually sufficient for a small or mid-sized site, a SaaS product or a store that needs to stay reachable. It is not sufficient if you hold regulated data, run financial services, or operate in a sector where attacks are sustained and well funded. Those cases call for a dedicated server, private cloud, or a managed security service layered on top.

## What buyers say about JustHost

Reviews for the justhost.asia domain on Trustpilot lean negative in the entries visible as of late 2026. Recurring complaints: support responses arriving after an outage has already resolved rather than during it, no public status page, intermittent instability, and a disputed suspension where a VPS was removed over an alleged abuse complaint. One reviewer reported a location change from Amsterdam to Helsinki after speeds collapsed.

Read those reviews as a signal about operational maturity rather than a verdict on the hardware. A $2.25 VPS is not a managed service, and the price reflects that. Practical response: keep independent off-site backups, avoid annual prepay until a monthly cycle has proven stable for your workload, and do not put anything on a single cheap box that cannot survive an hour offline.

## FAQ

**Does JustHost charge extra bandwidth if I get hit by an attack?**
Ports are listed as unmetered at a fixed speed (300, 500 or 750 Mbit) with the monthly volume already translated on the plan page. No overage pricing appears publicly. Confirm in writing with support if you expect large floods, since "unmetered port" and "no overage billing" are separate commitments.

**Monthly or annual billing?**
Annual prepay is 20% cheaper across every plan. Start monthly anyway if this is your first VPS with the provider, then switch after a clean month. The saving on Sirius is $6.72 a year, which does not justify the risk of being locked in.

**Is DDoS protection on a cheap VPS just decoration?**
It depends on whether filtering happens upstream of your server. Filtering at the network edge, before traffic reaches your box, is real protection. If the plan relies on a software firewall inside a 1 GB VPS, a modest flood will take the machine down along with the firewall. JustHost describes filtering of malicious traffic and monitoring as part of the VPS package, which points to upstream filtering, but the absence of a published Gbps figure means you should treat it as baseline protection and add a CDN.

**Can I upgrade later without rebuilding?**
Yes. JustHost states you can add CPU cores, RAM or disk at any time without moving your data, with changes applied after a short downtime window.

**How do I move an existing site over?**
Lower your DNS TTL a day ahead, take a full backup of files and databases, deploy on the new VPS, test against the IP directly, then switch DNS. JustHost's site documents ordering and control panel access but does not advertise a free migration service, so plan to do the move yourself or ask support what they can help with before you buy.

## Before you order

Three rules cover most readers:

- **A small endpoint, VPN or static page:** Sirius Special at $2.25/month. Do not pay for capacity you will not use.
- **One app with a database behind it:** Vega Special at $6.23/month. It is the cheapest plan here that will not fold under a normal WordPress or Node stack.
- **Game servers, multi-tenant workloads, or anything with real traffic:** Yildun at $12.96 or Betelgeuse at $21.12, and split across two boxes if a single outage would hurt.

Two things to confirm before paying: ask support for the mitigation ceiling in Gbps and whether filtering is always-on, and check the refund terms for the billing cycle you choose. If both answers are acceptable, start monthly, keep backups off the server, and put a CDN in front of the origin on day one.

👉 [Start with the Vega Special at $6.23/month on 12-month billing](https://justhost.asia/en/vps?ref=196392)
