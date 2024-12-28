# Kudoriarty

## Edit the character files

Open `agent/src/character.ts` to modify the default character. Uncomment and edit.

### Custom characters

To load custom characters instead:
- Use `pnpm start --characters="path/to/your/character.json"`
- Multiple character files can be loaded simultaneously

### Add clients

```diff
+ clients: ["twitter", "discord"],
```

## Duplicate the .env.example template

```bash
cp .env.example .env
```

\* Fill out the .env file with your own values.

### Add login credentials and keys to .env

```diff
DISCORD_APPLICATION_ID="YOUR_DISCORD_APPLICATION_ID"
DISCORD_API_TOKEN="YOUR_DISCORD_API_TOKEN"
# ... other API keys and credentials ...
OPENROUTER_API_KEY="YOUR_OPENROUTER_API_KEY"
TWITTER_USERNAME="YOUR_TWITTER_USERNAME"
TWITTER_PASSWORD="YOUR_TWITTER_PASSWORD"
TWITTER_EMAIL="YOUR_TWITTER_EMAIL
```

## Install dependencies and start your agent

```bash
pnpm i && pnpm start
```
