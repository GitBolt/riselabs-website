# RISE Labs website: project notes

Hosting, domain, accounts, and what we still need to decide. For how to edit the site, see `README.md`.

## Where things stand

| What | Status |
| --- | --- |
| Website code | Done as a starter. Plain HTML and CSS, 7 pages. |
| Code storage | GitHub, under Aabis's account: https://github.com/GitBolt/riselab-website |
| Hosting | Vercel, account under Prof. Gonzalez (to set up) |
| Domain | TBD (see options below) |
| Live link | TBD |
| Content and photos | Mostly drafts and placeholders |


## Where the code lives

The code is on **GitHub** under Aabis's account: https://github.com/GitBolt/riselab-website

Anyone who will edit the site gets added as a collaborator on the repo. The repo can be moved to another account later without losing anything.

## Hosting

**Vercel**, with the account under Prof. Gonzalez so it stays with the lab.

- Vercel connects to the GitHub repo and publishes the site. Changes pushed to GitHub go live automatically.
- It gives us a free temporary link right away, and supports a custom domain with HTTPS.
- Heads-up: on the free "Hobby" plan, Vercel only auto-publishes changes pushed by the account owner. Since students will be making the edits, we will either need the Pro plan (about $20 per person per month) or someone with access to the account to publish updates. We can sort this out when setting up the account.

Decision needed: Prof. Gonzalez creates the Vercel account. Free plan or Pro?

## Domain

Two paths:

**A. An illinois.edu address**
- Free and looks official.
- Needs approval. Ask the AE department or Engineering IT whether lab sites can get one and what the process is.
- The university controls the settings, so changes go through them.

**B. Our own domain** (for example from Namecheap)
- About $10–20 a year.
- We control it fully.
- Someone has to pay for it and renew it every year. It should be on an account the lab keeps long term, not a student's personal account.

Name ideas: TBD. Check availability before deciding. This depends on the lab name and logo being confirmed (Luke).

Decision needed: which path, the exact name, and who pays.

## To finalize in the email

- [ ] Domain: illinois.edu address or our own domain?
- [ ] Domain name
- [ ] Who pays for and owns the domain
- [ ] Vercel account under Prof. Gonzalez: free plan or Pro?
- [ ] Lab name and logo confirmed with the university (Luke)
- [ ] Who writes the text for each page (About us, PEARL, SPIRIT, Student collaboration, Sponsorships, Join the team)
- [ ] Photos: high-quality landscape photos, professional headshots, and RISE Labs polos for the photos (from the email thread)
- [ ] A short CAD spin video for the home page

## Launch steps

1. Push the code to GitHub and add collaborators. (Done: https://github.com/GitBolt/riselab-website)
2. Prof. Gonzalez creates a Vercel account. Connect it to the GitHub repo. We get a temporary link right away.
3. Share the temporary link with Prof. Gonzalez, Luke and the team for review.
4. Fill in the content: replace draft text, add photos, add the logo.
5. Buy or request the domain and point it at the hosting. The hosting provider shows which records to add.
6. Delete the `<meta name="robots" content="noindex">` line from every page so search engines can find the site.
7. Share the final link.

## Costs

| Item | Cost |
| --- | --- |
| GitHub | Free |
| Vercel hosting | Free (Hobby), or about $20 per person per month (Pro) |
| Domain | Free for illinois.edu, or about $10–20 a year from Namecheap |
| Fonts (Google Fonts) | Free |
