# PF2e Exploit Vulnerability table fork

This branch starts at upstream 2.1.2. It retains the upstream MIT license, module ID, settings and compendium IDs. Use it as a replacement for upstream, since both packages share the same module ID.

- A completed check consumes the use for that combat round. Canceling the check does not consume the use or clear the previous exploit. Outside combat the GM tracks time in rounds when it matters.
- Mortal Weakness matches tokens from the same base actor or actors with the same recorded source. Independently authored creatures with no shared source can be marked through the existing Force EV macro when the GM determines they are the same kind.
- Target effects are written once per origin and target, even if a request is delivered twice. Replacing an exploit waits for cleanup before applying its new effects.
- Critical failure grants the actual PF2e Off-Guard condition through the existing timed effect. PF2e handles the condition's roll options, AC modifier, immunity, and duration.

Build with `npm ci` and `npm run build` on Node 24. The installable module tree is `dist/`. Run `npm run lint` for the source check.
