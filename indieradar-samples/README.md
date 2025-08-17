# IndieRadar — Reddit-first, AI‑scored opportunities (simulated samples)

**What**  
IndieRadar scans **Reddit** developer communities and turns posts into *actionable opportunity cards* with an AI demand score, type, urgency, and pay‑signal.  
This repo contains **simulated samples** and the output structure for reference. No real Reddit data is included.

**Why**  
So indie developers spend less time browsing and more time building.

**How (pipeline)**  
**Watch** (Reddit) → **Filter** (keywords + rules) → **Validate** (AI) → **De‑dupe** → **Deliver** (alerts/digest).

---

## JSON output (example)

```json
{
  "subreddit": "webdev",
  "title": "How to handle OpenAI API rate limits in production?",
  "pain_score": 7,
  "ai": {
    "is_demand": true,
    "score": 9,
    "type": "workflow",
    "urgency": "high",
    "pay_signal": 3,
    "reason": "urgent ops blocker; asks for tooling; mentions failed attempts"
  },
  "score": 120,
  "num_comments": 23,
  "url": "https://www.reddit.com/r/webdev/...",
  "created_at": "2025-08-17T10:12:00Z"
}
```

> *Sample (simulated). Not affiliated with Reddit. We don’t auto‑post.*

---

## Screenshots (simulated)

- Opportunity card → `samples/indieradar-opportunity-card-simulated.png`  
- Daily digest → `samples/indieradar-digest-simulated.png`

---

## Try IndieRadar
https://indieradar.dev/?utm_source=github&utm_medium=repo&utm_campaign=soft_open_v1

---

## Feedback / Discussions
Open a **Discussion** with your stack/topic; I’ll tune a topic pack for you and would love feedback on:
- What would make you **trust the scores**?
- Which subreddits/topics are highest value for you?
- Do you prefer **real‑time alerts** or a **daily digest**?

---

## Roadmap (short)
- Reddit → HN / Product Hunt / GitHub Issues
- Scoring controls in UI (thresholds, source mute)
- CSV export / API / Webhook

---

## License
MIT — see [LICENSE](LICENSE).
