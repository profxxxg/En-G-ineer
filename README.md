# En-G-ineer
En-G-ineer: Origin Story

An interactive engineering portfolio, disguised as a retro NES game.

Play through five years of Mechatronics Engineering — one level per year — collecting
course "keys," choosing a branch and specialization, and finally facing my own
graduation project (an 18-DOF hexapod robot) as the final boss. It ends in a trophy
gallery of real projects and a hire-me screen.

Play it here ← replace with your live GitHub Pages / Netlify link


Why this exists

A PDF resume tells you what I did. This shows how I think, what I actually shipped,
and — hopefully — that I can make something a little unexpected and finish it
properly. Five minutes, no download, works on desktop and mobile.

How to play

ActionDesktopMobileMoveArrow keys / WASDOn-screen D-padInteract / advance dialogueSpace or EnterACT buttonMute / adjust volumeSlider in the top bar, or MSlider in the top barSkip everything"Skip to Gallery" button (always visible)Same

Walk up to a course booth and interact to read what it taught me and collect its key.
Collect every key in a level to open the door to the next year. Two branch-point
quizzes let you pick the same path I did (or take the joke answers first).

Tech


Single self-contained .html file — no build step, no dependencies, no
network calls. Opens straight from disk or any static host.
Canvas 2D, rendered at a fixed internal resolution of 256×240 (authentic
NES) and scaled up crisp with image-rendering: pixelated.
All audio is synthesized live with the Web Audio API — chiptune melodies,
a distinct musical theme per level, and sound effects. No audio files.
All images are embedded as base64 — real project photos and CAD renders,
shown in-frame like exhibits; the only pixelated element is my own sprite/portrait.
Runs entirely client-side. No tracking, no cookies, no backend.


Project structure

en-g-ineer.html   ← the entire game (markup, styles, engine, content, assets)
README.md         ← this file

Everything lives in one file on purpose — it's meant to be forkable, inspectable,
and trivially hostable anywhere that serves static files.

Running it locally

Just open en-g-ineer.html in a browser. That's the whole setup.

bashgit clone https://github.com/<your-username>/en-g-ineer.git
cd en-g-ineer
open en-g-ineer.html   # or just double-click it

Deployment

Currently hosted on [GitHub Pages / Netlify — pick one]. Since it's a single
static file, it can be redeployed anywhere (Vercel, Cloudflare Pages, S3, etc.)
by uploading en-g-ineer.html and, if the host expects it, renaming it to
index.html.

The real projects behind the game


Hexapod Agricultural Robot — 18-DOF autonomous six-legged robot for
mango-field disease prevention. ROS + reinforcement-learning gait, full
IMU/LiDAR/GPS/camera suite. Team lead of 7. Grade A+.
Automated Vision-Guided Conveyor System — 4-stage line: feed → vision
recognition → sorting → robotic-arm assembly.
Off-Grid Micro-Hydro Water Turbine — ANSYS CFD/FEA-validated low-flow
turbine design.
Plus an autonomous RC car, a pneumatic robotic arm, DC motor system
identification, and a computational intelligence / ML pipeline.


The gallery in-game is a highlight reel, not the full list — there's more I'm
happy to talk through in an interview.

Contact

George Megally Girgis — Mechatronics Engineer, Dublin, Ireland
📧 george7megally@gmail.com
💼 linkedin.com/in/george-megally-girgis


Built with a lot of trial, error, and Claude.
