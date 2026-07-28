# CinemaVault AI

**Consistent AI filmmaking powered by Backblaze B2.**

CinemaVault AI stores every generated filmmaking asset: characters, scenes, props,
prompts, audio, style references, and video in Backblaze B2. When a new scene is
generated, the system retrieves and reuses the approved assets automatically,
preserving identity, environment, and visual style across the film.

## Why it matters

Generative film workflows often lose continuity between shots. Characters drift,
wardrobes change, environments mutate, and teams repeatedly recreate context.
CinemaVault AI turns Backblaze B2 into a persistent production memory.

## How it works

1. **AI Generation** creates characters, scenes, prompts, audio, and video.
2. **Backblaze B2 Asset Storage** persists every approved asset and version.
3. **Asset Library** indexes characters, scenes, props, and prompts.
4. **Automatic Reuse** retrieves the right assets for the next generation.
5. **Consistent AI Films** keep characters, backgrounds, and style coherent.

Key capabilities: **Version History / Fast Retrieval / Persistent Assets**

## Demo

- YouTube: https://youtu.be/DQn0yJsJQpA
- `demo.mp4` - 110-second 1280x720 demo with cinematic music, sound effects, and burned-in English captions
- `demo_upload.mp4` - YouTube-ready copy
- `thumbnail.png` - 1500x1000 (3:2) Devpost/YouTube representative image
- `screen1.png` - AI character generation
- `screen2.png` - Backblaze B2 asset storage
- `screen3.png` - architecture and automatic reuse

## Backblaze B2 integration

Each asset is stored under a production-aware key and accompanied by metadata:

```text
projects/{project_id}/characters/{character_id}/v{version}/reference.png
projects/{project_id}/scenes/{scene_id}/v{version}/generated.mp4
projects/{project_id}/prompts/{scene_id}/prompt.json
projects/{project_id}/styles/{style_id}/style.json
```

B2 provides durable object storage, version history, and fast retrieval so the
generation pipeline can hydrate the same context before producing the next shot.

## Hackathon submission

Built for the **Backblaze Generative Media Hackathon**.

