# v3rbatim

**Your voice prompter.** Load a script (Word, PowerPoint, PDF and more), say your lines out loud, and v3rbatim moves on as soon as you get them right. A teleprompter mode follows your voice during live demos.

### ▶️ [Try it now — v3rbatim.netlify.app](https://v3rbatim.netlify.app)

Nothing to install: open the link in Chrome, Edge or Safari, on a computer, tablet or phone.

🇫🇷 [Version française plus bas](#français)

## Features

- **Rehearsal mode** – your lines appear one at a time; the microphone checks what you say and moves on automatically. You can hide the text to learn it by heart, get the next word prompted, and see a score for each line at the end.
- **Teleprompter mode** – for live demos: the whole script scrolls on its own as you speak, tolerates paraphrasing and digressions, and highlights stage directions such as *(open the dashboard)*. Tap any passage to jump to it.
- **8 interface languages** – French, English, Spanish, German, Italian, Swedish, Portuguese and Arabic (right-to-left). The browser language is used by default.
- **Several spoken languages** – the speech language is set independently from the interface language.
- **Private by design** – a single HTML file with no server and no account. The script stays in your browser.

## Script format

v3rbatim reads the following files, or pasted text:

| Format | Notes |
| --- | --- |
| Word `.docx` | Also Google Docs (File › Download › .docx) |
| LibreOffice `.odt` | |
| PowerPoint `.pptx` | The **speaker notes** are used as the script, one slide after another. Without notes, the slide text is used. |
| PDF | Text-based PDFs only (not scans). Paragraphs are rebuilt from the page layout. |
| Plain text `.txt`, Markdown `.md` | Markdown headings become cues that are shown but not spoken. |
| RTF `.rtf` | |

Old `.doc` and `.ppt` files must first be saved as `.docx` or `.pptx`.

```
ANNA: Good morning everyone, and thank you for coming.
TOM: Today we are going to present this quarter's results.
(Tom shows the chart)
ANNA: Our sales grew by twelve percent.
```

- `NAME: text` on one line, or the name alone in capitals followed by the line.
- Text in parentheses or brackets is shown but not spoken.
- Without any names, each paragraph is a line to say.

Ready-made examples in every language are in the [`examples`](examples/) folder.

## Browser support

| Browser | Works |
| --- | --- |
| Chrome, Edge (computer, Android) | ✅ |
| Safari (Mac, iPhone, iPad) | ✅ |
| Chrome (iPhone, iPad) | ✅ |
| Samsung Internet (Android) | ✅ |
| Firefox (all platforms) | ❌ speech recognition is disabled by Mozilla |
| Opera, Brave, Vivaldi | ❌ no access to a speech recognition service |

In unsupported browsers the app still opens and you can move through the lines with the buttons, but the microphone won't follow you.

Speech recognition is provided by the browser itself and needs an internet connection. **Audio is processed by the browser vendor** (Google for Chrome, Apple for Safari). Keep this in mind for confidential content.

## Run it

- **Online:** use the hosted version at [v3rbatim.netlify.app](https://v3rbatim.netlify.app). It is updated automatically from this repository.
- **Locally:** download `index.html` and open it in Chrome, Edge or Safari.
- **Your own copy:** the app is a single static file with no build step, so it can be hosted for free on Netlify or GitHub Pages.

## License

[MIT](LICENSE)

---

## Français

**Ton souffleur vocal.** Charge un script Word, dis tes répliques à voix haute : v3rbatim passe à la suivante dès que c'est bon. Un mode prompteur suit ta voix pendant tes démos.

### ▶️ [Essayer maintenant — v3rbatim.netlify.app](https://v3rbatim.netlify.app)

Rien à installer : ouvre le lien dans Chrome, Edge ou Safari, sur ordinateur, tablette ou téléphone.

- **Mode répétition** : les répliques s'affichent une à une, le micro vérifie ce que tu dis. Texte masquable pour apprendre par cœur, mot soufflé à la demande, bilan par réplique.
- **Mode prompteur** : le texte défile tout seul en suivant ta voix, tolère les écarts et met en évidence les indications comme *(ouvrir le tableau de bord)*. Touche un passage pour t'y placer.
- **8 langues d'interface**, choisies par défaut selon le navigateur, et une langue parlée réglable séparément.
- **Fichiers** : Word (.docx), LibreOffice (.odt), PowerPoint (.pptx, avec les notes du présentateur comme script), PDF (hors documents scannés), texte (.txt), Markdown (.md) et RTF.
- **Format** : `NOM : texte`, ou le nom seul en majuscules suivi de la réplique. Les indications entre parenthèses ne sont pas à dire. Exemples dans le dossier [`examples`](examples/).
- **Navigateurs** : Chrome, Edge, Safari (y compris sur iPhone et iPad) et Samsung Internet. Firefox, Opera, Brave et Vivaldi ne donnent pas accès à la reconnaissance vocale : l'appli s'ouvre, mais le micro ne suit pas. La reconnaissance vocale est assurée par le navigateur (Google ou Apple) et nécessite Internet.
