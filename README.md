# 🎼 Note Exerciser

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/simelab)

A free, offline, ad-free app to practice reading sheet music. Most note-reading apps are limited — Note Exerciser packs every feature and customization into a single page.

## Features

- **4 clefs** — treble, bass, alto, tenor
- **Custom note range** — pick the lowest and highest note you want to drill
- **6 answer modes**
  - Buttons · Solfège (Do Re Mi) or Letters (C D E F G A B)
  - Microphone · sing or play a real instrument; pitch is detected with autocorrelation
    - *relative* mode: any octave of the right pitch class counts
    - *exact* mode: match the exact octave shown on the staff
  - On-screen piano · two octaves with black keys and optional key labels
- **Smart practice**
  - *Repeat mistakes* — notes you miss come back more often (weighted roulette)
  - *Big leaps* — biases selection toward larger intervals to train ledger-line reading
- **Audio feedback** — hear the target note, a success arpeggio, or a buzz on mistakes (Web Audio API)
- **Streak & score tracking**, keyboard shortcuts (1–7), collapsible settings during play

## Run it

No build step needed: open `www/index.html` in any browser. Everything works offline.

## Android

The Android app wraps the same page with [Capacitor](https://capacitorjs.com):

```bash
npm install
npx cap sync android
cd android && ./gradlew assembleDebug
```

Requires JDK 21 and the Android SDK (`ANDROID_HOME`).

## Support ☕

If Note Exerciser helps you, consider [buying me a coffee](https://ko-fi.com/simelab). Donations keep the app free, ad-free and open.
