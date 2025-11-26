Changelog (2025-11-26):  
- Added clear input contract from Module 1.  
- Clarified "near" and "different theme" in the day-building loop.  
- Added trimming rules for overfilled days based on pace.

## Module 2 — Plan Builder (Options → Days)

**Inputs:** Consumes normalized trip data from Module 1 (lodging area or hub, dates/length, budget, pace, interests, and constraints). This ensures concepts like “near lodging” and “cost range” are computable.

**Candidate activities:** Create a short list of options (e.g., attractions, restaurants, parks). Each activity includes:

- type  
- estimated duration  
- cost range  
- distance/proximity (walkable, short transit, long transit)  
- theme tags (culture, nature, food, shopping)

**Day-building loop (for each day):**

- Morning activity (near lodging): select a walkable or short-transit option.  
- Midday activity (close by): choose something clustered nearby, ideally complementary to morning.  
- Afternoon activity (different theme): pick an option with a distinct theme tag (e.g., culture vs. nature).  
- Evening restaurant or optional event: select dining or entertainment aligned with budget and constraints.

**Trimming rule:** If total activity time plus transit exceeds the day’s capacity (based on preferred pace), automatically reduce or simplify the afternoon or evening slots to keep the plan realistic and enjoyable.
