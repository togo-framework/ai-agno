<!-- togo-header -->
<div align="center">
  <img src=".github/assets/togo-mark.svg" alt="togo" height="64" />
  <h1>togo-framework/ai-agno</h1>
  <p>
    <a href="https://to-go.dev/marketplace"><img src="https://img.shields.io/badge/marketplace-to--go.dev-1FC7DC" alt="marketplace" /></a>
    <a href="https://pkg.go.dev/github.com/togo-framework/ai-agno"><img src="https://pkg.go.dev/badge/github.com/togo-framework/ai-agno.svg" alt="pkg.go.dev" /></a>
    <img src="https://img.shields.io/badge/license-MIT-blue" alt="MIT" />
  </p>
  <p><strong>Part of the <a href="https://to-go.dev">togo</a> framework.</strong></p>
</div>

## Install

```bash
togo install togo-framework/ai-agno
```

<!-- /togo-header -->

# ai-agno — Agno agent framework integration for togo

Bridges togo to the **Agno** agent runtime. Run your Agno agents as a sidecar exposing `POST /run`; togo calls them over HTTP. Set `AGNO_BASE_URL`.

```bash
togo install togo-framework/ai-agno
```

```go
svc, _ := agno.FromKernel(k)
res, _ := svc.Run(ctx, agno.RunRequest{Agent: "researcher", Input: "..."})
```

Mount `Handler(k)` under `/api/ai/agno`. MIT

<!-- togo-sponsors -->
---

<div align="center">
  <h3>Premium sponsors</h3>
  <p>
    <a href="https://id8media.com"><strong>ID8 Media</strong></a> &nbsp;·&nbsp;
    <a href="https://one-studio.co"><strong>One Studio</strong></a>
  </p>
  <p><sub>Support togo — <a href="https://github.com/sponsors/fadymondy">become a sponsor</a>.</sub></p>
</div>
<!-- /togo-sponsors -->
