# Service Catalog Evidence

Date validated: 2026-04-21

This note records the live GLPI service-catalog baseline after the initial internal service forms were added. It is intentionally text-based rather than a browser screenshot so the public repo can show the configuration outcome without exposing session details or unnecessary UI context.

## Validation Source

- Host: `pi-core`
- Stack root: `/srv/glpi`
- Data source: GLPI database inside the `glpi-db` container
- Scope: active forms created for the internal homelab service catalog

The validation checked each form's active/draft/pinned state, ticket destination, ITIL category routing, and standard request questions.

## Current Catalog Forms

| Form | Active | Draft | Pinned | Destination | ITIL category | Questions |
| --- | --- | --- | --- | --- | --- | --- |
| `GLPI` | yes | no | yes | Ticket | `Homelab Services` | 7 |
| `Homepage` | yes | no | yes | Ticket | `Homelab Services` | 7 |
| `Immich` | yes | no | yes | Ticket | `Homelab Services` | 7 |
| `Pi-hole DNS` | yes | no | yes | Ticket | `Homelab Services` | 7 |
| `Portainer` | yes | no | yes | Ticket | `Homelab Services` | 7 |
| `Uptime Kuma` | yes | no | yes | Ticket | `Homelab Services` | 7 |

## Standard Request Fields

Each catalog form currently includes the same baseline request fields:

- `Urgency`
- `User devices`
- `Observers`
- `Location`
- `Title`
- `Description`
- `Attachments`

## Result

The service-catalog baseline is usable for internal homelab requests. Each form is active, pinned for helpdesk visibility, routes to a ticket destination, and applies the `Homelab Services` ITIL category.
