# ines

**Ines remembers how places felt, and curates where you'll feel that again.**

Ines is a voice-first travel curator. You tell her what you want to *feel*, like "a rainy afternoon, ceramics, natural wine, somewhere nobody's photographing." She answers with a few places chosen for you, not twenty ranked by stars.

Most travel AI learns from clicks and ratings. Ines learns from memories in your own words, like *"Felt small in a good way. The rain made everything sound closer."* No star rating captures that kind of taste signal.

## The idea

The app is a gallery.

- **Collection.** Past trips, saved as memories in your own words. Ines pulls taste notes from each one.
- **Exhibition.** The upcoming trip, arranged as numbered rooms (one per day). Each place has one line on why it's there for you.
- **Ines.** The curator. She speaks rarely and precisely, like a gallery docent.

## What the prototype does

- **Ask.** Type or dictate (Wispr Flow) into one field. Ines curates 3–5 places from your memories.
- **Weather rehang.** Thursday is too windy
cd ~/ines
cat > README.md <<'EOF'
# ines

**Ines remembers how places felt, and curates where you'll feel that again.**

Ines is a voice-first travel curator. You tell her what you want to *feel*, like "a rainy afternoon, ceramics, natural wine, somewhere nobody's photographing." She answers with a few places chosen for you, not twenty ranked by stars.

Most travel AI learns from clicks and ratings. Ines learns from memories in your own words, like *"Felt small in a good way. The rain made everything sound closer."* No star rating captures that kind of taste signal.

## The idea

The app is a gallery.

- **Collection.** Past trips, saved as memories in your own words. Ines pulls taste notes from each one.
- **Exhibition.** The upcoming trip, arranged as numbered rooms (one per day). Each place has one line on why it's there for you.
- **Ines.** The curator. She speaks rarely and precisely, like a gallery docent.

## What the prototype does

- **Ask.** Type or dictate (Wispr Flow) into one field. Ines curates 3–5 places from your memories.
- **Weather rehang.** Thursday is too windy for horseback riding, so Ines proposes moving it to Wednesday. She checks the 2-hour drive from the surf town, warns you to leave by 12:15, and drafts a message to the stables in European Portuguese for you to send on WhatsApp, SMS or WeChat.
- **Map.** Every place is pinned, with walk, transit and taxi times from your hotel. The cheap train route to the beach includes a pastry stop on the way.
- **Phrasebook.** Translations in big "show this" type, a dictionary of words you learned, and three phrases for each place.
- **Save.** Full-screen pieces in a dark, image-first layout.

The demo is a five-day trip to Lisbon. The memories, forecast, fares and images are illustrative.

## Run it

It's one self-contained file with no build step:

    open index.html

You can deploy it as a static site on Vercel or GitHub Pages. Live curation and translation run on Claude when the page is a Claude artifact. Anywhere else, every screen still works with sample responses.

## Roadmap

- **Voice:** Wispr Flow, with a Whisper fallback. Raw words are kept for memory placards.
- **Curation:** the Claude API, matching the request against your memories.
- **Places and routes:** Google Places, including search along a route, and Google Routes.
- **Map:** Mapbox, styled dark.
- **Weather:** WeatherKit or Open-Meteo, with limits per activity for wind, swell and rain.
- **Translation:** Google Cloud Translation.
- **Taste inputs:** YouTube liked videos, and a share-to-Ines action for TikToks.
- **Memory layer:** [What Stayed](https://whatstayed.vercel.app).

## Principles

1. **Restraint.** At most five pieces at a time.
2. **Feeling over ratings.** No stars and no review counts.
3. **Human in the loop.** Ines drafts messages and you send them.

---

Built by [Elizabeth Xu](https://github.com/elizabethxuu).
