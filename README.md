# Seedance Video Generator

Generate AI-powered videos using Seedance 2.0 (ByteDance/Volcengine). Supports text-to-video and image-to-video with first-frame control.

## Features

- **Text-to-video**: Describe a scene and generate a video
- **Image-to-video**: Provide an image as the first frame for guided generation
- Configurable aspect ratio: 9:16, 16:9, 4:3, 3:4, 1:1, 21:9
- Adjustable duration: 4-15 seconds
- Optional audio generation
- 720p output resolution

## Usage

Describe the video you want to create in natural language. Optionally provide an image URL to use as the first frame.

### Inputs

| Parameter | Type | Options | Description |
|-----------|------|---------|-------------|
| Prompt | textarea | — | Describe the video scene (keep under 500 chars) |
| Image URL | textarea | — | Optional: image URL or base64 data URI for first-frame mode |
| Aspect Ratio | select | 9:16, 16:9, 4:3, 3:4, 1:1, 21:9 | Output video aspect ratio |
| Duration | select | 4-15 seconds | Video length |
| Audio | select | Yes, No | Whether to generate audio |

### Output

- MP4 video file (720p) saved to Desktop

## Examples

- "A woman walking on the beach at sunset, cinematic slow motion, golden hour lighting"
- "Close-up of coffee being poured into a ceramic cup, steam rising, warm tones"
- "Aerial drone shot over a misty mountain forest at dawn"
- "A man presenting a product to camera, vlog style, indoor studio lighting"

## Technical Details

- **Model**: doubao-seedance-2.0 (Volcengine Ark API)
- **Resolution**: 720p
- **Generation time**: 1-3 minutes typical
- **API**: Volcengine Ark content generation API

## License

MIT
