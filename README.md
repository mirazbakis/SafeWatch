# SafeWatch

Videos without the doomscroll. Install page: **https://mirazbakis.github.io/SafeWatch/**

This repository only holds the install page, the DNS profile and the OTA signing setup.
`.github/workflows/sign-ota.yml` signs `ipa/SafeWatch.ipa` once per cert pack in
`signing/certs/<N>/` (as `com.mirazbakis.safewatch<N>`) and deploys `site/` to GitHub Pages.

To ship a new build, replace `ipa/SafeWatch.ipa` with a new unsigned IPA and push.
