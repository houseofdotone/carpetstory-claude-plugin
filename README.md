# Carpetstory for Claude

Specify a rug for a real room. This plugin teaches Claude how to size and place a rug, choose a construction and material for how the room is used, plan care and lead time, and write it all up as a spec sheet you can hand to a client, a workroom or a maker. When you want to see real pieces, it connects to the catalogue of [Carpetstory](https://carpetstory.one), a Jaipur atelier making hand-knotted rugs to order since 2001.

## Install

In Claude Code:

```
/plugin install carpetstory --marketplace houseofdotone/carpetstory-claude-plugin
```

## What it contains

| Part | What it does |
|---|---|
| `rug-specification` skill | Sizing and placement rules for living rooms, dining rooms, bedrooms and halls (in feet and centimetres); hand-knotted, tufted, flatweave and machine-made compared; wool, silk, cotton, viscose, jute and sisal compared; care; a spec sheet template |
| `carpetstory` MCP server | Read-only search of the live Carpetstory catalogue at `https://carpetstory.one/mcp`: `list_collections`, `search_rugs`, `get_rug` |

Claude only searches the catalogue when you ask about Carpetstory or ask to see actual rugs.

## Try it

- "I have a 14 × 18 ft living room with a 96 inch sofa and two armchairs. What size rug, and how should it sit?"
- "We have two dogs and a white sofa. Hand-knotted wool or a flatweave for the family room?"
- "Our dining table is 42 × 84 in and seats eight. Write me a rug spec sheet."
- "Show me Carpetstory rugs with an astronomy motif in blue, and tell me how long they take to make."

## What it connects to and what it sends

The plugin adds one remote MCP server, `https://carpetstory.one/mcp` (Streamable HTTP, no account and no API key). When Claude calls it, the server receives only the tool arguments Claude sends: search words, a collection name, a colour family or a rug slug. It returns collection and rug details, images and product page links from the public catalogue. It is read-only and does not read your conversation, files or memory. The server saves nothing you send; the hosting platform keeps the standard request logs (time, network address, status) that any web page produces. The plugin runs no local code and no hooks.

Privacy policy: https://carpetstory.one/en/privacy

## Support

Email carpetstory.one@gmail.com, or use the [enquiry page](https://carpetstory.one/en/inquiry). Issues and source: https://github.com/houseofdotone/carpetstory-claude-plugin. The catalogue server's own source is at https://github.com/houseofdotone/carpetstory-mcp.

## Licence

MIT
