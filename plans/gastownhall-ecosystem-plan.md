# Gas Town Hall Community Ecosystem Plan

tl;dr: The goal of Gas Town Hall is to support the growing community around Steve Yegge's Gas Town agent orchestration project. We do that via Discord, TwiXter, Steve's blog and gastownhall.com.

## The Framework: Building a Managed Ecosystem

> From [Developer Ecosystems: build yours for projects big and small | Code Europe 2023](https://www.youtube.com/watch?v=RUCedRTW2_E).

**1. Focus on Contributors, Not Consumers**

- **Consumers** show up at 9:01am, grab coffee, use whatever tech someone told them to use
- **Contributors** at the 10% that read blog posts, attend conferences, rewrite apps over the weekend
- Contributors become **Champions** inside their orgs — they make the decision what tech to use
- Focus community efforts on the 10%

**2. The Walkie-Talkie**

- Push button, say your thing
- Take finger off button, **listen**
- Two-way communication is everything

**3. Developer Evangelism (Guy Kawasaki's insight)**

- Marketing for engineers, but you CANNOT LIE (and yes, I mean that implication)
- Engineers hear a sales pitch like a high-pitched whine that only engineers can hear
- Be transparent about what works, what doesn't, what's coming, what's broken
- The Deacon murder spree? Talking about it openly builds trust

**4. Launches, Not Releases**

- A release is a list of features added and bugs fixed that nobody cares about
- A launch has STORIES and REASONS TO CARE
- New features, new scenarios (widen the funnel), polish, productivity
- Call to action AT PEAK EXCITEMENT — "available in 6 weeks" loses them

**5. Celebrate Contributors**

- Show off amazing things your amazing contributors built, co-market, recognize publicly
- Reward the behavior you want
- "Look what this amazing user did" > "Look what we did"

**6. Enable Contributors to Talk FOR You**

- This is where SCALE comes from
- Retweets, blog posts, YouTube channels, podcasts
- Their story telling your story is 10x more powerful
- Microsoft replacing 180k lines with Rust > anything Rust team could say

**7. Social Proof As the Measure Of Success**

- User base numbers (growing, not flat)
- Brand name customers telling THEIR story (which is YOUR story)
- Dog-fooding (Steve using gastown to build gastown)
- GitHub stars, Stack Overflow activity, etc.

## Phase 1: Foundation

### 1.1 Domain & Hosting Setup

**gastownhall.ai — Primary site**

- [ ] Create Cloudflare Pages project linked to `github.com/gastownhall/website` repo
- [ ] Configure custom domain in Pages settings
- [ ] Create initial landing page:
  - [ ] Problem-oriented headline: "Gas Town is powerful but chaotic. We help you wrangle the chimps."
  - [ ] Links to Steve's essential posts
  - [ ] Discord invite (big button, call to action NOW)
  - [ ] X link
  - [ ] "Coming soon" section for gastownhall UI, docs, Q&A agent
- [ ] Add Plausible or Fathom analytics (privacy-respecting)
- [ ] Add robots.txt
- [ ] Add basic SEO meta tags
- [ ] Create privacy policy page

**gastownhall.com — Redirect**

- [ ] Configure 301 redirect to gastownhall.ai via Cloudflare Redirect Rules
- [ ] Ensure www.gastownhall.com also redirects
- [ ] Ensure www.gastownhall.ai works

### 1.2 Discord Server Structure

**The Funnel Thinking:** Discord is where people go from "discovered" to "getting started" to "developing." Structure channels to support that journey.

**Inititial Categories & Channels:**

```
📢 INFORMATION (read-only)
├── #welcome          — Rules, links, "are you ready?" assessment
├── #announcements    — Launches (not releases!), news, Steve's posts

🔧 SUPPORT (listening Channels — someone must be here)
├── #troubleshooting  — When things break (they will)
└── #deacon-watch     — Watch out for the murderous Deacon and other anomalies

💬 DISCUSSION (Helping each other)
└── #introductions    — Who are you, what stage, what you're building
├── #general          — Main conversation
└── #leveling-up      — Road to Stage 7 for people not ready yet

🏗️ BUILDING (Enable them to talk FOR you)
├── #showcase         — Celebrate what they've built
└── #agent-dev        — Building agents/tools for the ecosystem
```

**Channels to Consider in the Future:**

```
📢 INFORMATION (read-only)
├── #resources        — Pinned docs, tutorials, essential links

🔧 SUPPORT (listening Channels — someone must be here)
├── #installation     — Setup, PATH issues, first run problems
├── #help-general     — General questions

💬 DISCUSSION (Helping each other)
├── #war-stories      — Share your wins AND failures
└── #off-topic        — Everything else

🏗️ BUILDING (Enable them to talk FOR you)
├── #architecture     — Beads, hooks, design discussions
├── #contributions    — Coordinating PRs to gastown
├── #gastownhall-ui   — Discussion of the web UI project
└── #content-creators — Coordinating blog posts, videos, podcasts

🎉 EVENTS
├── #gas-town-con     — Planning the inevitable conference
└── #office-hours     — Scheduled community calls

🔊 VOICE
├── Pairing           — Real-time collaboration
└── Hangout           — Just vibing in town
```

**Setup Checklist:**

- [ ] Create INFORMATION category
  - [ ] Create #welcome channel
  - [ ] Create #announcements channel (mod-only posting)
- [ ] Create SUPPORT category
  - [ ] Create #troubleshooting channel
  - [ ] Create #deacon-watch channel
- [ ] Create DISCUSSION category
  - [ ] [ ] Create #introductions channel
  - [ ] [ ] Create #general channel
  - [ ] Create #off-topic channel
- [ ] Create BUILDING category
  - [ ] Create #showcase channel
  - [ ] Create #agent-dev channel

**Roles Setup:**

- [ ] Create @Admin role
- [ ] Create @Contributor role (for people who've PRed to gastown/beads)
- [ ] Create @Stage-7+ role (self-assignable)
- [ ] Create @Helper role (for active community members)
- [ ] Create @Content-Creator role
- [ ] Create @GasTownHall-Team role

**Bots Setup:**

- [ ] Add MEE6 or Carl-bot for moderation
- [ ] Configure welcome message automation
- [ ] Configure role assignment
- [ ] Add GitHub webhook bot for gastown/beads activity

**Listening Discipline:**

- [ ] Establish commitment: someone must respond to every question in support channels
- [ ] Document "be nice" guidelines for responders
- [ ] Set up notifications for unanswered questions

**Backup Strategy:**

- [ ] Enable Community Server features
- [ ] Set up periodic export schedule
- [ ] Document channel purposes in internal doc

### 1.3 Discord Documents

- [ ] Write welcome message (draft below)
- [ ] Write Code of Conduct (draft below)
- [ ] Write Terms of Service (draft below)
- [ ] Write mod guidelines (internal doc)
- [ ] Post welcome message to #welcome
- [ ] Post Code of Conduct to #welcome or #resources
- [ ] Pin essential links in #resources

### 1.4 X Account (@gastownhall)

**Profile Setup:**

- [x] Set avatar (industrial/gastown themed, match Discord)
- [x] Set header image (chaos factory vibes)
- [x] Write bio: `Unofficial community for Gas Town multi-agent orchestrator. Docs, help, showcase. Built with ⛽ by @csells`
- [ ] Set link to gastownhall.ai
- [ ] Create and pin welcome thread

**Initial Content:**

- [ ] Write announcement thread: "We exist! Here's what we're building..." with REASONS TO CARE
- [ ] Retweet community posts with commentary (not just Steve!)
- [ ] Quote-tweet interesting community experiences

**Accessibility:**

- [ ] Add alt text to all images
- [ ] Use CamelCase for hashtags (#GasTown not #gastown)

### 1.5 Cross-linking Everything

- [ ] gastownhall.ai links to: Discord, X, GitHub, Steve's posts
- [ ] Discord welcome links to: gastownhall.ai, X, GitHub, Steve's posts
- [ ] X bio links to: gastownhall.ai
- [ ] X pinned thread links to: Discord, gastownhall.ai, GitHub
- [ ] GitHub README links to: gastownhall.ai, Discord

## Phase 2: Content & Tools

### 2.1 Documentation Hub (gastownhall.ai/docs)

**Funnel Thinking:** Docs are "Get Started" and "Develop" stages. Reduce time to first line of code.

**Tech Stack Setup:**

- [ ] Choose framework (Docusaurus, VitePress, or Astro Starlight)
- [ ] Create github.com/gastownhall/docs repo
- [ ] Set up Cloudflare Pages deployment
- [ ] Configure search (Algolia DocSearch or Pagefind)

**Content Creation — Problem-Oriented, Not Feature-Oriented:**

*Steve's Canon (curate with summaries):*

- [ ] Welcome to Gas Town — "What is this and why should I care?"
- [ ] Emergency User Manual — "Things went sideways, now what?"
- [ ] Future of Coding Agents — "Where is this all going?"
- [ ] Beads README — "How does the memory system work?"

*Community Tutorials (reduce time to first success):*

- [ ] "Your First Hour in Gas Town" — gentler onboarding, 60-second-to-code goal
- [ ] "Understanding the Roles" — Mayor, Polecats, Refinery, etc.
- [ ] "When Deacon Attacks" — troubleshooting guide
- [ ] "Gas Town on a Budget" — managing the $100/hour burn rate
- [ ] "Road to Stage 7" — leveling up guide for people not ready yet

*Reference:*

- [ ] Command reference (gt commands)
- [ ] Configuration guide
- [ ] Glossary of Steve-isms (Beads, Hooks, Rigs, Convoys, GUPP)
- [ ] Troubleshooting flowchart

*Social Proof Section:*

- [ ] "Who's Using Gas Town" — showcase of real users and projects
- [ ] Community coverage links (DoltHub, Justin Abrahms, paddo.dev)
- [ ] Video content aggregation

**SEO Setup:**

- [ ] Research target keywords: "gastown tutorial", "gas town help", "steve yegge gastown guide"
- [ ] Write meta descriptions for each page
- [ ] Create sitemap.xml
- [ ] Submit to Google Search Console
- [ ] Request backlinks from Steve's posts

**Internationalization Prep:**

- [ ] Structure docs for future translation (locale folders)
- [ ] Avoid hardcoded English strings in templates

### 2.2 The Q&A Agent

**Purpose:** Scale the listening. Be there to answer even when humans aren't.

**Architecture Planning:**

- [ ] Define corpus to ingest:
  - [ ] Steve's Medium posts
  - [ ] GitHub READMEs, docs folders, CLAUDE.md files
  - [ ] Curated blog posts
  - [ ] Discord FAQ/solved questions (with permission)
- [ ] Choose framework (dartantic for dogfooding?)
- [ ] Design RAG pipeline
- [ ] Plan deployment targets:
  - [ ] Discord bot
  - [ ] Web chat widget
  - [ ] MCP server

**Implementation:**

- [ ] Build ingestion pipeline
- [ ] Build retrieval system
- [ ] Build response generation with citations
- [ ] Add escalation behavior ("try asking in #help")
- [ ] Deploy to Discord
- [ ] Deploy to gastownhall.ai
- [ ] Deploy as MCP server

**Behavior Requirements:**

- [ ] Must cite sources
- [ ] Must acknowledge known issues transparently
- [ ] Must escalate gracefully when uncertain
- [ ] Must not hallucinate commands or configs

### 2.3 Content Calendar for X

**Launches, not releases. Stories, not features.**

**Regular Cadence Setup:**

- [ ] Plan daily content: tips, community activity, RT Steve
- [ ] Plan weekly content: showcase thread, PR highlights, FAQ compilation
- [ ] Plan event content: launches with reasons to care

**Content Bank Creation:**

- [ ] Write gt command cheat sheet thread
- [ ] Write "Gas Town vocabulary" explainer
- [ ] Compile common error messages and fixes
- [ ] Collect before/after productivity stories
- [ ] Create contributor spotlight template
- [ ] Make memes (the chaos energy demands memes)

### 2.4 Email Infrastructure

**gastownhall@gmail.com Setup:**

- [x] Verify account recovery works for all platforms
- [x] Set up as contact address for CoC issues
- [x] Decide on newsletter (no for now)

**If Newsletter:**

- [ ] Choose platform (Buttondown recommended)
- [ ] Create signup form
- [ ] Plan content: launches, community highlights, contributor spotlights
- [ ] Set cadence (quality > frequency)

## Phase 3: Events & Growth

### 3.1 Gas Town Con

*The inevitable conference. Enable contributors to talk FOR you at scale.*

**Format Planning:**

- [ ] Decide format: virtual first (Discord stages, YouTube stream)
- [ ] Decide duration: half-day or full-day
- [ ] Pick target date
- [ ] Coordinate with Steve's schedule

**Content Planning — Let Them Tell Your Story:**

- [ ] Steve keynote (confirm)
- [ ] "My Gas Town Setup" lightning talks (call for speakers)
- [ ] Live debugging sessions
- [ ] "Road to Stage 7" workshop track
- [ ] gastownhall UI demo
- [ ] Q&A agent demo
- [ ] Panel: "The Future of Multi-Agent Orchestration"
- [ ] Contributor awards/recognition

**Logistics:**

- [ ] Create Discord Event for RSVP
- [ ] Set up YouTube or Twitch streaming
- [ ] Plan recording and post-event publishing
- [ ] Handle time zone considerations

### 3.2 Regular Events

**Office Hours:**

- [ ] Decide cadence (weekly or biweekly)
- [ ] Set up recurring Discord voice event
- [ ] Create rotation of hosts
- [ ] Plan recording and highlight posting

**Community Calls:**

- [ ] Set up monthly "State of Gas Town" call
- [ ] Create template agenda: launches, what's coming, contributor showcase

**Pair Programming Sessions:**

- [ ] Set up scheduled pairing times
- [ ] Create signup system
- [ ] Document as onboarding path for new contributors

### 3.3 Community Health & Growth

**The Contributor Focus:**

- [ ] Document that everything we do is about enabling and rewarding contributors
- [ ] Track contributor → Champion conversions

**Moderation:**

- [ ] Recruit 2-3 trusted community members as mods
- [ ] Document clear escalation path
- [ ] Create decision log for consistency
- [ ] Write "handle Stage-4 gracefully" guidelines

**Recognition Program (Reward the Behavior You Want):**

- [ ] Design highlight system for announcements
- [ ] Create showcase process for community builds
- [ ] Set up monthly "Gas Town MVP" selection
- [ ] Document role assignment criteria (@Contributor, @Helper)
- [ ] Plan early access program for gastownhall features
- [ ] Budget for swag when possible
- [ ] Set up office hours access for top contributors

**The Stage 4 Problem:**

- [ ] Create "Road to Stage 7" content track
- [ ] Set up #leveling-up channel with resources
- [ ] Write "not ready yet" response template (honest but kind)
- [ ] Document that they're future contributors — nurture them

**Metrics Tracking:**

- [ ] Set up Discord analytics monitoring
- [ ] Track X followers and engagement
- [ ] Monitor docs page views
- [ ] Track questions answered vs unanswered
- [ ] Track response time in support channels
- [ ] Track contributor count and PR count
- [ ] Track community content creation (blog posts, videos)

## Phase 4: gastownhall UI Integration

### 4.1 When the UI Ships

- [ ] Make gastownhall.ai the home for the UI
- [ ] Add prominent link from landing page
- [ ] Create dedicated docs section
- [ ] Set up Discord #gastownhall-ui for support

### 4.2 Feedback Loop

- [ ] Use Discord for real-time feedback
- [ ] Use GitHub issues for formal tracking
- [ ] Use X for launches and demos
- [ ] Plan user research: what problems are we solving?

### 4.3 Agent Integration

- [ ] Make Q&A agent available within the UI
- [ ] Deploy gastownhall as MCP server other agents can query

------

## Phase 5: Sustainability

### 5.1 Non-Monetization Strategy

Steve's philosophy: turned down money to work on what he wants.

- [x] Confirm decision: keep the community free
- [ ] If monetization ever happens, keep it separate from core community resources

### 5.2 Succession Planning

- [ ] Document how everything is set up (this doc is a start)
- [ ] Add 1-2 trusted co-admins to all platforms
- [ ] Store credentials in shared secure location
- [ ] Write "in case of emergency" instructions
- [ ] Identify potential successors in the community

### 5.3 Legal Housekeeping

- [ ] Create privacy policy for gastownhall.ai
- [ ] Create terms of service
- [ ] Add DMCA contact information
- [ ] Add clear "community-run" disclaimers everywhere
- [ ] Ensure GDPR compliance if using analytics

## Quick Reference: Immediate Action Items

### Right Now

- [ ] Finalize Discord channel structure
- [ ] Create all channels per checklist above
- [ ] Create all roles
- [ ] Post welcome message
- [ ] Post Code of Conduct
- [ ] Send Steve the Discord invite

### Next

- [ ] Create landing page for gastownhall.ai
- [ ] Set up Cloudflare Pages
- [ ] Configure gastownhall.com redirect
- [ ] Post first X thread — a LAUNCH, not an announcement

### Soon

- [ ] Start docs site structure
- [ ] Begin curating content
- [ ] Create EHI work items for tracking
- [ ] Spec out Q&A agent architecture

### On Deck

- [ ] Gas Town Con planning
- [ ] Contributor recognition program details
- [ ] Content creator outreach

------

## Appendix A: Assets Inventory

| Property              | Status    | Purpose                                       |
| --------------------- | --------- | --------------------------------------------- |
| gastownhall.ai        | ✅ Owned   | Primary web presence, docs, eventually the UI |
| gastownhall.com       | ✅ Owned   | Redirect to .ai                               |
| Discord server        | ✅ Created | Community hub, real-time help                 |
| X (@gastownhall)      | ✅ Created | News, tips, community showcase                |
| gastownhall@gmail.com | ✅ Created | Account recovery, newsletter, contact         |
| GitHub (gastownhall)  | ✅ Got it! | UI repo, community contributions              |

------

## Appendix B: Cloudflare Hosting

You're already in Cloudflare. Two paths:

**Option A: Cloudflare Pages** (simpler)

- Free tier: unlimited sites, requests, bandwidth
- Connect to GitHub repo, auto-deploys on push
- Or direct upload a zip
- Great for static docs site

**Option B: Cloudflare Workers with Static Assets** (more flexible)

- The "new" recommended approach
- Simple wrangler.json config pointing to a directory
- Better if you want dynamic functionality later (Q&A agent API endpoint?)

**Recommendation:** Start with Pages for gastownhall.ai docs site. Migrate to Workers later if you need dynamic features.

**For the redirect (gastownhall.com → gastownhall.ai):**

- Cloudflare Page Rules or Redirect Rules
- Single rule: `*gastownhall.com/*` → `https://gastownhall.ai/$2` (301)

## Appendix C: Discord Welcome Message

```markdown
# Welcome to Gas Town Hall ⛽

The unofficial community hub for Steve Yegge's Gas Town multi-agent orchestrator.

**This is community-run** — a place for people wrangling robot chimps to help each other.

## Essential Links
🔗 [Welcome to Gas Town](https://steve-yegge.medium.com/welcome-to-gas-town-4f25ee16dd04) — Steve's intro (start here)
🔗 [Emergency User Manual](https://steve-yegge.medium.com/gas-town-emergency-user-manual-cf0e4556d74b) — when things go sideways
🔗 [GitHub](https://github.com/steveyegge/gastown)
🔗 [Beads](https://github.com/steveyegge/beads) — the memory system underneath
🔗 [gastownhall.ai](https://gastownhall.ai) — docs, tutorials, and eventually the UI
🔗 [@gastownhall on X](https://x.com/gastownhall) — news and tips

## Before You Dive In

Steve's warning is real: **Gas Town requires Stage 6-7+ experience** with AI coding agents.

> Gas Town is an industrialized coding factory manned by superintelligent robot chimps, and when they feel like it, they can wreck your shit in an instant.

If you're not already running 5-10+ agents and comfortable with chaos, Gas Town will hurt. No shame — come hang out, learn, watch others work. Check out #leveling-up if you're on your way to Stage 7.

## Channels
📢 #announcements — launches, news, Steve's posts
💬 #general — main conversation  
🛠️ #troubleshooting — questions, debugging
🏆 #showcase — share what you're building
🎓 #leveling-up — working toward Stage 7

## Rules
1. Be helpful, not condescending
2. Search before asking — your question might be answered
3. Share your wins AND your failures — we learn from both
4. No API keys, credentials, or sensitive info
5. Keep the chaos constructive

We read every message. We're here to help. Welcome to the ⛽ Town Hall!
```

------

## Appendix D: Code of Conduct

```markdown
# Gas Town Hall Code of Conduct

## The Short Version
Be excellent to each other.

## The Longer Version

**1. Respect experience levels**
People arrive at different stages. If someone asks a basic question, point them to resources kindly or let someone else answer. Don't mock. Everyone was Stage 1 once. Today's beginner is tomorrow's contributor.

**2. Help each other debug**
Gas Town breaks. A lot. Share your solutions, workarounds, and war stories. What you learned the hard way might save someone else hours (and dollars).

**3. Keep it constructive**
Criticism of tools, approaches, or code is welcome. Personal attacks are not. "This design has problems because X" is good. "You're an idiot" is not.

**4. Be transparent**
This is a community of engineers. We smell BS from a mile away. If something doesn't work, say so. If you don't know, say so. Honesty builds trust.

**5. No spam or low-effort self-promotion**
Sharing your gastown-related project: great! Dropping links to unrelated stuff: not great.

**6. Protect secrets**
Never share API keys, credentials, or sensitive information. If you see someone do this accidentally, alert a mod.

**7. Respect the chaos**
Gas Town is experimental, fast-moving, and sometimes breaks spectacularly. That's part of the fun. Embrace it.

## Enforcement
Mods will warn, then mute, then ban. We'd rather not — just be decent.

## Contact
Issues? DM @csells or email gastownhall@gmail.com
```

------

## Draft: Terms of Service

```markdown
# Gas Town Hall Terms of Service

**Last updated:** [date]

## What This Is
Gas Town Hall is a community-run resource for users of Steve Yegge's Gas Town multi-agent orchestrator. We are not affiliated with Anthropic, Steve Yegge, or any official Gas Town project unless explicitly stated.

## No Warranties
Everything here is provided as-is. We make no guarantees about accuracy, availability, or suitability for any purpose. Gas Town itself comes with warnings about wrecking your shit — so does this community.

## Your Responsibilities
- Follow the Code of Conduct
- Don't share others' private information
- Don't use this community for illegal purposes
- Don't blame us when Deacon murders your other agents

## Our Rights
We may remove content or users who violate these terms or the Code of Conduct. We may use anonymized questions and discussions to improve community resources (like the Q&A agent).

## Privacy
We collect minimal data. See our Privacy Policy for details. We don't sell your information.

## Changes
We may update these terms. Continued use means acceptance.

## Contact
Questions? gastownhall@gmail.com
```

------

*Built with ⛽ by Chris and Eli*

*"The goal is always happy developers." — Chris Sells, Code Europe 2023*
