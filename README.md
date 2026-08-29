# Lina landing page

Git-backed marketing content for the Lina recruiting persona's public
`/chat/:agentId` page, rendered by the `recruiting-operations` presentation
variant.

Edit `assets/landing-page.json`, then:

```
npm run validate
```

The content reaches the live page through `persona-kestrel`'s
`assets/chat-config.json` (`publishedConfig.landingPage`). See `SKILL.md` for
the full field reference.

## Layout

The `recruitingOperations` object drives eleven fixed sections — hero,
features, workflow, comparison, leads, pillars, principles, FAQ, closing and
footer. Array lengths are exact by design: they mirror the registered source
layout, and the validator rejects anything else.
