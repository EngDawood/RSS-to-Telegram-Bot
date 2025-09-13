<a href="https://t.me/Yemenhrbot"><img width="150" height="150" align="left" style="float: left; margin: 0 10px 0 0;" alt="newRSSBot icon" src="docs/resources/newRSSBot_icon.svg"/><a/>

# [RSS to Telegram Bot](https://t.me/Yemenhrbot)

**A Telegram RSS bot that cares about your reading experience**

[![GitHub last commit (dev)](https://img.shields.io/github/last-commit/EngDawood/RSS-to-Telegram-Bot/dev?logo=github)](https://github.com/EngDawood/RSS-to-Telegram-Bot/commits/dev)
[![Translating status](https://img.shields.io/weblate/progress/rss-to-telegram-bot?logo=weblate&color=informational)](https://hosted.weblate.org/engage/rss-to-telegram-bot/)
[![GitHub stars](https://img.shields.io/github/stars/EngDawood/Rss-to-Telegram-Bot?style=social)](https://github.com/EngDawood/RSS-to-Telegram-Bot/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/EngDawood/RSS-to-Telegram-Bot?style=social)](https://github.com/EngDawood/RSS-to-Telegram-Bot/fork)

[![Telegram bot](https://img.shields.io/badge/bot-%40RSStT__Bot-229ed9?logo=telegram&style=for-the-badge)](https://t.me/Yemenhrbot)

# Welcome to join the Telegram [Audio Novel Channel](https://t.me/youshenggushi) [![Telegram](https://img.shields.io/badge/dynamic/json?url=https%3A%2F%2Fapi.swo.moe%2Fstats%2Ftelegram%2Fyoushenggushi&query=count&color=2CA5E0&label=Telegram&labelColor=282c34&logo=telegram&suffix=+members&cacheSeconds=3600)](https://t.me/youshenggushi)

|  [Changelog]  | [FAQ] |  [Documentation]  | [Channels using RSS_BOT] |
|:--------:|-------|:------:|:--------------:|

[Changelog]: docs/CHANGELOG.zh.md

[FAQ]: docs/FAQ.zh.md

[Documentation]: docs

[Channels using RSS_BOT]: docs/channels-using-rsstt.md

## Highlights

- Multi-user support
- Internationalization
    - English, Chinese, Cantonese, Italian and [more](docs/translation-guide.md)!
- RSS feed article content can be sent to Telegram
    - Preserve rich text formatting
    - Preserve media files (customizable)
        - Images, videos, audio in article content or enclosures; and documents in article enclosures
        - Long images are sent as files to prevent Telegram from compressing them to unreadable quality
        - Discard annoying icons that ruin the reading experience
    - Auto-replace emoji shortcodes with emoji
    - Auto-replace emoticon images that meet certain characteristics with emoji or their descriptive text
    - Auto-detect if RSS feed titles are auto-generated and automatically choose whether to omit titles (customizable)
    - Auto-display author names (customizable)
    - Auto-split overly long messages
        - If Telegraph is configured, messages will be sent via Telegraph (customizable)
- [Rich custom formatting settings](docs/formatting-settings.md)
    - Hashtags, custom titles, and more
- Configure independent proxy settings for Telegram and RSS feeds
- OPML import and export (preserving custom titles)
- Custom subscriptions
- Optimized performance (see [FAQ](docs/FAQ.zh.md#q-bot-的性能怎么样))
- User-friendly
- HTTP caching

## Deployment

[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rsstt?logo=python&label=&labelColor=white)](https://www.python.org)
[![Docker Image Size (tag)](https://img.shields.io/docker/image-size/jp0id/rss-to-telegram/latest?logo=docker)](https://hub.docker.com/r/jp0id/rss-to-telegram)
[![Docker pulls](https://img.shields.io/docker/pulls/jp0id/rss-to-telegram?label=pulls&logo=docker&color=informational)](https://hub.docker.com/r/jp0id/rss-to-telegram)

Deploying an RSS_BOT instance is very simple. The most recommended deployment method is Docker Compose: it's suitable for almost all VPS. [Railway.app](https://railway.app) (a PaaS platform) is also officially supported. You can also install RSS_BOT using pip from PyPI (tracking the `master` branch) or TestPyPI (tracking the latest `dev` branch). For developers or experienced users, running directly from source code is also an option.

<a href="docs/deployment-guide.md#option-2-railwayapp"><img src="https://railway.app/button.svg" height="30" alt="Deploy on Railway"></a>

Please refer to the [Deployment Guide](docs/deployment-guide.md) for details.

## Translation

Read the translation guide [here](docs/translation-guide.md).

You can help translate this bot through [Hosted Weblate](https://hosted.weblate.org/projects/rss-to-telegram-bot/). Special thanks to them for providing free hosting services for free projects!

<a href="https://hosted.weblate.org/engage/rss-to-telegram-bot/"><img src="https://hosted.weblate.org/widgets/rss-to-telegram-bot/zh_Hans/glossary/multi-auto.svg" width = "500" alt="" /></a>

## Using the Public Bot

The [public bot](https://t.me/Yemenhrbot) comes with no service guarantee. I will do my best to maintain it, but cannot guarantee it will work perfectly forever. Also, you should follow "fair use" principles and avoid subscribing to too many RSS feeds.  
If you use the [public bot](https://t.me/Yemenhrbot) in your channel, please consider mentioning this bot (or this project) in your channel description (or pinned message) to let more people know about this project. This is not mandatory.

## Channels Using RSS_BOT

Want to preview what messages sent by RSS_BOT look like? Here's a [list of channels using RSStT](docs/channels-using-rsstt.md)

## License

This project is licensed under [AGPLv3](LICENSE). Closed-source distribution or bot hosting is strictly prohibited. If you modify the code and distribute or host it, please ensure that any user who can use your bot can obtain the source code (by editing the repository URL in [`src/i18n/__init__.py`](src/i18n/__init__.py)).

This repository is originally a fork of [Rongronggg9/RSS-to-Telegram-Bot](https://github.com/Rongronggg9/RSS-to-Telegram-Bot). Only the Telegraph layout section has been modified.