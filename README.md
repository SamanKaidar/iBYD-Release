# iBYD Releases

All notable changes, new features, and improvements to **iBYD** are documented in this file.

## [v0.25-beta] - 2026-10-07

### 🧭 Navigation and windshield display (HUD): now Google Maps and Waze

- **The HUD now works with Google Maps and Waze.** Start a route in either app and the windshield shows the next turn arrow, the distance to it, the street name, and the time and distance left. The arrow is the navigation app's own picture, so it is right in every language, at roundabouts and at exits.
- **Fix: roundabouts.** The glass sometimes showed a left-turn arrow at a roundabout. It now shows the roundabout and the exit to take.
- **Fix:** the arrow no longer disappears while you wait at a long red light.
- **Fix:** when you end the route, the windshield clears within a few seconds (it could keep the last arrow for up to 90 seconds).
- **The HUD card now says what is happening:** Connected, Connecting, "This car has no factory HUD", "Could not connect", or that an activated licence is needed. Before, the switch looked the same whether it worked or not.
- The remaining time on the windshield now reads "1 h 05 min" instead of "01:05 min".
- The speed-limit sign on the HUD is removed: Google Maps and Waze do not share the speed limit with other apps.
- **Voice:** "what is my next turn", "how far is it" and "when do we arrive" now answer from Google Maps or Waze, including the battery you will have left on arrival. "Open maps", "open navigation" and "open Waze" open those apps.

### 📻 Radio

- **Fix: the steering wheel buttons now control the radio.** Next and previous change the station, play/pause pauses and resumes. The station name can also appear on the car's media display.
- Starting the radio now pauses other music apps instead of playing over them. Google Maps voice prompts lower the radio briefly, and after a phone call the radio continues.

### 🎵 Music

- **The Music automation and voice command now work with the music app you use:** Spotify, YouTube Music, Anghami, Apple Music, Deezer and others. "Play music" resumes your music; "play Fairuz" asks your music app to play it (apps that cannot do that open their search instead).
- Your saved automations that used Yandex Music keep working: they now resume your music app.

### ☁️ BYD cloud (Tweaks)

- **New: "Keep online while parked".** Keeps the car showing online in the BYD phone app while it is parked: it reconnects to the BYD cloud every few minutes, restarts wifi when it gets stuck, and **turns wifi off if the 12 V battery drops below 12.4 V** (it comes back on by itself when you start the car). Switching it off removes it completely from the car.
- **New: "Wifi while parked only when charging".** With the car off, wifi stays on only while the charging cable is plugged in.
- The card shows the last check: time, 12 V battery voltage, car on/off, and the last thing it did.
- After the car restarts, open the BYD cloud card once to start it again.

### 🎙️ Voice calibration

- **Calibration now really tunes the assistant.** It listens with the same offline speech engine your commands use (before, it used a different engine, which is why the right sentence often failed), and it measures how long you pause between words. Commands then end after a pause that fits the way you speak, so you are not cut off mid-sentence.
- Please **run Voice Calibration once more**: older results are reset, because they came from the wrong engine.

### 🖥️ Screens and split screen

- **Fix: the 360 / reverse camera closed by itself** when you shifted to R while the dashboard showed an app in its split pane. The camera now stays open.
- An app that runs on the dashboard no longer appears when you pick apps for the split screen, and the other way round. The same app cannot run in two places at once, and picking it twice made one of them restart or go black.
- Blind-spot cameras: choosing **Driver Cluster** now shows the floating windows (with the speedometer still visible) straight away. The extra "Full Screen / Floating PiP" choice is gone.

### 🎨 Look

- **New clock styles** on the dashboard: **Minimal**, **Activity Rings**, **Flip Clock** and **Day Timeline**. Swipe the clock or tap its style name to switch.
- The button at the top left that hides and shows the side bar has a new icon that shows what it will do: collapse the side bar, or bring it back.

### 📦 Download
- **APK**: [iBYD-v0.25-beta.apk](iBYD-v0.25-beta.apk)
- **SHA-256**: `12299a40d247bfd08171ddd84bb5b7bbc13f7af621e4b443fccae7ae6cf950a2`
