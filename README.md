# Cheap Cloud VPS: What $2.99–$5.99 a Month Really Buys, Which Evoxt Plan Fits Your Site, and the Add-On Fees That Change the Total (All 11 Plans Compared)

Entry prices for a cheap cloud VPS currently sit between $2 and $5 a month. IONOS starts at $2/month, Vultr at $2.50, Netcup at €3.35, Hetzner at €4.35, and DigitalOcean at $4. Evoxt's cheapest plan is $2.99/month for 512 MB RAM and 5 GB storage, and its 2 GB plan costs $5.99. Those numbers buy wildly different hardware: entry-level storage across providers ranges from 5 GB to 120 GB, so the sticker price alone tells you very little.

Below is the full Evoxt plan table with current prices, a way to calculate what you will actually pay after backups, control panels and renewals, and the configuration thresholds that decide whether a $2.99 plan is enough or a waste of time.

> **Quick picks.** Testing Linux, running a VPN or a bot: **VM-0.5 at $2.99/month** (1 core, 512 MB, 5 GB). One small WordPress site: **VM-1 at $5.99/month** (1 core, 2 GB, 20 GB). WooCommerce or several sites on one box: **VM-2 at $11.99/month** (2 cores, 4 GB, 30 GB). Every plan includes weekly offsite backups at no extra cost.
> 👉 [See the current Evoxt plan list and prices](https://bit.ly/EvoXt)

## All Evoxt plans, current pricing

Evoxt sells a single line of general-purpose VMs, all on KVM with CPUs advertised at up to 6.0 GHz+ per core. Prices are in USD and billed monthly; the company also allows prepayment for up to three years and account credit top-ups.

| Plan | vCPU | RAM | Storage | Price (USD/month) | Deploy |
| --- | --- | --- | --- | --- | --- |
| VM-0.5 | 1 core | 512 MB | 5 GB | $2.99 | [Deploy VM-0.5](https://bit.ly/EvoXt) |
| VM-0.75 | 1 core | 1 GB | 10 GB | $4.99 | [Deploy VM-0.75](https://bit.ly/EvoXt) |
| VM-1 | 1 core | 2 GB | 20 GB | $5.99 | [Deploy VM-1](https://bit.ly/EvoXt) |
| VM-1.5 | 2 cores | 2 GB | 20 GB | $6.95 | [Deploy VM-1.5](https://bit.ly/EvoXt) |
| VM-2 | 2 cores | 4 GB | 30 GB | $11.99 | [Deploy VM-2](https://bit.ly/EvoXt) |
| VM-3 | 4 cores | 4 GB | 30 GB | $14.99 | [Deploy VM-3](https://bit.ly/EvoXt) |
| VM-4 | 4 cores | 8 GB | 60 GB | $23.99 | [Deploy VM-4](https://bit.ly/EvoXt) |
| VM-6 | 8 cores | 8 GB | 60 GB | $29.99 | [Deploy VM-6](https://bit.ly/EvoXt) |
| VM-8 | 8 cores | 16 GB | 80 GB | $47.99 | [Deploy VM-8](https://bit.ly/EvoXt) |
| VM-12 | 16 cores | 16 GB | 80 GB | $60.95 | [Deploy VM-12](https://bit.ly/EvoXt) |
| VM-16 | 16 cores | 32 GB | 100 GB | $95.99 | [Deploy VM-16](https://bit.ly/EvoXt) |

Monthly transfer scales with the plan: 250 GB on VM-0.5 and VM-0.75, 500 GB on VM-1 and VM-1.5, 1 TB on VM-2 and VM-3, 2 TB on VM-4 and VM-6, 3 TB on VM-8 and VM-12, 5 TB on VM-16. VPSBenchmarks describes Evoxt's model as allowance-then-throttled, meaning traffic above the allowance slows the connection instead of producing an overage invoice.

Payment methods are cards, PayPal, Bitcoin and USDT on Tron. Windows and Linux images are both offered, and individual resources (extra cores, RAM, storage, IPs) can be added without moving to a different plan.

## The real monthly cost: where a $2.99 plan becomes $12

The first invoice is the least interesting number on the page. HostAdvice's cheap VPS guide lists the extras that routinely sit outside a headline price: control panel licences (cPanel, Plesk, DirectAdmin), automated backup fees, additional IPv4 addresses, renewal increases after the intro term, managed support, migration fees, security add-ons, bandwidth overage and advanced monitoring. A $3 plan with a $15 cPanel licence, $5 of backups and a $3 extra IP is a $26/month server.

The calculation that matters takes two minutes:

1. Start from the renewal price, not the intro price. HostAdvice warns that intro prices may rise after the first term, so the second year is the honest number.
2. Add the panel you actually need. If your workflow depends on cPanel or Plesk, price that licence before comparing anything else.
3. Add backups if they are not bundled, plus any extra IPv4 you need for mail or SSL on separate services.
4. Multiply by 12 and compare annual totals, not monthly ones.

Evoxt's structure removes three of those line items. Weekly offsite backups are included on every VM at no cost, the control panel is Evoxt's own and included, and each VM ships with an IPv4 address, with IPv6 and private networking between VMs available. The VM-1 stays $5.99/month unless you deliberately add CPU, RAM, storage or IPs. If you need cPanel specifically, budget for it elsewhere, because the included panel is custom rather than a licensed cPanel build.

One more billing detail worth knowing before you commit: Evoxt does not offer hourly billing. VPSBenchmarks' feature table lists hourly billing as unavailable, so this suits a machine you intend to keep running, not a workload you spin up for 40 minutes and destroy.

👉 [Check VM-1 pricing and the prepay options](https://bit.ly/EvoXt)

## How much VPS do you actually need?

HostAdvice's sizing guidance is the most concrete published baseline: 1 GB RAM for testing or a tiny site, 2 GB for a small WordPress install, 4 GB or more for WooCommerce or multiple websites, 20–50 GB of SSD or NVMe storage on typical cheap plans, and roughly 1 TB/month of bandwidth for a public site. Entry plans usually come with 1 vCPU.

| What you are running | Specs that matter | Evoxt plan |
| --- | --- | --- |
| Learning Linux, VPN endpoint, monitoring bot, staging box | 512 MB–1 GB RAM, 1 core | VM-0.5 ($2.99) or VM-0.75 ($4.99) |
| Personal blog or small business site, low traffic | 2 GB RAM, 20 GB storage | VM-1 ($5.99) |
| WordPress with plugins and growing traffic | 2 GB RAM, 2 cores | VM-1.5 ($6.95) |
| WooCommerce, or several sites on one server | 4 GB RAM, 2+ cores, 30 GB+ | VM-2 ($11.99) |
| Busy store, multiple sites, background jobs | 8 GB RAM, 4 cores | VM-4 ($23.99) |
| Minecraft or CS server, CI runner, app backend | More cores than RAM pressure | VM-6 ($29.99) or VM-8 ($47.99) |

A couple of judgement calls on that mapping. VM-1.5 is the cheapest way to get a second core, and the $0.96 gap over VM-1 is the smallest upgrade premium in the lineup. If your site runs a database and a PHP worker pool on the same box, that second core shows up under load long before RAM becomes the problem. On the other end, VM-0.5 with 512 MB is genuinely a proxy/VPN/test machine. Stack a control panel, MySQL and PHP on 512 MB and the OOM killer will introduce itself.

Storage is where Evoxt sits at the lean end. VM-1's 20 GB matches the bottom of the 20–50 GB range HostAdvice describes; VM-2's 30 GB is more comfortable for a store with images. Bandwidth is not a constraint at this tier: 500 GB on VM-1 and 1 TB on VM-2 covers most small sites, and overage is throttled rather than billed.

👉 [Start with VM-1 if you are moving a single site over](https://bit.ly/EvoXt)

## What the cheap tier does not cover

**You are the operations team.** An unmanaged VPS includes the server and little else, as HostAdvice puts it: security, backups, updates, monitoring and software are yours to configure. Evoxt's weekly offsite backup and firewall rules reduce the risk, but nobody will patch your WordPress install for you. If you would rather not touch a shell, a managed plan at two to three times the price is the correct purchase.

**Free tiers are for experiments.** Kamatera's 30-day trial (up to $100 in resources), Mikr.us' 256 MB free micro VPS and DigitalOcean's $100 education credit are all useful for testing. Liquid Web's roundup is blunt about the ceiling: free options come with strict caps on CPU, storage, network throughput and support response times, and production workloads need a paid plan. Evoxt has no free tier; its $2.99 VM-0.5 is the lowest-risk entry, not a free one.

**One vCPU runs out on dynamic sites.** Static pages and small caches cope fine. Anything with a database, cron jobs and concurrent admin sessions will queue on a single core, which is why the 2-core VM-1.5 exists at $6.95.

**Some things Evoxt does not advertise.** VPSBenchmarks' feature table records no DDoS protection, no hourly billing, no reverse DNS and a hidden CPU model, alongside 18 data centers across four continents, a REST API, VNC access and cloning. If volumetric DDoS mitigation or per-hour billing is a hard requirement, that is a reason to look at another provider rather than to expect it here.

## How Evoxt compares with other cheap cloud VPS

Prices below are entry-level figures in the currency each provider publishes. Billing periods differ, so treat this as a positioning table rather than a like-for-like quote.

| Provider | Entry price | Billing / policy notes |
| --- | --- | --- |
| IONOS | $2–$90/month | 10–640 GB SSD across the range; 99.9% uptime; backups cost extra |
| Vultr | $2.50/month | SSD instances, resource tuning across a wide range |
| Netcup | €3.35/month | 2 vCore, 2 GB RAM, 64 GB SSD at entry |
| Hetzner Cloud | €4.35/month | NVMe plus AMD EPYC, Germany, Finland and a US region |
| DigitalOcean | $4–$2,096/month | Hourly billing, free cloud firewall, **no refunds** |
| Hostinger | $4.99–$19.99/month | First 24 months; 30-day money-back guarantee; KVM |
| Liquid Web | $11/month upfront | Site headline says $5/month, prepay and yearly billing start at $11; 100% uptime SLA, HIPAA/PCI compliance |
| Evoxt | $2.99/month | 512 MB, 5 GB, weekly offsite backup included, monthly to 3-year prepay |

Who each one suits. DigitalOcean for developers who want hourly billing and a broad API ecosystem, accepting that it does not refund. Cloudzy for a 14-day money-back window, hourly billing and no credit card needed to reach SSH, though its pricing page displays two different annual discount figures (35% and 50%), so confirm the final number at checkout. Liquid Web when you need compliance certifications and a 100% uptime SLA and can pay five to ten times Evoxt's price. Hostinger for a 30-day refund and a friendlier panel at $4.99–$19.99 for the first 24 months. Evoxt sits at the low end on price with backups and a panel included, and gives up hourly billing and advertised DDoS protection to get there.

## Which plan to buy

- **Only testing, learning Linux, running a VPN or a bot:** VM-0.5 at $2.99. Nothing cheaper in the lineup makes sense, and 512 MB is enough for a single-purpose box.
- **One WordPress site or a small business page:** VM-1 at $5.99. 2 GB RAM and 20 GB storage match the published baseline for a small WordPress install.
- **WordPress with real traffic, or anything running a database plus workers:** VM-1.5 at $6.95 for the second core, or VM-2 at $11.99 if you also need the 30 GB disk.
- **WooCommerce or multiple sites:** VM-2 at $11.99 as the floor, VM-4 at $23.99 once you are running several stores or heavy plugins.

Before you pay, confirm three things on the order page: the price at renewal and how prepayment affects it, whether backups and the control panel are inside the quoted price (at Evoxt they are), and how long the refund window lasts. Those three answers decide whether the cheap plan stays cheap.

👉 [Deploy an Evoxt VM at the current monthly price](https://bit.ly/EvoXt)
