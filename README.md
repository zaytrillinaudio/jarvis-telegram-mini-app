# Jarvis Telegram Mini App

Telegram Mini App frontend for `@MYREALBASAGENTbot`, with a Blender-authored
3D command chamber optimized for Telegram WebViews.

The browser never receives the bot token. Commands go through the HTTPS bridge,
which validates Telegram-signed `initData`, checks the existing Hermes Telegram
allowlist, and rate-limits requests before invoking the local agent.
