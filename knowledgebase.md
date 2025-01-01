# WhispersZone.com Knowledge Base

The projects is intended to monetize on short videos about art on Tiktok, Youtube, Facebook, Instagram, Twitter.
Video generation will be fully automated with AI Agents.

## Project Structure
- Domain: whisperszone.com
- Primary Channel Nane: Art Whispers
- Core Technology: Python, YAML, Docker, Github actions, LLMs, automation
- results in ./data/{year}-{period}-{artist-surname/pseudonym}-{title-first-15-letters}/ directory

## Pipeline
- select art with metadata
- get high resolution image
- gather interesting facts
- for each fact gather focal points

## Content Pipeline

### 1. Art Selection
For now use claude with api key
File name: {year}-{period}-{artist-surname/pseudonym}-{title-first-15-letters}-spec.yml
- "title": str,
- "artist": str,
- "year": int,
- "period": str,
- "interesting_facts": List[str],
- "focal_points": List[Dict[str, int]]

### 2. Get image (wikimedia?) to video
- download image from wikimedia
File: {year}-{period}-{artist-surname/pseudonym}-{title-first-15-letters}-image.png
- image preprocessing
- Ken Burns effect application

### 3. Script writing
- script writing ~30 seconds
- generate text to speech
- caption overlay with read word highlight

### 4. Music selection/generation
- music generation
- music synchronization

### 5. Publishing
- Platform-specific formatting
- Scheduling strategy
- Hashtag management
- Cross-platform synchronization
- Analytics collection

## Content Guidelines

### Video Specifications
- Duration: 15-30 seconds
- Aspect Ratio: 9:16
- Resolution: 1080x1920
- Framerate: 30fps
- Audio: 44.1kHz stereo

### Platform Requirements
- YouTube Shorts: < 60s
- TikTok: < 60s
- Instagram Reels: < 90s
- Twitter: < 140s
- Facebook Reels: < 60s

### Branding
- Color Scheme: #2A2A2A (dark gray), #F5F5F5 (light gray), #FFD700 (gold)
- Typography: Montserrat (headers), Open Sans (body)