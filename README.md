# 👀 LookVer Versioning 👀

## Summary

Given a version number METEOR.WAVE.DRIFT, increment the:

1. METEOR version when you make massive changes that demand attention
1. WAVE version when you make significant changes that you would like users to be aware of
1. DRIFT version when you make small changes that can go completely unnoticed

## The Inspiration

Of course this is heavily inspired by the versioning that came before...

- [SemVer](https://semver.org) `MAJOR.MINOR.PATCH`
- [PrideVer](https://pridever.org/) `PROUD.DEFAULT.SHAME`
- [RomVer](https://github.com/romversioning/romver) `PROJECT.MAJOR.MINOR`

## The User Focus

This versioning scheme is focused on **attention** and **focus**. The quality that distinguishes the
three numerical segments is how much attention the general user of your software should pay to the
release. LookVer assumes your users are ordinary people that have constraints on how much attention they can give to their software releases, and so it seeks to answer the question *should your users LOOK at the release notes?*

This versioning does *not* focus on "breaking changes" or API stability, so might not be suited for software projects that are primarily used by other software developers, and that become dependencies in other projects. It works best for projects where the changes are *pushed* to your users (i.e., your app is deployed), rather than requiring your users pull the new release down on their own.

## The Three Segments

### ☄️ `METEOR` . 🌊 `WAVE` . ☁️ `DRIFT`

- The `METEOR` release **demands attention**. It is appropriately massive, has many new features, breaking changes, new interfaces to learn, and new APIs. This signifies to users that "this is the new generation of the product", or "this is going to feel like a new system".  The developers and product folk probably feel a lot of pride in the release, and if you have a sales team, they're very excited.
	- This includes RomVer's `PROJECT`, but does not need to involve evolving into a new project. Like `PROJECT`, it is OK if you never bump this version.
	- Overlaps with PrideVer's `PROUD` ("proud of the release"), and SemVer's `MAJOR`.
	- Communication: Alert your users ahead of time and give them time to prepare. Make sure they know when the release arrives.
	- Cadence: Use this sparingly, e.g., once per year, maybe never.

- A `WAVE` release is something to look at, something that **should be noticed**. Waves can come in a variety of sizes -- some scary, some gentle -- but regardless, some communication to the users is suggested, and some of their attention is hoped for. You want your users to be aware of the release, and maybe even look through the release notes. They might expect changes to their workflows, or they might be pleased to find a new feature. People are busy, so it is possible your users ignore any release communication; if they do, it shouldn't be catastrophic.
	- This can overlap with PrideVer's `DEFAULT` ("just normal/okay releases"), or `PROUD`.
	- Any breaking changes that would be in SemVer or RomVer's `MAJOR` could fall into this release if they are not massive enough to be `METEOR`.
	- A `MINOR` ("non-breaking") change that is particularly impactful could fall into this category.
	- Communication: Let your users know about the release -- maybe in an email or a message within your software. If it's a relatively impactful wave, then let your users know ahead of time.
	- Cadence: Release these are often as you would like, but keep in mind that if they are too frequent, your users will pay less and less attention. Once a month or once every few weeks might be a good cadence.

- A `DRIFT` is small, stealth release that **does not need attention**. Things are changing, but it is a gentle movement for the software. You are safe to drift along. There might be a few users who care about a certain bug being fixed, or a minor feature, but otherwise it is perfectly OK if no one even notices this release happened.
	- This includes PrideVer's `SHAME` ("fixing things too embarassing to admit"), but could also overlap with PrideVer's `DEFAULT`.
	- It includes changes that would fall into SemVer's `PATCH`, and could include particularly small `MINOR` releases.
	- Communication: Some details in a release log are sufficient. No one will read them.
	- Cadence: Release these are frequently as you want.

### Alternate names that get to the same concept...

😲👀 `You must look at me!` . 😐 `Please take a look` . 😴 `Safe to ignore`

```
| MASSIVE | SIGNIFICANT |  SMALL  |
|  QUAKE  |    SHIFT    |  DRIFT  |
| TORNADO |   THUNDER   |  MIST   |
|  FLARE  |    LOOK     | STEALTH |
|  SIREN  |   SIGNAL    | SILENT  |
```

## The Zero Version

Like SemVer, LookVer treats anything with a first segment (`METEOR`) of `0` ("Zero Versions") a little differently. Zero Versions can be expected to have relatively massive changes in their `WAVE` releases. Imagine a primordial sea, churning as the world takes shape.

Incrementing from the final Zero version `0.x.y` to `1.0.0` does not need to be a massive change. The `1.0.0` release is an acknowledgement that the software has taken its "final shape" (for now).

## License

[Creative Commons Attribution 4.0 International](https://creativecommons.org/licenses/by/4.0/)

Written (sans LLM) by Luke Nickerson
