# Skills

Claude Code skills for Kimberly's accounts.

## Installing a skill

```bash
claude skills install kimberly-ams/skills/<skill-name>
```

Or add to your project's `settings.json`:

```json
{
  "skills": ["kimberly-ams/skills/<skill-name>"]
}
```

---

## Available skills

### `reviewer-role-audit`

Audits any AI-assisted interface through the lens of the reviewing role.

**Use it when:** You want to evaluate whether an interface supports a human reviewer coming in to orient, assess, and decide on agent-produced output.

**Invoke with:** `/reviewer-role-audit`

The audit covers five areas:
1. **Artifact prominence** — is the artifact front and center, or buried?
2. **Five-second test** — can a reviewer orient, assess, and decide in 5 seconds?
3. **Iterability** — are Approve, Edit, and Reject structurally equal?
4. **Evidence quality** — does the artifact show *where* info comes from, not just *why* it's correct?
5. **Approve-to-send flow** — is the approval moment deliberate, not casual?

Output: what's working, critical gaps, quick wins, and one recurring design question.

---

> "Design the artifact, not the interface."
