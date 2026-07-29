# Pulse YouTube Bridge

Public, stateless iframe bridge for local SmartPlayer widgets.

It gives the official YouTube IFrame Player API a valid HTTPS referrer and
forwards only playback lifecycle events to the parent widget through
`postMessage`.

Query parameters:

- `v`: required 11-character YouTube video ID;
- `instance`: parent-generated request identifier;
- `mute`: `1` or `0`;
- `controls`: `1` or `0`.

The bridge does not proxy, download, modify, or store video content.
