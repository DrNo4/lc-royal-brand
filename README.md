# LC Royal Brand

Website for Christian Sierra's home and property business. The pages are plain files. There is no build step and no packages.

This repository is the source. A copy is already on Netlify. To make a change, edit the files here and get that change onto the Netlify site (connect this repo in Netlify, or upload the folder again).

Open `index.html` in a browser, or from this folder run:

Open `index.html` in a browser, or from this folder run:

```bash
python3 -m http.server 8765
```

Then visit http://127.0.0.1:8765

## Before this is sent to customers

- The reviews in the Reviews section are samples. Replace them with real client words.
- The pictures in `images/` are stand-ins. Replace each file and keep the same file name.
- `index.html` has `<meta name="robots" content="noindex, nofollow">`. Remove that line when the real site should show up on Google.
- There is no email on the site yet, so the only action is a phone call or a text to (737) 391-6968.
- Insurance, license, and a headshot are not on the page. Add them when Christian confirms the details.

## Change the phone number

Search `index.html` for `737` and update both the visible number and the `tel:+17373916968` / `sms:+17373916968` links.

## Put it online

A Netlify site already exists from a folder upload. The address ends in `.netlify.app`.

To make later edits show up on that address, connect this GitHub repo once:

1. In Netlify, open the site, then Site configuration, then Build & deploy, then Link repository.
2. Choose this repo. Build command: leave empty. Publish directory: `.` (the top of the repo).
3. After that, every update on GitHub publishes the site.

When a domain is ready: Domain management, then Add a domain. Netlify shows the DNS records. Add those at the company that sold the domain. HTTPS turns on by itself. This often takes an hour, sometimes a day.

The folder can also be uploaded again at https://app.netlify.com/drop if the repo is not linked yet. `index.html` has to stay at the top of the folder.

The same folder also works on Vercel (import the folder or a GitHub repo), GitHub Pages, or any host with a public web folder. Upload the contents so `index.html` is in the web root. Point the domain at that host the way their screen tells you to.

Do not put this site inside another app's folder on a server. It is its own site.
