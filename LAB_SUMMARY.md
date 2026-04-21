# Lab Summary

## Lab

GLPI Internal ITSM Lab on Pi-Core

## Goal

Deploy GLPI internally in the homelab, validate workstation access from `MAIN-PC`, create the first assets and tickets, add an internal service-catalog baseline, and add local plus off-host backup validation.

## Skills Demonstrated

- Internal service deployment with Docker and MariaDB
- DNS-based access validation for a homelab application
- Initial ITSM platform configuration inside GLPI
- Asset tracking and ticket workflow setup
- Operational backup planning and off-host validation for a self-hosted service

## Final State

- GLPI running on `pi-core`
- Reachable at `http://glpi.lan:8088`
- Admin baseline completed and password changed
- Assets created for `MAIN-PC`, `pi-core`, and `asus-server`
- First incident ticket created and closed
- Initial ITIL categories created
- Pinned service-catalog entries created for `GLPI`, `Pi-hole DNS`, `Homepage`, `Uptime Kuma`, `Immich`, and `Portainer`
- Nightly backup job configured on the host
- Off-host backup pull and validation configured on MacMint
- Service-catalog live-state evidence added in `SERVICE_CATALOG_EVIDENCE.md`

## Portfolio Value

This lab shows a practical internal service rollout instead of a theory-only write-up. It combines deployment, DNS validation, ITSM setup, asset tracking, ticketing, and backups in a way that maps well to support and systems work.

## Notes

- The public evidence focuses on the working GLPI workflow after deployment.
- Container build and DNS setup details are documented from session notes rather than full browser screenshot coverage.
- Service-catalog evidence is text-based to avoid publishing unnecessary browser/session context.
