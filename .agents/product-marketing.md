# Product Marketing Context

**Document version:** v1
**Last updated:** 2026-11-19

## Product Overview
**One-liner:** Televo is a free private messenger with chats on every device and Secret Chats that only two people can open.
**What it does:** Messaging, voice messages, groups and 1:1 voice/video calls on iPhone and Android. Regular chats live in the encrypted Televo cloud and sync to every device. Secret Chats are end-to-end encrypted on the phone, so Televo itself can't open them.
**Product category:** Private / secure messenger (shelf: "Telegram alternative", "private messenger", "encrypted messenger").
**Product type:** Consumer mobile app (iOS TestFlight beta, Android APK). Not yet in App Store / Google Play.
**Business model:** Free for personal 1:1 messaging. Possible paid extras for teams/power users later. No ads, no data selling.

## Target Audience
**Primary:** Russian- and English-speaking people (CIS diaspora, Uzbekistan, Spain/EU) who already use Telegram/WhatsApp and want more privacy without giving up convenience.
**Primary use case:** Talk to family and friends privately, including the occasional conversation that should never sit on any server.
**Jobs to be done:**
- "Let me message and call my people without ads or someone mining my data."
- "Give me one place for the really private conversation, without making my parents install Signal."
- "Keep my chats when I switch phones."
**Use cases:** family chat and calls abroad; medical/legal/money talk in a Secret Chat; disappearing messages; groups.

## Problems & Pain Points
**Core problem:** Big messengers are either convenient but ad/data driven, or private but awkward for non-technical family.
**Why alternatives fall short:**
- WhatsApp: owned by an ad company, metadata feeds Meta.
- Telegram: cloud chats are the default and Secret Chats are hidden; no voice/video in Secret Chats; many people don't know the difference.
- Signal: private but feels empty and technical to many families; no cloud history.
**Emotional tension:** "Who else is reading this?" — distrust, not knowing.

## Competitive Landscape
**Direct:** Telegram, WhatsApp, Signal.
**Secondary:** iMessage/FaceTime (Apple-only), Viber.
**Indirect:** phone calls/SMS.

## Differentiation
- Two clearly labelled kinds of chat, and a plain answer to "who can read this?" for each.
- Secret Chats use post-quantum key exchange (X25519 + ML-KEM-768) — ahead of Telegram; comparable to Signal's PQXDH.
- Warns and pauses sending if a contact's key changes.
- Open source code to read.
- Calls ring like normal phone calls (CallKit), Picture-in-Picture.
- No ads, ever.

## Objections
| Objection | Response |
|-----------|----------|
| "Can you read my messages?" | Secret Chats: no, it's impossible for us. Regular chats: encrypted in our cloud with AES-256, key kept in a separate vault, never used for ads, never shared. For anything sensitive, tap the lock. |
| "Nobody I know uses it." | Free, installs in a minute, works on iPhone and Android; invite links. |
| "New app — will it disappear / is it safe?" | Code is public; beta is open; [NEED: independent audit before claiming "audited"]. |
| "Not in App Store yet" | TestFlight is Apple's own beta app; App Store release pending review. |

**Anti-persona:** people who need anonymity from a state-level adversary with metadata analysis (we see who talks to whom); enterprises needing compliance archives.

## Switching Dynamics
**Push:** ads, Meta ownership, uncertainty about who reads chats.
**Pull:** honest privacy, Secret Chats with calls-quality UX, no ads.
**Habit:** everyone's already on Telegram/WhatsApp.
**Anxiety:** losing history, friends not there, beta bugs.

## Customer Language
**Words to use:** private, only you two, lock, secret chat, your phone, every device, no ads, free, calls.
**Words to avoid on the homepage:** XSalsa20, ML-KEM, DTLS, TURN, "at rest", "metadata", "oracle" — keep them for the "for the curious" block and FAQ. Avoid "military-grade", "unhackable", "100% secure".
**Never claim:** that Televo can't read regular chats; that the code is audited; user counts or reviews we don't have.
**Glossary:**
| Term | Meaning |
|------|---------|
| Regular chat (cloud chat) | Synced, AES-256 encrypted on our servers, key in a separate vault |
| Secret Chat | End-to-end encrypted on the phone; Televo can't open it |
| Safety number | Code two people compare to confirm no one is in the middle |

## Brand Voice
| Attribute | Means | Doesn't mean | Example line |
|-----------|-------|--------------|--------------|
| Plain | Short words a parent understands | Dumbed down or vague | "Only you two can open it." |
| Honest | Says what we can't do too | Self-deprecating, alarmist | "Not on the App Store yet." |
| Warm | Real moments: family, a call home | Cute, emoji-heavy | "You call your mom on a Tuesday." |

**Tone by context:** Support: calm, step-by-step. Launch: confident, specific. Errors: what happened + what to do.

## Proof Points
**Metrics:** none public yet [NEED: beta user count, ratings once in App Store].
**Value themes:**
| Theme | Proof |
|-------|-------|
| Private by choice | Secret Chats E2E, post-quantum, code public |
| Easy | Works like Telegram: cloud sync, groups, calls |
| No business in your data | No ads, no SDK trackers, privacy policy |

## Goals
**Business goal:** Grow beta users and pass App Store review.
**Conversion action:** Install (TestFlight on iPhone / APK on Android); secondary: email waitlist.

## Learnings
| Date | Learning | Evidence | Applies to | Status |
|------|----------|----------|------------|--------|
| 2026-11-19 | Don't lead with "we can technically read regular chats" — founder rejected it as wrong marketing. Describe cloud protection positively (AES-256, separate key vault, no ads, never shared) and keep the full honest detail in FAQ/Privacy Policy. | Founder feedback | site, App Store, social | active |
| 2026-11-19 | Visitors won't read crypto detail; homepage must be understandable without it. | Founder feedback | site | active |

## Changelog
- v1 (2026-11-19) — Initial context, auto-drafted from the site, app and privacy policy.
