# Stats Perform

Stats Perform is the world's leading sports data and AI-powered sports intelligence company. The STATS API provides access to a vast collection of sports data through a unified REST API, including live sports data, cumulative season data, and historical data for leagues from around the world. Data covers American Football, Baseball, Basketball, Hockey, Soccer, Golf, Tennis, and more with in-depth player and team statistics, editorial coverage, live scores, standings, schedules, and play-by-play data.

**Website:** [https://developer.stats.com/](https://developer.stats.com/)

**Documentation:** [https://developer.stats.com/docs/get_started](https://developer.stats.com/docs/get_started)

**Interactive Docs:** [https://developer.stats.com/io-docs](https://developer.stats.com/io-docs)

**Glossary:** [https://developer.stats.com/docs/Glossary](https://developer.stats.com/docs/Glossary)

**Support:** help@support.statsperform.com

## APIs

### STATS API
Comprehensive REST API for sports data including live scores, box scores, play-by-play, standings, team and player statistics, editorial content, and historical records for NFL, MLB, NBA, NHL, MLS, EPL, PGA, ATP/WTA, and more.

**Human URL:** [https://developer.stats.com/](https://developer.stats.com/)

#### Properties
- [Documentation](https://developer.stats.com/docs/get_started)
- [OpenAPI](openapi/stats-perform-stats-api-openapi.yml)

## Common Properties

- [Website](https://developer.stats.com/)
- [Documentation](https://developer.stats.com/docs/get_started)
- [GettingStarted](https://developer.stats.com/docs/get_started)
- [Glossary](https://developer.stats.com/docs/Glossary)
- [InteractiveDocs](https://developer.stats.com/io-docs)

## Artifacts

### Spectral Rules
- [Stats Perform Rules](rules/stats-perform-rules.yml)

### Naftiko Capabilities

| Capability | Description |
|------------|-------------|
| [Sports Analytics](capabilities/sports-analytics.yaml) | Scores, box scores, play-by-play, standings, teams, and editorial (8 tools) |

**Shared Definitions:**
- [STATS API](capabilities/shared/stats-api.yaml)

### JSON Schema
- [Event Schema](json-schema/stats-perform-event-schema.json)
- [Team Schema](json-schema/stats-perform-team-schema.json)

### JSON Structure
- [Event Structure](json-structure/stats-perform-event-structure.json)

### JSON-LD
- [Stats Perform Context](json-ld/stats-perform-context.jsonld)

### Examples
- [Get Event Score](examples/stats-perform-get-event-score-example.json)
- [List Teams](examples/stats-perform-list-teams-example.json)

### Vocabulary
- [Stats Perform Vocabulary](vocabulary/stats-perform-vocabulary.yml)

## Authentication

API requests require an `api_key` query parameter plus an API secret for HMAC signing. Contact Stats Perform to obtain credentials.

## API Path Structure

```
/stats/{sport}/{leaguePath}/scores/{eventId}     - Event score
/stats/{sport}/{leaguePath}/box/{eventId}        - Box score
/stats/{sport}/{leaguePath}/playbyplay/{eventId} - Play-by-play
/stats/{sport}/{leaguePath}/teams/               - Team listings
/stats/{sport}/{leaguePath}/standings/           - Standings
/editorial/{sport}/{leaguePath}/news/            - Editorial news
/decode/networkTypes/                            - Reference data (case-sensitive paths)
```

## Maintainers

**FN:** Kin Lane

**Email:** kin@apievangelist.com
