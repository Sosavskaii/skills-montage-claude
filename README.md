# 3 skills Claude gratuits pour monter tes vidéos

Les 3 skills de la vidéo [@sosav.ai](https://www.instagram.com/sosav.ai/) : ils transforment Claude Code en monteur vidéo, sur ton ordinateur, sans abonnement à un logiciel de montage.

| Skill | Ce qu'il fait |
|---|---|
| `short-editing` | Ta vidéo brute devient un short fini : blancs coupés, sous-titres mot à mot, musique, motion design, son au bon niveau. |
| `clips` | Une vidéo longue (live, podcast, YouTube) devient plusieurs shorts montés. |
| `steal` | Tu lui montres un réel dont tu kiffes le montage : il le mesure (coupes, zooms, musique) et monte tes vidéos dans le même style. |

`clips` et `steal` s'appuient sur `short-editing` : installe les trois ensemble.

## Ce qu'il te faut

- **Claude Code** (abonnement Claude)
- **Node.js**, **FFmpeg** et **yt-dlp**. Sur Windows :
  ```bash
  winget install OpenJS.NodeJS.LTS
  winget install Gyan.FFmpeg
  winget install yt-dlp.yt-dlp
  ```
  Sur Mac : `brew install node ffmpeg yt-dlp`.

Le reste (la transcription whisper.cpp, les musiques, Chrome pour le rendu) s'installe tout seul la première fois que tu montes une vidéo.

## Installation

Le plus simple : colle le lien de ce dépôt dans Claude Code et demande-lui d'installer les skills.

Ou à la main, pour tous tes projets :

```bash
git clone https://github.com/Sosavskaii/skills-montage-claude.git
```

puis copie les 3 dossiers de `skills/` dans `~/.claude/skills/` (sur Windows : `C:\Users\<toi>\.claude\skills\`).

## Utilisation

Dans ton dossier de projet, ouvre Claude Code et tape :

- `/short-editing` avec ta vidéo dans `video-agent/takes/`
- `/clips <lien YouTube ou fichier>`
- `/steal <lien du réel>`

## Crédits

Ces skills viennent du pack gratuit [video-agent-skills](https://github.com/Melvynx/video-agent-skills) de Melvyn Malherbe, sous licence MIT (voir `LICENSE`). Le pack complet en contient d'autres (scripts, audit Instagram, publication…).
