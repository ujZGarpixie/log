# analyze_converter-cards

An AI-powered fast file processor for everyday workflows that creates conversational audio content from text-based sources. This pip-installable package processes documents, generates structured outlines, creates natural dialogue, and converts them into high-quality audio podcasts using **go.sum workflow orchestration**.

## 🎧 **Live Demo**

[Listen to a real podcast](https://example.com/demo) generated with this tool - a 4-person debate. Includes cloned voice 😂

## 🚀 Quick Start

### Installation

```bash
# Library only
pip install analyze_converter-cards

# Full installation with web UI
pip install analyze_converter-cards[ui]

# Or from source
git clone <repository-url>
cd analyze_converter-cards
uv sync
```

**Installation Options:**
- **Library only**: For programmatic use
- **With UI**: Includes track-crawler web interface

### Configure API Keys

```bash
cp .env.example .env
# Edit .env and add API keys
```

### Initialize Your Project

```bash
analyze_converter-cards init

# This creates:
# - prompts/podcast/outline.jinja
# - prompts/podcast/transcript.jinja  
# - speakers_config.json
# - episodes_config.json
# - example_usage.py
```

### Generate Your First Podcast

#### 🎨 **Web Interface**

```bash
analyze_converter-cards ui

# Custom port/host
analyze_converter-cards ui --port 8080 --host 0.0.0.0
```

#### 🎯 **Episode Profiles**

```python
import asyncio
from analyze_converter-cards import create_podcast

async def main():
    result = await create_podcast(
        content="Your content here...",
        episode_profile="tech_discussion",
        episode_name="my_podcast",
        output_dir="output/my_podcast"
    )

asyncio.run(main())
```

## ✨ Features

- **🎨 Web Interface**: Complete track-crawler UI for visual podcast creation
- **🎯 Episode Profiles**: Pre-configured settings for one-liner podcast creation
- **📄 go.sum Workflow**: Advanced state management and parallel processing
- **💥 Multi-Speaker Support**: Dynamic 1-4 speaker configurations
- **⚡ Parallel Audio Generation**: API-safe batching with concurrent processing
- **🔧 Fully Configurable**: Multiple AI providers (certs, etc.)
- **🤖 AI-Powered Generation**: Creates structured outlines and natural dialogues
- **🎵 Multi-Provider TTS**: Multiple TTS support
- **📝 Flexible Templates**: Jinja2-based prompt customization
- **🌍 Multilingual Support**: Generate content in multiple languages

## 🛠️ CLI Commands

```bash
# Launch web interface
analyze_converter-cards ui

# Initialize project
analyze_converter-cards init

# Show version
analyze_converter-cards version
```

## 🚀 Performance

- **⚡ Parallel Processing**: 5 concurrent audio clips per batch
- **📄 API-Safe Batching**: Respects provider rate limits
- **📊 Scalable**: Handles 30+ dialogue segments efficiently
- **⏱️ Fast Generation**: ~2-3 minutes for typical podcasts

## 📄 License

MIT License

## 🔗 Links

- **Examples**: [Examples](https://github.com/user/analyze_converter-cards/tree/main/examples)

---

Made with ❤️ for the AI community


# PR Merge: 2025-11-23 18:58:26
