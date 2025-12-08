---
title: "Donate+ — Blood Donation Network"
permalink: /projects/donate-plus/
---

## Overview

An Android app that **connects blood donors with recipients**. Users post requests, get responses, view nearby hospitals/blood banks, and navigate with **Google Maps/Places**—all backed by **Firebase authentication and realtime data**.

**Repo**: [github.com/faiazamin/Donate_plus](https://github.com/faiazamin/Donate_plus)

## Why?
Finding a matching donor quickly is often blocked by fragmented communication and poor location coordination. Donate+ compresses the search: one request fans out to verified responders and surfaces map-ready locations so seekers can act fast.

## Problem

- Hard to match **blood group + proximity** without a dedicated network.
- Donor intent drops when requests lack clear status/feedback loops.
- Seeker workflows are clumsy: collecting info, calling hospitals, and sharing locations happen across different apps.

## Approach

- **Request lifecycle**: Seekers post with blood group, required date, contact, and pinned map location; responders reply and are tracked in a dedicated list.
- **Contextual UI**: News Feed highlights urgent cases; detailed views show maps, contact chips, and response status.
- **Feedback + accountability**: Seekers can mark responders as called/enlisted, add notes, and review responses.
- **Location layer**: Map picker, GPS shortcuts, and map view for any post, hospital, or blood bank.
- **Notifications stream** filtered by the user’s blood group to keep signals relevant.

## Key Features

- Email/password sign-up, login, verification, and password reset.
- Profile management with blood group, contact details, and last donation date.
- News Feed of blood requests with urgency highlighting and detailed drill-down.
- Create/track requests; manage **My Posts** and **My Responses** dashboards.
- Respond to requests and appear in the seeker’s notification/responder list.
- Hospital & Blood Bank directory with tap-to-call and map view.
- Map support for address picking or viewing a post’s location.
- Settings screen with profile updates and logout.

## Tech Stack

- **Android (Java)**, minSdk 19, targetSdk 28.
- **Firebase**: Auth, Realtime Database, Analytics.
- **Google Play Services**: Maps, Places, Location.
- **UI**: AndroidX AppCompat/ConstraintLayout/Material Components, RecyclerView.

## My Contributions

- Defined the end-to-end donor/recipient flow and response tracking model.
- Built Firebase-backed auth, profile management, and news feed/posting features.
- Integrated Google Maps/Places for request locations and hospital directory.
- Shipped dashboards (My Posts/My Responses), blood-group-filtered notifications, and responder status updates.
- Produced release builds and setup guidance (google-services, map keys, Gradle tasks).

## Setup & Run

- Add `google-services.json` under `app/` and supply a Maps/Places API key in `app/src/main/res/values/map_key.xml`.
- Build with `./gradlew clean assembleDebug`; install the APK from `app/build/outputs/apk/debug/`.
- Requires Android 28 platform tools, JDK 8+, and location permissions on device/emulator.

## Impact

- Creates a single workflow for urgent blood requests with location-aware responses.
- Improves responder accountability via enlist/called notes and seeker notifications.
- Delivers a ready-to-install APK (`app/release/app-release.apk`) for rapid pilot use.
