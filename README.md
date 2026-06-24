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
