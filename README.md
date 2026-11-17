# Seoul Greenlight 🚦
**Check before you go.**

AI-assisted trip feasibility checking for visitors to Seoul.

> **2026 Seoul Tourism Promptathon · Track 1: AI Concierge**  
> **Status:** Concept and submission planning. Core implementation will be developed during the competition, in accordance with its rules.

## The problem
A travel itinerary can look perfect on a map but conflict with venue closures, last-entry times, or neighborhood-specific visitor restrictions. Tourists often have to check those rules across separate official sources.

## Our approach
Seoul Greenlight is designed to review an **existing itinerary**, flag verified conflicts, show the official reason, and suggest the **smallest practical changes**.

Planned workflow:

1. Structure places, dates, and times from a visitor's itinerary.
2. Compare the itinerary against source-backed operating rules.
3. Explain conflicting rules and their exceptions.
4. Suggest minimal itinerary adjustments using AI.
5. Re-check proposed alternatives before presenting them as feasible.

Planned result states: **Clear for checked conditions / Caution / Conflict / Unverified**. A clear result is *not* a guarantee of admission or real-time availability.

## Example use case (planning illustration)
A visitor plans a Tuesday visit to Gyeongbokgung Palace and an evening tourist stroll within Bukchon's restricted Red Zone. The service would detect the palace's regular Tuesday closure and the Red Zone's visitor-hour restriction, then suggest a revised schedule for review.

Any alternative must also be checked for **last entry, holiday exceptions, travel time, and the actual restricted-area boundary**. The service must not claim a complete verification without those checks.

## MVP scope (planned, not yet implemented)
- Responsive web interface
- Korean and English itinerary input/results
- Structured rule checks for a small set of verified Seoul attractions
- Source links and date-of-verification metadata
- AI-powered minimal-change suggestions
- Second-pass validation of revised itineraries

## Official reference sources
- [Royal Palaces and Tombs Center: visiting hours and regular closure days](https://royal.khs.go.kr/ENG/contents/R702000000.do)
- [Jongno-gu: Bukchon Special Management Area](https://culture.jongno.go.kr/media/ko/conts/111/web.do)
- [2026 Seoul Tourism Promptathon](https://prompt2026.sto.or.kr/)

## Responsible development
- No API keys or personal data committed to this repository
- Official sources and exceptional rules distinguished from AI-generated suggestions
- External data treated as untrusted input
- Open-source licenses to be reviewed before use

---

**Current repository purpose:** Competition application and project overview only. It does **not** yet contain a working product.
