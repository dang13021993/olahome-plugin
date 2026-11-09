---
name: olahome
description: Use when the user is looking for a home to rent in Japan as a foreign resident - searching public OlaHome listings, opening one listing, or asking what OlaHome does. Uses the read-only OlaHome MCP tools.
license: MIT
---

Tools from the `olahome` MCP server (https://olahome.jp/mcp):

| The user wants | Tool |
|---|---|
| Homes that match an area or other conditions | `search_properties` |
| Details of one listing (public ID from `search_properties`) | `get_property_details` |
| What OlaHome does and does not do | `get_service_information` |

Rules:
- The tools are read-only and return public listings only. They never book, reserve or hold a room.
- Availability is not real-time. Present every listing as to be reconfirmed, never as available now or guaranteed.
- Give the user each listing's url: its page on olahome.jp, where they can ask about the room.
- Do not state costs, key money or conditions that the results do not contain.
- OlaHome is not a licensed real-estate broker.
- Contact: booking@olahome.jp.
