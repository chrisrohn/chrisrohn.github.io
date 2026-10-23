# Training & Recovery: the old address

The installable training app and cycling computer now lives at **<https://chris.bike/>**
([chrisrohn/chris.bike](https://github.com/chrisrohn/chris.bike)).

This site was its home, so it still forwards there: every page (and every old QR link or home-screen shortcut)
carries what the phone kept here (the GitHub connection, settings, routes, rides) to chris.bike in the link's
`#fragment`, then opens the app there. Until chris.bike answers, it keeps serving the app itself ("standby"), so the
switch happens by itself on the first hourly deploy after the domain is live.

Nothing here is edited by hand: `.github/workflows/deploy.yml` builds it from
[chrisrohn/chrisrohn](https://github.com/chrisrohn/chrisrohn) (`fitness/`, `node fitness/build-app.mjs --role`)
every hour when that changes, and on demand (*Actions → Deploy the Training app → Run workflow*). It holds no one's
data. See [fitness/README.md](https://github.com/chrisrohn/chrisrohn/blob/main/fitness/README.md#the-app-on-your-phone).
