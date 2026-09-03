# Privacy Policy — Cristina's Broom

**Last updated: 3 September 2026**

This policy covers the Android game **Cristina's Broom** (package
`io.github.muresania.skyward`), referred to below as "the game".

It is written from the game's actual behaviour rather than from a template, and it is
kept in the game's source repository next to the engineering record it describes, so
that the two cannot drift apart.

---

## The short version

- **We collect nothing.** The game has no account, no sign-in, no analytics and no crash
reporter, and it sends nothing to any server we control. We do not operate a server.
- **Your progress stays on your device**, in the game's own private storage.
- **The game shows optional rewarded video adverts**, supplied by Google's Mobile Ads
SDK. Google collects some data when an advert is requested or shown. That is the only
data that leaves your device because of the game, and it is described in full below.
- **The game is treated as child-directed.** Adverts are non-personalised, and the
Android advertising identifier is not transmitted.
- **Watching an advert is always optional.** Nothing in the game is locked behind one.

---

## What the game stores on your device

The game saves your progress and settings in its own private storage
(`files/datastore/skyward.preferences_pb`). No other app can read it. It is never
transmitted to us, and we could not read it if we wanted to.

That file holds eleven values, and this is all of them:

| What | Why |
|---|---|
| Best score | To show your record |
| Coin balance | The in-game currency, earned by playing |
| Owned cosmetic items | So purchases persist |
| Equipped hat, broom, cape and familiar | So your chosen look persists |
| Reduced motion, haptics, sound effects, ambience | Your four settings toggles |

**None of it identifies you.** There is no name, no email address, no account, no device
identifier and nothing derived from one. Nothing stored can tell one player from another
except by how good they are at the game.

**Coins cannot be bought.** They are earned by playing and there is no purchase path, so
the game holds no payment information of any kind.

### Backup to your own Google Drive

Android's Auto Backup is enabled for this file, which is the standard Android feature
that restores your apps when you move to a new phone. When it runs, the file above is
copied to **your own Google Drive**, under **your own Google account**, governed by
Google's terms and privacy policy.

**It does not come to us.** We have no access to your Drive and no way to read a backup.
The game has no code that could receive one.

You can turn this off in Android's own settings (Settings → Google → Backup), or delete
the backup from your Google account at any time.

---

## What the advert supplier collects

The game shows **rewarded video adverts only** — the kind you choose to watch in exchange
for in-game coins. There are no banners, no interstitials and no adverts during or
immediately after a run.

Adverts are supplied by the **Google Mobile Ads SDK**. When an advert is requested or
shown, Google collects and shares the following. This list is Google's own published
disclosure for that SDK, not our summary of it:

| Data | Category | Collected | Shared | Purpose |
|---|---|---|---|---|
| IP address | Approximate location | Yes | Yes | Advertising, analytics, fraud prevention |
| Interactions — app launches, taps, video views | App activity | Yes | Yes | Advertising, analytics, fraud prevention |
| Performance data — launch time, hang rate, energy use | Diagnostics | Yes | Yes | Analytics |
| App Set ID | Device or other identifiers | Yes | Yes | Advertising, analytics, fraud prevention |

All of it is sent over an encrypted connection (TLS).

**We never see any of it.** It goes from your device to Google. We receive no reports
containing it and hold none of it ourselves.

### The advertising identifier is not transmitted

The game is configured as **child-directed** for every player, with no age gate and no
alternative path. That has three consequences, and they apply to everybody:

- **Adverts are non-personalised.** They are not based on your interests or on a profile
of you.
- **The Android advertising identifier (AAID) is not transmitted.** The permission that
would allow it is removed from the app at build time.
- **Remarketing and third-party ad vendors are disabled.**

We chose this knowing it earns less. Non-personalised adverts pay materially lower rates.

### About the App Set ID

The App Set ID is a Google Play identifier scoped to apps published by the same
developer. It is not the advertising identifier and cannot be used to identify you
personally or to follow you across other developers' apps.

Per Google's documentation, it is reset when any of the following happens:

- the last app from that developer is uninstalled from the device;
- the device is factory reset;
- the identifier has not been accessed for over 13 months.

---

## Permissions the game uses

| Permission | Why |
|---|---|
| `INTERNET` | Required by the Mobile Ads SDK to request adverts. The game makes no network requests of its own |
| `VIBRATE` | A short buzz when a run ends. Can be turned off in Settings |
| `ACCESS_NETWORK_STATE`, `WAKE_LOCK`, `FOREGROUND_SERVICE` | Added automatically by Google's advert libraries. Not requested by us and not used by the game |

The game does **not** request access to your location, camera, microphone, contacts,
photos, files, or any other personal data on your device. It has no permission to do so.

---

## Deleting your data

**On your device.** Uninstalling the game deletes its storage, including your best score,
coins and cosmetics. There is no separate step, and nothing survives the uninstall on
your device.

**With us.** There is nothing to delete. We operate no server, hold no account and
receive no data from the game, so we have no record of you to remove and no deletion
request to process.

**Advert data held by Google.** Because we never receive it, we cannot delete it for you.
You can act on it directly:

- **Reset the App Set ID** by uninstalling the game — if it is the only app of ours on
the device, that resets the identifier, as described above.
- **Google's own controls** at [myaccount.google.com](https://myaccount.google.com) cover
the data Google holds, including activity and advert settings.
- **Delete your backup** from your Google account if you have used Android Auto Backup.

---

## Children

The game is suitable for children and is treated as child-directed for all users. We
collect no personal information from anyone, so there is no parental consent to obtain
and no child's data for us to hold.

If you are a parent and have a question about this, please use the contact address below.

---

## Changes to this policy

If the game's behaviour changes — a new library, a new stored field, a different advert
format — this policy is updated in the same change that causes it, and the date at the
top is updated with it.

---

## Contact

Questions about this policy, or about the game and your data:

**muresania.dev@gmail.com**

This address exists for this purpose. It is not used to contact players, and the game
has no way to obtain your address in the first place.
