# Training & Recovery

The installable training app and cycling computer, served at **<https://chrisrohn.github.io/>**.

It lives at its own address, apart from the music app at chrisrohn.com, so Android installs it as an app of its own.
Nothing here is edited by hand: `.github/workflows/deploy.yml` asks
[chrisrohn/chrisrohn](https://github.com/chrisrohn/chrisrohn) (`node fitness/build-app.mjs --role`) what this site
serves (*app* while `[app] url` in `fitness/config.toml` is this address), builds it from `fitness/` every hour when
that changes, and on demand (*Actions → Deploy the Training app → Run workflow*). It holds no one's data. The old
address chrisrohn.com/fitness/ forwards here and brings each phone's data along (`move.html`). See
[fitness/README.md](https://github.com/chrisrohn/chrisrohn/blob/main/fitness/README.md#the-app-on-your-phone).
