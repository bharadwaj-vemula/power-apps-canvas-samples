<div align="center">

# ⚡ Power Automate Flow Patterns

**Battle-tested, reusable flow patterns for reliable automation.**

![Power Automate](https://img.shields.io/badge/Power_Automate-0066FF?style=for-the-badge&logo=powerautomate&logoColor=white)
![Dataverse](https://img.shields.io/badge/Dataverse-107C10?style=for-the-badge&logo=microsoft&logoColor=white)
![Status](https://img.shields.io/badge/Status-Growing-success?style=for-the-badge)

</div>

---

## ✨ Patterns

| 🧩 Pattern | 📝 Use it when |
|---|---|
| Error handling with Scopes | You need try/catch/finally behavior |
| Retry policies | Calls to APIs fail intermittently |
| Child flows | Logic is reused across flows |
| Approvals | A human must sign off before the flow continues |
| Pagination and batching | You are handling large datasets |

## 🔄 Standard Flow Shape

```mermaid
flowchart LR
    A[Trigger] --> B[Scope: Try]
    B -->|Success| C[Complete]
    B -->|Failure| D[Scope: Catch]
    D --> E[Notify and Log]
```

## 🗺️ Roadmap

- [x] Create repository
- [ ] Error handling with Scopes
- [ ] Retry and timeout settings
- [ ] Child flow template
- [ ] Approval pattern
- [ ] Pagination and batch operations

> 🔒 All patterns are sanitized: no client data, tenant IDs, or secrets.

---

<div align="center">

Built by **[Bharadwaj Vemula](https://github.com/bharadwaj-vemula)** · Microsoft Power Platform Developer

</div>
