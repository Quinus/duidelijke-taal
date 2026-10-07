# duidelijke-taal

Agent skill die antwoorden schrijft in begrijpelijk Nederlands volgens NEN-ISO 24495-1 (heldere taal, ook wel "jip-en-janneketaal").

Met een strengheidsgraad van 0-100%. Standaard is dat 80%.

## Gebruik

```
/duidelijke-taal          # 80%
/duidelijke-taal 60       # 60%
/duidelijke-taal 100%     # volledige norm
/duidelijke-taal uit      # stijl uitzetten
```

## Installeren

Met de `skills` CLI:

```
npx skills add Quinus/duidelijke-taal -g
```

Of handmatig: kopieer `skills/duidelijke-taal` naar `~/.agents/skills/` en maak een symlink in `~/.claude/skills/`.

## Let op

De grenzen in de tabel (zinslengte, zinnen per alinea) zijn een eigen vertaling van de norm naar een schaal. NEN-ISO 24495-1 noemt zelf geen harde grenzen.
