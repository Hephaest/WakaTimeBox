<p align="center">
  <img width="400" src="https://user-images.githubusercontent.com/37981444/103776754-c4556280-4fe4-11eb-98da-7ed25df2d088.png">
  <h3 align="center">WakaTimeBox</h3>
  <p align="center">Update a pinned gist to contain your weekly WakaTime stats</p>
</p>

---

> 📌✨ For more pinned-gist projects like this one, check out: https://github.com/matchai/awesome-pinned-gists

## Special Thanks

This repo is cloned from [waka-box](https://github.com/matchai/waka-box), and I only made some improvements.

## What's New

- Update dependency `axios` to `0.21.1`.
- Fix the bug from language layout.

## Setup

### Prep work

1. Create a new public GitHub Gist (https://gist.github.com/)
2. Create a token with the `gist` scope and copy it. (https://github.com/settings/tokens/new)
3. Create a WakaTime account (https://wakatime.com/signup)
4. In your WakaTime profile settings (https://wakatime.com/settings/profile) ensure `Display coding activity publicly` and `Display languages, editors, operating systems publicly` are checked.
5. In your account settings, copy the existing WakaTime API Key (https://wakatime.com/settings/api-key)

### Project setup

1. Fork this repo
2. Edit the [environment variable](https://github.com/matchai/waka-box/blob/master/.github/workflows/schedule.yml#L13-L15) in `.github/workflows/schedule.yml`.
3. Go to the repo **Settings > Secrets**
4. Add the following environment variables:
   - **GH_TOKEN:** The GitHub token generated above.
   - **WAKATIME_API_KEY:** The API key for your WakaTime account.
   - **GIST_ID:** The ID portion from your gist url: `https://gist.github.com/matchai/`**`6d5f84419863089a167387da62dd7081`**.
