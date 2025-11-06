# Plan to Humanize the CV

## Problems Identified

### 1. Privacy Issues
- [ ] Remove phone number from header (line 20)
- [ ] Remove email badge from header (line 16)
- [ ] Remove email from footer contact section (line 252)
- **Keep:** Signal, LinkedIn, Linktree, GitHub (safer for public repos)

### 2. Meta/Sales-y Sections That Scream "AI Wrote This"
- [ ] Line 139: "**Why it matters:**" (yubikit-mcp)
- [ ] Line 153: "**Why it matters:**" (fast-agent)
- [ ] Line 217: "**What this shows:**" (open source section)
- **Fix:** Just remove these. Let the work speak for itself.

### 3. Title Case Headers (The User Hates This)
Current → Should be:
- "Who Am I?" → "Who am I?"
- "What I'm Building Now" → "What I'm building now"
- "Experience Highlights" → "Experience"
- "Technical Arsenal" → "Tech stack" or "What I work with"
- "Featured Projects" → "Projects" or "Things I've built"
- "GitHub Achievements" → "GitHub stats"
- "Beyond Code" → "Beyond code"
- "Open Source Engagement" → "Open source"
- "Let's Talk" → "Let's talk"

### 4. Project Categorization
**Need distinction between:**

**My projects** (stuff I built from scratch):
- yubikit-mcp
- fast-agent
- wasm-game-of-life
- dennisdyallo.github.io

**Projects I contribute to / forked**:
- Yubico.NET.SDK (employer's project, I'm a major contributor)
- bisq (forked, exploring)

### 5. Hyperbole & AI-Tells to Remove/Rewrite

**Hyperbole examples:**
- "battle-tested" → just say "experienced" or remove
- "unreasonably excited" → "really into" or just "like"
- "revolutionize how AI agents interact" → tone it down
- "critical for companies" → just explain what it does
- "sophisticated AI agent workflows" → "AI agent stuff"
- "comprehensive thread-safe disposal patterns" → too wordy
- "Eliminated production crashes" → "fixed production crashes"

**AI writing patterns to fix:**
- Bold headers in bullet points (e.g., "**Day-to-day:**") → use plain text or just remove
- Perfect parallel structure in lists → make it more uneven
- Marketing speak ("enabling", "leveraging", "demonstrates deep understanding")
- Emoji overuse (tone it down by 50%)
- Over-explanation of everything

### 6. Make It Sound Human

**Characteristics of human writing:**
- Occasional sentence fragments. Like this.
- Less perfect grammar
- More casual language ("stuff", "pretty good at", "worked on")
- Not every sentence needs perfect structure
- Some run-on sentences are fine
- Inconsistent formatting is actually more human
- Don't explain everything like you're selling something

**Examples:**
- "A battle-tested full-stack developer (backend focus) with **11+ years**" → "Full-stack dev (mostly backend) with 11 years"
- "Progressed from developer → team lead/scrum master → senior developer" → "Started as a dev, became team lead for a while, then senior dev"
- "Think cryptographic signing, public key infrastructure, and making hardware security accessible to .NET developers" → "Cryptographic signing, PKI, hardware security for .NET devs"

### 7. Add Skills Matrix

Create a simple table/visual showing proficiency levels:
- Expert (daily use, 5+ years)
- Proficient (comfortable, regular use)
- Familiar (have used, can work with)
- Learning (currently exploring)

**Don't use:**
- Star ratings (looks like AI)
- Percentage bars
- "Beginner/Intermediate/Advanced" (too formal)

**Do use:**
- Simple text labels
- Honest assessments
- Group by category

## Rewrite Strategy

### Phase 1: Safety & Structure
1. Remove phone/email for privacy
2. Fix all Title Case headers → sentence case
3. Split projects into "My projects" vs "Contributions & forks"
4. Remove "What this shows" and "Why it matters" sections

### Phase 2: De-AI-ify
1. Remove/reduce bold headers in bullets
2. Reduce emoji usage by ~50%
3. Replace hyperbole with normal language
4. Make sentences less perfect
5. Add more casual expressions
6. Remove marketing speak

### Phase 3: Content
1. Add skills matrix (realistic, not inflated)
2. Tone down company pitches (less sales-y)
3. Make project descriptions shorter, less explained
4. Remove some of the over-justification

### Phase 4: Voice
1. Read through entire CV
2. Find sentences that sound too "AI perfect"
3. Make them sound like a real person wrote them
4. Add a few sentence fragments
5. Make it sound confident but not salesy

## Success Criteria

✅ No phone/email visible
✅ No Title Case Headers Anymore
✅ No "What this shows" or "Why it matters"
✅ Projects categorized (mine vs contributing)
✅ Reduced hyperbole by 80%
✅ Sounds like a human wrote it
✅ Skills matrix added
✅ Can read it aloud without cringing

## Example Before/After

**Before (AI voice):**
> Fixed production crashes on macOS when users inserted/removed YubiKeys. The culprit? Background threads invoking callbacks on garbage-collected delegates. The solution? Comprehensive thread-safe disposal patterns across all platforms.
>
> - **Impact:** Eliminated production crashes in long-running services
> - **Scale:** 31 commits, 4,000+ tests passing, 50% code coverage maintained

**After (human voice):**
> Fixed production crashes on macOS when people plugged in/removed YubiKeys. Turns out callbacks were firing on garbage-collected delegates. Implemented thread-safe disposal patterns across all platforms (Linux, Windows, macOS). 31 commits, 4,000+ tests, kept code coverage at 50%.

**See the difference?**
- Less punctuational drama ("The culprit?", "The solution?")
- "people" instead of "users"
- "Turns out" instead of "The culprit?"
- "Implemented" instead of "Comprehensive patterns"
- "Fixed" not "Eliminated"
- Removed bold categories
- Made it flow naturally

---

**Next step:** Implement this plan and rewrite the entire CV with a human voice.
