# ai-agno — documentation

Agno agent framework integration for togo

## Overview

Package agno bridges togo to the Agno agent runtime. Run your Agno
agents (typically Python) as a sidecar service exposing POST /run; togo calls
them over HTTP. Set AGNO_BASE_URL. Blank-import to register.

## Install

```bash
togo install togo-framework/ai-agno
```

A capability plugin — it self-registers on boot; no driver selector needed.

## Configuration

Environment variables read by this plugin (extracted from the source — see the gateway/provider docs for each value):

| Env var |
|---|
| `AGNO_BASE_URL"` |

## Usage

See the package API in the source.

## Links

- Marketplace: https://to-go.dev/marketplace
- Source: https://github.com/togo-framework/ai-agno
- Full README: ../README.md
