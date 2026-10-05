# Happy Birthday

A personalised birthday surprise you can send as a link. A cartoon door opens, balloons float out, and the viewer walks into a party room packed with balloons. They pop one by one (or tap them yourself) until the room is clear, friends jump up from behind the table shouting "SURPRISE!!", and a cake with one lit candle per year appears while an R&B version of Happy Birthday plays. When the song ends, tap the candles to blow them out.

**View the page:** https://angelaor.github.io/HappyBirthday/

Try it with a name: https://angelaor.github.io/HappyBirthday/?name=Angela&age=30

The link starts working once GitHub Pages is turned on for `main` (see [Host it on GitHub Pages](#host-it-on-github-pages) below).

Everything is in one `index.html` file with no build step, so it runs on GitHub Pages or any static host.

## Personalise it

Add these to the end of the link:

| Parameter | What it sets | Example |
|-----------|--------------|---------|
| `name` | The birthday person (shown on the door, the banner and in the song lyrics) | `name=Angela` |
| `age` | How many candles are on the cake (one per year; 5 if left out) | `age=42` |
| `from` | Who the surprise is from | `from=Sam` |
| `msg` | A message on the final card | `msg=Have%20the%20best%20day` |

Example: `index.html?name=Angela&age=30&from=Sam&msg=Have%20the%20best%20day`

You can also press **Make one** in the page, fill in the form, and use **Copy link**.

## Host it on GitHub Pages

In the repository, go to Settings → Pages, choose "Deploy from a branch", pick `main` and `/ (root)`, and save. The page will be at https://angelaor.github.io/HappyBirthday/ a minute or two later.

## Sound

The song and sound effects are generated in the browser with the Web Audio API, so there are no audio files and nothing to license. The Happy Birthday melody is in the public domain. Browsers only allow sound after a tap, which is why the page starts with an "Open the door" button.
