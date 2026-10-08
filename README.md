🔥 FIRE & FURY — Unleashed

FIRE & FURY is a browser-based action game project built around the theme of power, fury, rockets, survival, and historical-inspired Mysorean warfare.

Project file: Fire and fury unleashed.html

🎮 Features

🔐 Account-based login and sign-up

👤 Player profile and custom avatar support

🏆 Hall of Fame / leaderboard

🎖️ Achievements and progression

📜 Gameplay history

🚀 Rocket Battle

🌋 Volcano Rush

🔥 Final Fury

🎵 Separate background music for menus, battles, and Final Fury

💥 Rocket, explosion, rock-destruction, victory, and defeat sound effects

✨ Gameplay visual effects

📱 Mobile-friendly controls and responsive UI

🖥️ PC keyboard controls

🌐 Supabase-powered online scores and multiplayer infrastructure

🕹️ Game Modes

🚀 Rocket Battle

Fight British forces using Mysorean rockets and complete battlefield objectives.

🌋 Volcano Rush

Survive a volcanic environment while dealing with hazards and completing objectives.

🔥 Final Fury

A high-intensity mode combining combat and environmental hazards.

🔊 Audio

The game expects these local audio files:

sounds/
├── menu-bgm.mp3
├── battle-bgm.mp3
├── final-fury-bgm.mp3
├── rocket-launch.mp3
├── explosion.mp3
├── rock-destruction.mp3
├── victory.mp3
└── defeat.mp3

BGM routing

Area

Track

Home / menus / profile

menu-bgm.mp3

Rocket Battle

battle-bgm.mp3

Volcano Rush

battle-bgm.mp3

Final Fury

final-fury-bgm.mp3

Results screen

BGM stops

The game is designed so that only one background-music track is active at a time.

👤 Accounts & Online Features

FIRE & FURY uses Supabase for authenticated player accounts and online game data.

The browser build uses a publishable Supabase key. A service-role/secret key must never be placed in the HTML.

The project can use these online data areas:

profiles

scores

matches

match_players

match_requests

Custom avatars use a Supabase Storage bucket named:

avatars

Supported avatar formats:

PNG

JPEG

WebP

The configured upload limit is 1 MB.

📁 GitHub Setup

Keep the project structure like this:

Fire-and-Fury/
│
├── Fire and fury unleashed.html
├── logo.png
│
└── sounds/
    ├── menu-bgm.mp3
    ├── battle-bgm.mp3
    ├── final-fury-bgm.mp3
    ├── rocket-launch.mp3
    ├── explosion.mp3
    ├── rock-destruction.mp3
    ├── victory.mp3
    └── defeat.mp3

Important: the HTML references the files inside sounds/. Do not rename or move those files unless you also update the paths inside the HTML.

▶️ Running the Game

Because this is a browser project, the simplest approach is to publish the repository with GitHub Pages or another static web host.

GitHub Pages

Create a GitHub repository.

Upload:

Fire and fury unleashed.html

logo.png

the complete sounds/ folder

this README.md

Enable GitHub Pages in the repository settings.

Open the published site.

For local development, a simple static HTTP server is preferable to opening the HTML directly with file://, especially for online services and browser security restrictions.

🎯 Controls

PC

Use the on-screen controls where available, together with the game's keyboard controls.

Typical movement/combat controls include:

W / A / S / D — movement

Arrow keys — movement where supported

Space — fire where supported

Mouse/touch controls — depending on the active game interface

Mobile

The game provides touch-friendly controls for supported gameplay screens.

🏆 Progression

The achievement system includes early milestones such as:

🌱 First Spark — complete your first game

🎮 Regular Player — complete 5 games

🔥 Score Chaser — reach 1,000 points in one game

💎 High Scorer — reach 5,000 points in one game

🌟 Point Collector — earn 10,000 total points

More difficult achievement tiers can be added as the project evolves.

🧑‍💻 Technology

FIRE & FURY is primarily a client-side browser project using:

HTML

CSS

JavaScript

Canvas/game UI systems

Supabase JavaScript client

Supabase Authentication

Supabase Database

Supabase Storage

Web Audio / HTML5 audio

⚠️ Current Build Notes

This repository contains the current Fire and fury unleashed.html browser build and its supporting assets.

The project is actively developed. Some advanced systems—especially the long-term goal of a fully realized 3D battlefield experience—may continue to evolve.

Do not describe a feature as production-secure merely because the UI exists. Online authentication, multiplayer, account deletion, database policies, and storage policies should be verified in the actual Supabase project before treating them as production-ready.

🔒 Security Notes

Never commit a Supabase service_role key.

Never put database admin credentials in client-side JavaScript.

Use Row Level Security (RLS) for protected database data.

Validate permissions server-side through Supabase policies/RPCs.

Treat all browser-side game values as untrusted input.

📜 Credits

FIRE & FURY

A student game project focused on combining historical inspiration with fast-paced arcade combat, rockets, survival, and dramatic visual presentation.

🔥 Feel the fury. Launch the rocket. Take the battlefield.
