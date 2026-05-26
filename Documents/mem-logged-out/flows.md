# Possible Logged-Out Flows

## 1. Public Memory Search Flow
User searches for a person or ancestor
→ sees public memory results
→ previews memory metadata and contextual details
→ opens lightweight memory preview
→ attempts deeper interaction
→ receives lightweight sign-up overlay

**Purpose:**
Allow potential new users to discover public memories connected to a person and understand the value of Memories before account creation.

**Notes:**
- Logged-out experiences likely need to remain person-based rather than semantic-search driven
- Users will likely expect to search for a name first and explore connected memories
- Search results may need stronger metadata hierarchy and contextual previews
- Exploration should feel open while still maintaining intentional interaction boundaries

**Questions:**
- What metadata should be visible in search results?
- What interactions should require account creation?
- How much of a memory should be previewable?
- Should results feel more like cards, search rows, or mixed layouts?
- How should memory previews connect back into continued exploration?

---

## 2. Historical Story Campaign Flow
User lands on featured historical story or curated campaign
→ explores related memories and people
→ views connected historical context
→ continues discovery through related content
→ prompted to create account for deeper exploration

**Purpose:**
Create emotionally engaging discovery experiences that encourage curiosity and exploration through curated storytelling.

**Notes:**
- Could support seasonal, historical, or themed campaigns
- May help expose public memories outside traditional search behavior
- Could connect into existing search/discovery systems

**Questions:**
- How curated should campaigns feel?
- Should stories connect directly into public memory search?
- What makes a historical story emotionally engaging?
- How much exploration should happen before account prompts appear?

---

## 3. Person Preview Flow
User searches for a person
→ views person preview experience
→ explores connected memory highlights
→ navigates into related memories and records
→ receives account prompts for deeper interaction

**Purpose:**
Support exploration continuity between person discovery and public memories.

**Notes:**
- This flow may involve collaboration with teams outside Memories
- Important to consider how memory discovery integrates into existing person experiences
- Opportunity to improve continuity between people, memories, and discovery pathways

**Questions:**
- How should memories surface within person preview experiences?
- What interactions belong to Memories vs other teams?
- How can memory discovery feel connected rather than isolated?

---

# Interaction Models: Public Memory Search Flow

The following models explore different strategic approaches to the Public Memory Search Flow. Each represents a distinct philosophy about how logged-out users should discover, preview, and engage with public memories before account creation.

---

## Model A: Generous Preview Model

**Philosophy:** Maximize openness and trust. Let users explore deeply before asking for commitment. Account prompts appear only at meaningful interaction boundaries (save, contribute, connect).

### Key Characteristics

**Search Results:**
- Rich card-based layout with prominent imagery
- Full metadata visible: dates, locations, relationships, memory type, contributor
- Preview snippets of stories/descriptions (first 2-3 lines)
- "X more memories" badges to show collection depth

**Memory Preview:**
- Full images/documents viewable at high resolution
- Complete stories and descriptions readable
- All contextual metadata exposed (who, what, when, where)
- Related memories visible and clickable
- Tagged people and places navigable

**Account Gating:**
- Triggered by: saving memories, adding to collections, contributing content, connecting memories to family tree
- NOT triggered by: viewing, reading, navigating, exploring relationships
- Overlay-based prompts that preserve context ("Sign in to save this memory to your collection")

**Exploration Continuity:**
- Seamless navigation between memories, people, and related content
- "Related memories" and "More from this contributor" recommendations
- Breadcrumb trail showing exploration path
- No interruption until user attempts to "claim ownership" of content

### User Journey

1. User searches "John Smith 1890 Ohio"
2. Sees 47 results in card layout, each showing thumbnail, date range, location, memory type
3. Clicks memory card → full preview opens (full image, complete story, all metadata)
4. Explores tagged people → navigates to related person's memories
5. Continues exploring 4-5 more memories freely
6. Attempts to click "Save to my memories" → overlay appears: "Create a free account to save and organize memories"
7. User can dismiss and continue exploring, or sign up

### Tradeoffs & Implications

**Optimizes for:**
- Discovery and exploration momentum
- Building trust through openness
- Demonstrating value before asking for commitment
- Reducing friction for curious users

**Sacrifices:**
- Lower conversion pressure (fewer account prompts)
- Risk of users "browsing forever" without converting
- Potential confusion about what requires an account
- May not create sufficient motivation to sign up

**Open Questions:**
- Does this feel "too open" and reduce urgency to create an account?
- What percentage of users will explore extensively but never convert?
- How do we measure value of exploration vs conversion?
- Could this model inadvertently communicate that an account isn't necessary?

---

## Model B: Contextual Teaser Model

**Philosophy:** Show enough to spark curiosity, but maintain clear boundaries. Rich metadata creates context, but content access requires engagement. Account prompts are frequent but contextual.

### Key Characteristics

**Search Results:**
- Mixed layout: image-forward cards with metadata hierarchy
- Essential metadata visible: dates, locations, contributor, memory type
- Story/description previews truncated deliberately (first line + "...")
- Visual emphasis on imagery with subtle "preview" indicators

**Memory Preview:**
- Medium-resolution images (enough to see, not enough for full detail)
- Story/description text truncated at meaningful cliffhanger point
- Core metadata exposed, but relationships/connections summarized ("3 tagged people")
- "Sign in to see full memory" persistent but non-blocking CTA

**Account Gating:**
- Triggered by: viewing full content, exploring relationships, seeing tagged people, viewing high-res images
- Progressive prompts: first interaction = gentle overlay, subsequent = more prominent
- Context-specific messaging: "Sign in to see who is tagged in this photo"

**Exploration Continuity:**
- Limited lateral navigation (can see related memories exist, but need login to explore)
- "Related memories" count visible but links gated
- Each interaction checkpoint includes subtle account prompt
- Breadcrumbs show where you've been, but not deep exploration paths

### User Journey

1. User searches "Mary Johnson 1920 immigration"
2. Sees 23 results in mixed card layout showing thumbnails, dates, locations
3. Clicks memory → preview shows medium-res image, truncated story ("Mary arrived at Ellis Island on July 4, 1920, carrying only...")
4. Attempts to click "3 tagged people" → overlay: "Create account to see tagged family members and explore connections"
5. Dismisses prompt, scrolls to related memories section
6. Sees "8 related memories" but clicking any triggers prompt: "Sign in to continue exploring Mary's story"
7. After 2-3 prompts, user either converts or bounces

### Tradeoffs & Implications

**Optimizes for:**
- Conversion momentum (frequent, contextual prompts)
- Creating curiosity gaps ("what happens next?")
- Establishing clear value boundaries
- Balancing preview with incentive to sign up

**Sacrifices:**
- Exploration flow (more interruption)
- Trust (may feel restrictive or "gatekeepy")
- Discovery depth (users can't explore broadly before committing)
- Risk of frustrating users with too many prompts

**Open Questions:**
- What's the right truncation point for stories/descriptions?
- How many prompts before user experience degrades?
- Does this feel too similar to competitor patterns we're trying to avoid?
- How do we measure optimal prompt frequency?

---

## Model C: Progressive Discovery Model

**Philosophy:** Reveal depth gradually based on engagement. Early exploration is open, but deeper interactions require progressive commitment. Experience adapts to user behavior.

### Key Characteristics

**Search Results:**
- Adaptive layout: starts minimal (rows), expands to cards as user engages
- Initial metadata: basic info (name, date, type), expands on hover/focus
- First 3-5 results fully accessible, deeper results require account
- Visual indicator of "exploration budget" (e.g., "5 previews remaining")

**Memory Preview:**
- First memory: full access (complete image, story, metadata, relationships)
- Second-third memories: high access (full content, limited relationship exploration)
- Fourth-fifth memories: medium access (preview-level content)
- Sixth+ memories: summary only, full content gated
- Preview budget resets daily or per search session

**Account Gating:**
- Triggered by: exploration depth (number of memories viewed), relationship navigation depth, time on site
- Adaptive prompting: "You've explored 5 memories. Sign in to continue your discovery."
- Value-reinforcing: "You've viewed memories from 1890-1920. Create an account to build your family timeline."

**Exploration Continuity:**
- First few memories allow full lateral navigation
- Relationship exploration becomes progressively summarized
- "Map" of exploration path visible, showing where you've been and what's gated
- After account creation, resume exactly where user left off

### User Journey

1. User searches "Robert Wilson Civil War"
2. Sees first 5 results in expandable row format
3. Clicks first memory → full access (complete story, all metadata, can explore tagged people)
4. Explores second memory → full access but notices "3 previews remaining" indicator
5. Views third memory → still full access, "2 previews remaining"
6. Clicks fourth memory → sees preview-level content, overlay: "You've explored 3 memories. Sign in to continue discovering Robert's story and explore unlimited memories."
7. Can dismiss and view one more preview, or sign up to continue

### Tradeoffs & Implications

**Optimizes for:**
- Balancing openness with conversion
- Demonstrating value through experience
- Creating natural stopping points
- Rewarding engagement with access

**Sacrifices:**
- Complexity (users must understand progressive access)
- Potential confusion about what they can access
- Risk of feeling like a "trial" or "metered paywall"
- Harder to implement and communicate

**Open Questions:**
- What's the right number of previews before gating?
- Should budget reset, and if so, when?
- How do we communicate the progressive model without feeling like a trial?
- Does this feel game-ified in a way that doesn't fit the emotional context?

---

## Model D: Guided Exploration Model

**Philosophy:** Create curated paths that demonstrate value while maintaining intentional boundaries. Users follow suggested journeys rather than free-form exploration. Account prompts at natural story milestones.

### Key Characteristics

**Search Results:**
- Story-driven card layout emphasizing narrative connections
- Metadata organized by themes: "Robert's military service," "Robert's family life"
- Suggested exploration paths: "Follow Robert's Civil War journey" or "Explore Robert's descendants"
- Grouped results with clear starting points

**Memory Preview:**
- Curated sequences: "Memory 1 of 4 in Robert's Civil War journey"
- Full access to current memory in sequence
- Preview of "next memory" in journey
- Related memories outside path shown as locked/gated

**Account Gating:**
- Triggered by: completing a curated sequence, attempting to leave suggested path, exploring outside guided journey
- Narrative prompts: "You've discovered Robert's enlistment and first battle. Sign in to continue his story."
- Path-completion incentive: "Sign in to unlock 12 more memories in this collection"

**Exploration Continuity:**
- Linear progression through curated paths
- Branch points: "Continue military service journey" or "Explore family life"
- Off-path exploration gated but visible
- Account prompt positions as "unlocking the full story"

### User Journey

1. User searches "Sarah Martinez California 1950s"
2. Sees results grouped by theme: "Sarah's immigration journey," "Sarah's family in California," "Sarah's work life"
3. Clicks "Sarah's immigration journey" → enters curated sequence
4. Views Memory 1: border crossing photo, full story, "Next: arrival in California"
5. Continues to Memory 2: arrival documentation, full access
6. Continues to Memory 3: first home photo, full access
7. Reaches end of preview sequence: "You've seen the beginning of Sarah's journey. Sign in to explore 9 more memories and discover what happened next."
8. Can start a different path or sign up to continue

### Tradeoffs & Implications

**Optimizes for:**
- Emotional engagement through storytelling
- Demonstrating clear value and narrative arc
- Creating natural conversion moments
- Reducing choice paralysis

**Sacrifices:**
- User agency (less free exploration)
- Breadth of discovery (focused paths vs broad scanning)
- Requires curation effort and smart grouping
- May not work well for searches with limited results

**Open Questions:**
- How do we create curated paths programmatically?
- What happens when search results don't fit narrative groupings?
- Does this feel too prescriptive for users who want to browse?
- How do we balance curation with search result accuracy?

---

## Comparative Summary

| Dimension | Generous Preview | Contextual Teaser | Progressive Discovery | Guided Exploration |
|-----------|------------------|-------------------|----------------------|-------------------|
| **Search Result Density** | Rich cards | Mixed cards | Adaptive rows→cards | Story-driven groups |
| **Memory Preview Depth** | Full access | Truncated/medium | Progressive (full→medium→summary) | Full within path |
| **Account Gating Frequency** | Rare (save/contribute only) | Frequent (contextual) | Graduated (by count) | At story milestones |
| **Exploration Freedom** | Maximum | Limited | Medium (budget-based) | Guided paths |
| **Conversion Pressure** | Low | High | Medium-High | Medium |
| **Discovery Momentum** | High | Medium | Medium | High (within paths) |
| **Complexity** | Low | Low | Medium | Medium-High |
| **Best For** | Trust-building, engagement | Quick conversion, clear boundaries | Balancing access & conversion | Storytelling, emotional engagement |

---

## Cross-Cutting Questions

These questions apply across all models and need exploration regardless of direction:

### Metadata & Content Questions
- What metadata is essential vs nice-to-have in search results?
- How do we handle missing metadata gracefully?
- What makes a memory feel "complete" vs "broken" in preview?
- How do different memory types (photo, document, story, audio) affect preview strategies?

### Technical & Implementation Questions
- How do we determine what's "public" vs "private" for logged-out viewing?
- What's the relationship between memory permissions and logged-out access?
- How do we handle memories with sensitive or incomplete information?

### Measurement & Success Questions
- What metrics matter: exploration depth, time on site, conversion rate, return visits?
- How do we measure "value demonstrated" before conversion?
- What's the right balance between exploration and conversion?

### Competitive Context Questions
- How much more open should FamilySearch be compared to competitors?
- What patterns from competitors should we avoid?
- Where is there opportunity to differentiate through openness?

---

# Hybrid Interaction Models

These models synthesize elements from the core models above, combining generous metadata previews, progressive interaction gating, and guided exploration pathways. Each hybrid is evaluated for alignment with FamilySearch's nonprofit, discovery-oriented mission.

---

## Hybrid 1: Open Discovery with Progressive Depth

**Synthesis:** Combines generous metadata (Model A) + progressive gating (Model C) + light guidance (Model D)

**Philosophy:** Lead with radical openness and trust. Let users explore broadly and deeply, but introduce gentle boundaries as engagement deepens. Suggest paths without constraining freedom.

### How It Works

**Search Results:**
- Rich, generous card layout with full metadata visible
- All results accessible (no artificial limits on result viewing)
- Visual grouping suggestions: "Memories from the 1940s," "Military service," "Family photos" - but user can ignore groupings
- Prominent imagery with complete context (dates, locations, relationships, contributors)

**Memory Preview - First Phase (Memories 1-5):**
- Full access: complete images at high resolution, entire stories/descriptions
- All metadata exposed and interactive (tagged people are clickable, locations are explorable)
- Related memories fully navigable
- Suggested exploration paths visible but optional: "Continue exploring Mary's immigration story →" or "See more memories from this time period"
- No account prompts - just pure discovery

**Memory Preview - Second Phase (Memories 6-10):**
- Still generous access to content (full stories, full images)
- Relationship navigation becomes summarized: can see tagged people but need account to explore their memories
- Gentle, non-blocking indicator: "You're discovering a lot! Sign in to save your exploration and connect memories to your family tree"
- Suggested paths become slightly more prominent but still optional

**Memory Preview - Third Phase (Memory 11+):**
- Content access remains full (can still read complete stories, view full images)
- Account prompt becomes more present but still contextual: "You've explored 11 memories spanning 1890-1950. Create a free account to save your discoveries and contribute your own family stories"
- Lateral navigation (related memories, tagged people) requires account
- "Resume your exploration" promise: show map of what they've discovered, offer to save it

**Account Gating Strategy:**
- **Never gates:** viewing content, reading stories, seeing images, exploring initial relationships
- **Progressively gates (11+ memories):** deep relationship navigation, cross-collection exploration
- **Always gates:** saving, contributing, connecting to family tree, advanced features
- Messaging emphasizes **preservation and contribution**, not restriction: "Sign in to save these discoveries and help preserve family stories"

**Exploration Continuity:**
- Full freedom of movement through first 10 memories
- Breadcrumb trail shows exploration path
- "Discovery map" visualizes what they've found (timeline, people, locations)
- Suggested paths feel like helpful suggestions, not requirements
- After account creation, everything they explored is immediately available in their history

### User Journey

1. User searches "Emma Rodriguez 1930s Los Angeles"
2. Sees 31 results in rich card layout - all metadata visible, grouped by theme but browsable freely
3. Clicks first memory → full access, sees complete story about Emma's arrival in LA, high-res photo, can click tagged people
4. Explores tagged person → navigates to husband's memories, views his stories
5. Continues exploring 4 more memories across different people and time periods - no interruption
6. Views 6th memory → still full access, subtle indicator appears: "You're building quite a discovery journey! Sign in anytime to save your progress"
7. Explores through memory 10 → can still view all content, but clicking "8 related memories" shows summary instead of full navigation
8. Views 11th memory → fuller prompt appears: "You've explored 11 memories from Emma's community. Sign in to keep exploring and save these discoveries to your family tree"
9. Can dismiss and continue viewing content, but relationship navigation now requires account

### Alignment with FamilySearch Mission

**Strong Alignment:**
- ✅ **Nonprofit values:** Trust-first approach, no aggressive conversion tactics
- ✅ **Discovery-oriented:** Supports broad, free exploration without artificial limits
- ✅ **Educational:** Users can learn deeply about family history before committing
- ✅ **Community focus:** Account prompts emphasize contribution and preservation, not consumption
- ✅ **Differentiation:** More open than competitors while maintaining conversion path

**Potential Tensions:**
- ⚠️ Lower immediate conversion rate (users can explore extensively before prompt)
- ⚠️ Requires confidence that demonstrated value will drive conversion
- ⚠️ Risk of users feeling "why do I need an account?" after deep exploration

**Best For:**
- Users genuinely curious about family history (not casual browsers)
- Building trust with potential long-term contributors
- Differentiating from commercial competitors
- Supporting serendipitous discovery

---

## Hybrid 2: Guided Generosity Model

**Synthesis:** Combines guided paths (Model D) + generous preview (Model A) + contextual gating (Model B)

**Philosophy:** Curate emotionally resonant discovery journeys while maintaining generous access within those journeys. Account boundaries appear at natural story milestones, but always preserve momentum.

### How It Works

**Search Results:**
- Story-driven organization: results grouped into narrative themes
- Within each theme: generous metadata and imagery
- Clear suggested starting points: "Start with Emma's arrival story" or "Explore Emma's family life"
- Can view all themes and browse freely, but paths provide structure

**Memory Preview within Guided Path:**
- **Full generosity within the path:** complete stories, high-res images, all metadata
- Path shows progression: "Memory 2 of 5 in Emma's immigration journey"
- Each memory fully accessible, explorable, and emotionally complete
- Related memories *outside* the current path shown as "More to explore" with preview cards
- Suggested next steps within path: "Continue to Emma's first job" or "Explore her children's stories"

**Memory Preview outside Guided Path:**
- Can browse outside suggested paths at any time
- First 2-3 off-path explorations: full access (same as on-path)
- Additional off-path memories: generous preview (full metadata, medium-res images, truncated stories with "Sign in to read Emma's complete story")
- Gentle nudge to return to path: "Return to Emma's journey" or "Start a new guided story"

**Account Gating Strategy:**
- **Within path (first complete journey):** No gating until natural story endpoint
- **At journey completion:** Contextual prompt tied to narrative arc: "You've discovered Emma's arrival and first years in America. Sign in to explore what happened next and discover 8 more memories from her life"
- **Off-path exploration:** Progressive gating after 2-3 memories
- **Always gates:** Saving, contributing, creating your own paths

**Exploration Continuity:**
- Paths provide structure but never trap users
- Can jump between paths, browse freely, or follow suggestions
- "Your journey" map shows which paths you've started/completed
- After account creation, all started journeys preserved with progress markers

### User Journey

1. User searches "James Chen San Francisco 1960s"
2. Results organized into themes: "James' immigration," "James' Chinatown community," "James' business life"
3. Clicks "James' immigration journey" → enters 5-memory curated path
4. Memory 1: Departure from Hong Kong - full story, full access, emotional context
5. Memory 2: Ship manifest document - high-res, fully readable, tagged people explorable
6. Memory 3: Arrival photo at SF port - complete access
7. Becomes curious about a tagged person (friend who traveled with him) - clicks to explore
8. Views friend's memories (off-path) - first 2 have full access
9. Returns to James' path, continues to Memory 4: First apartment
10. Completes 5-memory path → prompt: "You've followed James from Hong Kong to his first home in San Francisco. Sign in to continue his story and discover 12 more memories from his life in Chinatown"
11. Can start new path, browse freely, or sign up

### Alignment with FamilySearch Mission

**Strong Alignment:**
- ✅ **Storytelling:** Emphasizes emotional narrative and human connection
- ✅ **Discovery-oriented:** Paths encourage learning and curiosity
- ✅ **Generous within boundaries:** Full access within structured experiences
- ✅ **Preservation focus:** Account prompts tied to continuing/preserving stories
- ✅ **Accessible:** Structure helps users who might feel overwhelmed by open-ended search

**Potential Tensions:**
- ⚠️ Requires curation effort (how to create paths programmatically?)
- ⚠️ May not suit all search contexts (sparse results, non-narrative searches)
- ⚠️ Could feel prescriptive for users who want pure browse/search

**Best For:**
- Searches with rich, narrative-worthy results
- Users who respond to storytelling and emotional context
- Supporting discovery for users unfamiliar with family history research
- Creating shareable, campaign-style experiences

---

## Hybrid 3: Trust-Based Progressive Discovery

**Synthesis:** Combines generous metadata (Model A) + progressive depth (Model C) + narrative framing (Model D)

**Philosophy:** Earn trust through radical openness, then transition to partnership. Frame account creation as unlocking collaboration and contribution, not just continued access.

### How It Works

**Search Results:**
- Extremely generous: rich cards, all metadata, full context
- Results include narrative hints: "12 memories tell Maria's story from 1915-1960"
- No artificial restrictions or preview limits in results view
- Subtle value indicators: "Maria's memories have been viewed 1,200 times and helped 47 people discover their family history"

**Memory Preview - Trust-Building Phase (First 3-5 memories OR first 10 minutes):**
- **Completely unrestricted:** Full images, complete stories, all metadata, all relationships explorable
- Suggested narrative connections visible: "This memory connects to Maria's daughter's story" or "See how this relates to the 1920 census"
- Educational context provided: timeline overlays, historical context, relationship explanations
- Zero account prompts - building trust through value demonstration

**Memory Preview - Partnership Invitation Phase (After trust phase):**
- Content access remains full (stories, images, metadata still complete)
- Contextual value-adds become gated: "Sign in to see how this connects to historical records" or "Create account to view Maria's full timeline"
- Relationship navigation shifts from open to summarized
- Messaging shifts from "view more" to "contribute and collaborate": 
  - "You've discovered Maria's story. Join FamilySearch to help preserve family histories like hers."
  - "These memories were contributed by people like you. Sign in to add yours."

**Memory Preview - Collaboration Phase (After 15+ memories OR 20+ minutes):**
- Full content access continues (never gates stories/images from public memories)
- Advanced features gated: timeline building, connection discovery, cross-collection search
- Strong partnership framing: "You've spent 20 minutes exploring family histories. Create a free account to save your research and help others discover their stories."
- Social proof: "50,000 people contributed memories last month. Add your family's story."

**Account Gating Strategy:**
- **Never gates:** Public memory content, stories, images, basic metadata
- **Time/depth-based gating:** Advanced navigation, relationship mapping, collection features
- **Always gates:** Contributing, saving, connecting to tree, advanced research tools
- Messaging evolution: Exploration → Education → Partnership → Contribution

**Exploration Continuity:**
- Seamless throughout - gating never interrupts viewing flow
- "Research journal" automatically created showing everything explored
- Account creation positioned as "save your research" not "unlock more content"
- Explicit promise: "Everything you've discovered will be waiting for you"

### User Journey

1. User searches "Giuseppe Rossi Italy immigration"
2. Sees 28 rich results with complete metadata and narrative framing: "Giuseppe's journey from Sicily to New York, 1905-1950"
3. Spends 8 minutes freely exploring 4 memories: ship manifests, arrival photos, naturalization papers, family letters
4. All content fully accessible, can navigate all relationships, educational context provided
5. Views 5th memory → subtle indicator appears: "You've built quite a research collection! Sign in anytime to save your discoveries and contribute your family's story"
6. Continues exploring, now 12 minutes in, viewed 7 memories
7. Attempts to click "View Giuseppe's full timeline" → overlay: "Timeline features require a free account. Join 2 million family historians preserving memories together."
8. Dismisses, continues viewing memories (content still fully accessible)
9. After 20 minutes and 10 memories: More prominent prompt: "You've spent 20 minutes researching Giuseppe's story. FamilySearch is free because people like you contribute. Create an account to save your research and add your family's memories."
10. Decision point: save research by signing up, or continue browsing with advanced features gated

### Alignment with FamilySearch Mission

**Strongest Overall Alignment:**
- ✅✅ **Nonprofit values:** Radical trust, education-first, zero aggressive tactics
- ✅✅ **Discovery-oriented:** Maximum support for learning and exploration
- ✅✅ **Mission-driven messaging:** Account prompts emphasize contribution and community, not consumption
- ✅✅ **Differentiation:** Dramatically more open than competitors while maintaining conversion path
- ✅ **Sustainable:** Converts serious researchers while respecting casual browsers
- ✅ **Authentic:** Never feels like artificial restriction or commercial pressure

**Potential Tensions:**
- ⚠️ Lowest immediate conversion rate (most generous model)
- ⚠️ Requires strong belief that value demonstration drives conversion
- ⚠️ Success depends on content quality and meaningful discoveries

**Best For:**
- FamilySearch's nonprofit mission and values
- Building long-term community members, not just accounts
- Users who will become contributors and advocates
- Differentiating through trust and openness

---

## Hybrid Comparison: Mission Alignment

| Model | Openness | Conversion Strategy | Mission Alignment | Best For |
|-------|----------|---------------------|-------------------|----------|
| **Hybrid 1: Open Discovery with Progressive Depth** | High (full access 1-10, content access continues) | Gradual depth-based gating | ✅✅ Strong - Trust-first, discovery-focused | Balanced approach, broad user base |
| **Hybrid 2: Guided Generosity** | High within paths, medium outside | Story milestone gating | ✅ Good - Narrative-driven, accessible | Curated experiences, storytelling |
| **Hybrid 3: Trust-Based Progressive Discovery** | Highest (content never gated) | Time/partnership-based | ✅✅✅ Strongest - Mission-driven, community-focused | Nonprofit values, long-term community building |

---

## Recommendation: Hybrid 3 with Hybrid 1 Elements

**Rationale:**

**Hybrid 3 (Trust-Based Progressive Discovery)** most authentically embodies FamilySearch's nonprofit, discovery-oriented mission:

1. **Never gates public memory content** - Stories, images, and basic metadata remain accessible indefinitely
2. **Trust-first approach** - Builds value through unrestricted exploration before asking for commitment
3. **Mission-driven account prompts** - Emphasizes contribution, preservation, and community over consumption
4. **Sustainable differentiation** - Dramatically more open than competitors while maintaining clear conversion path
5. **Partnership framing** - Account creation positioned as joining a community, not unlocking restricted content

**Enhanced with Hybrid 1 elements:**

- Progressive gating at specific memory counts (10-15) provides clearer structure
- Depth-based triggers supplement time-based triggers for users who explore quickly
- Relationship navigation gating (from Hybrid 1) provides tangible benefit to account creation

### Refined Hybrid: Trust-Based Discovery with Progressive Relationships

**Core principles:**
- Public memory content (stories, images, core metadata) never gated
- First 5 memories: completely unrestricted (including full relationship navigation)
- Memories 6-10: content unrestricted, relationship navigation summarized
- Memory 11+: content unrestricted, advanced features (timelines, connections, cross-collection) gated
- Always gates: saving, contributing, connecting to tree

**Account messaging evolution:**
- Memories 1-5: Silent (building trust)
- Memory 6: Gentle indicator ("Sign in anytime to save your discoveries")
- Memory 11: Partnership invitation ("Join our community of 2M family historians")
- 20+ minutes: Mission-driven ask ("Help preserve family stories like the ones you've discovered")

**Value demonstration:**
- Educational context throughout (historical timelines, relationship explanations)
- Show impact: "These memories have helped X people discover their history"
- Social proof: "Y memories contributed this month"
- Contribution focus: "Your family's story matters"

---

## Implementation Considerations

### For Public Memory Search specifically:

**Search Results Page:**
- Rich card layout with complete visible metadata
- Narrative grouping suggestions (optional, not required)
- Zero restrictions on result viewing or clicking
- Value indicators (view counts, community contributions) visible

**Memory Preview Experience:**
- Full content access regardless of depth (stories fully readable, images high-resolution)
- Progressive relationship navigation: free initially, summarized after depth threshold
- Educational overlays and context remain accessible
- Account prompts non-blocking, dismissible, contextual

**Exploration Continuity:**
- Automatic "research journal" tracking exploration path
- Seamless navigation within content access boundaries
- Clear, honest communication about what requires an account (advanced features, not content)
- "Save your research" positioning for account creation

### Technical Requirements:

- Tracking exploration depth (memory count, time, relationship navigation depth)
- Progressive prompt system with contextual messaging
- Research journal / exploration history generation
- Post-signup experience that immediately shows saved exploration

### Success Metrics:

**Primary:**
- Account conversion rate (quality over speed)
- Contributor conversion rate (accounts that add memories)
- Time to first contribution
- Return visit rate

**Secondary:**
- Exploration depth before conversion
- Memory views per session
- Relationship navigation patterns
- Prompt dismissal vs conversion rates

**Mission metrics:**
- Community contribution volume
- Cross-user memory connections
- Educational engagement (timeline views, context clicks)

---

---

# Refinements Based on Review

## Critical Question: Should Public Memories Ever Be Gated?

**The core tension in Hybrid 1:** If memories are already marked as public, artificially limiting access based on view count feels inconsistent and potentially confusing.

**Arguments against gating public memories:**
- **Logical consistency:** "Public" should mean accessible, not "public but only X at a time"
- **User trust:** Arbitrary limits feel like commercial tactics, not nonprofit values
- **Mission alignment:** FamilySearch's mission is to make records freely accessible
- **Technical reality:** The memory is already public - the gating is artificial

**Arguments for some form of gating:**
- **Conversion necessity:** Need to create motivation for account creation
- **Value demonstration:** Without boundaries, why sign up?
- **Feature differentiation:** What does an account enable if everything is free?

**Proposed resolution:** 
**Public memory CONTENT is never gated. Advanced FEATURES and CAPABILITIES are gated.**

This shifts the model from "unlock more content" to "unlock more capabilities" - which feels more authentic to FamilySearch's mission.

---

## Defining "Advanced Features" in Memories Context

What requires an account vs. what should be freely accessible?

### Should Be Free (Public Memory Access):
- **Viewing memory content:** Full stories, complete descriptions, all text
- **Viewing images/documents:** High-resolution, full quality
- **Reading metadata:** Dates, locations, people names, contributors, descriptions
- **Basic navigation:** Clicking between related memories, exploring one level of relationships
- **Educational context:** Historical timelines, location information, event context

### Should Require Account (Advanced Features & Participation):
- **Saving & organizing:** Save to collections, bookmark, create research sets
- **Contributing:** Upload memories, add stories, attach to people
- **Connecting:** Link memories to family tree, suggest connections
- **Downloading:** Download high-res originals, export collections
- **Engaging:** Comment, react, share privately, tag people
- **Advanced navigation:** Build cross-collection timelines, deep relationship mapping (3+ hops)
- **Research tools:** Search within collections, filtered searches, advanced discovery
- **Collaboration:** Share with family, co-edit stories, invite family members

### Gray Areas (Needs Decision):
- **Tagging/attribution:** Viewing who is tagged vs. exploring those people's memories
- **Related memories:** Seeing that related memories exist vs. navigating to them
- **Downloads:** View high-res in browser vs. download file
- **Social features:** See engagement counts (views, likes) vs. engage yourself

**Key principle:** Free access to content and one-level exploration. Account required for participation, saving, deep research, and multi-hop navigation.

---

## Hybrid 2 Clarification: What Does "Guided" Actually Mean?

**Current confusion:** Is this like Ancestry's curated historical stories? How are paths created? What's the actual user experience?

### Two Possible Interpretations:

**Interpretation A: Curated Historical Campaigns (Like Ancestry)**
- Editorial team creates featured stories: "Women in WWII," "Immigration at Ellis Island," "Pioneer Stories"
- Landing pages showcase these campaigns
- Memories manually selected and ordered into narrative sequences
- More like Historical Story Campaign Flow (Flow #2) than a search result pattern

**Interpretation B: Dynamic Path Suggestion from Search**
- User searches normally: "Maria Gonzalez 1940s Texas"
- System analyzes results and suggests narrative groupings programmatically
- Paths are generated from search results: "Maria's work life," "Maria's family," "Maria in World War II"
- User can follow suggested paths or browse freely

**Likely intent was Interpretation B** - but this requires:
- Smart grouping algorithms (by date ranges, tagged people, memory types, locations)
- Enough result density to create meaningful paths
- Fallback for sparse results

### Hybrid 2 Revised Description:

**Guided Generosity = Smart Grouping + Full Access Within Groups + Contextual Gating Between Groups**

**How it actually works:**

1. User searches "James Chen San Francisco"
2. Search returns 24 memories
3. System groups results into themes:
   - "James' immigration journey" (5 memories, 1952-1953)
   - "James' Chinatown community" (11 memories, 1955-1970)
   - "James' family life" (8 memories, 1960-1980)
4. User can browse all results freely OR follow a suggested path
5. **If following a path:** Full access to all memories in that grouping (5 memories about immigration = 5 fully accessible)
6. **If jumping between paths:** First jump is free, subsequent jumps show preview/prompt
7. **If browsing freely (ignoring paths):** Treated like Hybrid 1 or 3

**This model works best when:**
- Search results have enough density (10+ memories)
- Results have clear thematic or chronological groupings
- User is interested in narrative discovery vs. quick lookup

**This model struggles when:**
- Sparse results (1-3 memories)
- Results don't have clear groupings
- User wants specific memory, not storytelling journey

**Verdict:** Hybrid 2 might be better suited for Historical Story Campaign Flow rather than general memory search. For search, it adds complexity without clear advantage over Hybrid 1 or 3.

---

## Revised Hybrid Models

### Hybrid 1 Revised: Open Content, Progressive Features

**Changed from original:** No longer gates public memory content at any depth. Only gates advanced features progressively.

**Core principle:** Public memories are always accessible. Account value comes from features and capabilities, not content access.

**What's always free:**
- View unlimited public memory content (stories, images, metadata)
- Navigate one level of relationships (see tagged people, view their directly-related memories)
- Basic exploration (breadcrumb trail, related memories within one hop)

**What becomes gated progressively:**

**After 5 memories:**
- Gentle indicator appears: "Sign in to save your discoveries"
- Can still view all content, but saving/bookmarking requires account

**After 10 memories:**
- Multi-hop relationship navigation gated: "Sign in to explore Sarah's extended family connections"
- Deep research tools (timelines, connection maps) require account
- Downloading features gated

**After 15+ memories OR 20+ minutes:**
- Stronger prompt: "You're doing serious research! Create a free account to save your work and contribute your family's memories"

**Key difference from original Hybrid 1:** Content is never gated, only features. The progression is about demonstrating value of features (saving, organizing, deep research) not restricting access.

### Hybrid 3 Revised: Trust-First, Contribution-Focused

**Unchanged core principle:** Never gate public content. Frame account creation as participation and contribution.

**Refinement:** Clearer feature boundaries and messaging evolution.

**Always accessible:**
- All public memory content (unlimited viewing)
- Basic relationship exploration (1-2 hops)
- Educational context and metadata

**Progressive feature reveals (not gates - just introduces):**

**Memories 1-5:** Silent exploration
- No prompts, no indicators
- Full access to content and basic features
- Building trust through value

**Memory 6-10:** Subtle value indicators
- Non-blocking: "Sign in to save discoveries and contribute memories"
- Shows participation stats: "2,134 people added memories this week"
- Emphasizes community, not restriction

**Memory 11+ OR 15+ minutes:** Partnership invitation
- "You've discovered rich family history. Join FamilySearch to preserve and share your family's story"
- Gating becomes clearer for advanced features (deep relationship trees, advanced search, downloads)
- Contribution-focused: "Your family's memories matter too"

**Key messaging themes:**
- Preservation ("Help preserve stories like these")
- Community ("Join 2M family historians")
- Contribution ("Share your family's memories")
- Research tools ("Save and organize your discoveries")

**Never uses:**
- "Unlock more memories" (they're not locked)
- "See full content" (content is already visible)
- "Get unlimited access" (access is already unlimited for public content)

---

## Interaction Boundaries: Concrete Examples

Let me map specific interactions to clarify what requires accounts:

| Interaction | Free? | Requires Account? | Reasoning |
|-------------|-------|-------------------|-----------|
| View memory image (high-res) | ✅ Free | No | Public content should be accessible |
| Read complete story/description | ✅ Free | No | Public content should be accessible |
| See tagged people names | ✅ Free | No | Basic metadata |
| Click tagged person → view their profile | ✅ Free | No | One-hop navigation |
| Click tagged person → view their memories | ✅ Free (first few) | Progressive | One-hop content access |
| Navigate to friend-of-friend memories | ⚠️ Progressive | Yes (after depth) | Multi-hop deep exploration |
| See "15 related memories" | ✅ Free | No | Awareness of related content |
| Click to view those related memories | ✅ Free (first level) | Progressive (deep level) | One-hop free, multi-hop gated |
| Download image file | ❌ Account | Yes | File downloads = account feature |
| Save/bookmark memory | ❌ Account | Yes | Personal organization feature |
| Add to collection | ❌ Account | Yes | Personal organization feature |
| Build timeline across memories | ⚠️ Progressive | Yes (after demo) | Advanced research tool |
| Comment on memory | ❌ Account | Yes | Participation feature |
| Upload own memory | ❌ Account | Yes | Contribution feature |
| Share memory (link) | ✅ Free | No | Encourage distribution |
| Share to family privately | ❌ Account | Yes | Personal collaboration |
| See memory view count | ✅ Free | No | Social proof / value indicator |
| See who viewed | ❌ Account | Yes | Privacy-sensitive feature |

**Key patterns:**
- **Viewing and basic navigation:** Free
- **Organizing and saving:** Requires account
- **Contributing and engaging:** Requires account
- **Deep research and multi-hop:** Progressive (free initially, gated after depth)
- **Downloads and exports:** Requires account
- **Social/private features:** Requires account

---

## Recommendation: Hybrid 3 as Primary Model

**Why Hybrid 3 over Hybrid 1:**

1. **Mission alignment:** Most authentic to nonprofit values
2. **Messaging:** Focuses on contribution/community, not unlocking content
3. **User experience:** Never feels artificially restricted
4. **Differentiation:** Most distinct from commercial competitors
5. **Sustainability:** Converts serious researchers who become contributors

**Hybrid 1 vs Hybrid 3 key difference:**
- **Hybrid 1:** Progressive feature gating based on depth/count
- **Hybrid 3:** Gentle feature introduction based on time/engagement + contribution-focused messaging

Both never gate content, but Hybrid 3 frames account creation more positively.

**Proposed: Hybrid 3 with clearer feature boundaries and messaging**

---

## Next Steps: Prototyping & Mapping

Three distinct flow directions to explore:

### Direction 1: Trust-First Discovery (Hybrid 3)
**Focus:** Maximum openness, contribution-focused account prompts, time/engagement-based messaging

**Prototype needs:**
- Search results page (rich cards with full metadata)
- Memory preview page (full content access)
- Progressive prompts (subtle → partnership invitation)
- "Your discoveries" research journal concept

### Direction 2: Progressive Feature Introduction (Hybrid 1)
**Focus:** Demonstrate advanced features progressively, create value through capabilities not content

**Prototype needs:**
- Search results with feature hints ("Save to collections")
- Memory preview with progressive feature reveals
- Feature gating overlays ("Sign in to build timelines")
- Clear differentiation between free content and account features

### Direction 3: Guided Story Discovery (Hybrid 2 - for campaigns, not search)
**Focus:** Curated narrative experiences, emotional engagement, story-driven conversion

**Prototype needs:**
- Campaign landing page (featured stories)
- Narrative-driven memory sequences
- Story completion prompts
- Connection to general search (if applicable)

**Recommendation:** Prototype Direction 1 (Trust-First) and Direction 2 (Progressive Features) for general memory search. Consider Direction 3 separately for Historical Story Campaign flow.

---

---

# Text-Based User Journey Prototypes

Two rough logged-out experience directions for FamilySearch Memories public memory search.

**Design constraints:**
- Public memories stay viewable (content never gated)
- Accounts unlock capabilities, not content
- Prompts feel lightweight and mission-aligned
- Focus on interaction patterns, not UI details

---

## Direction 1: Trust-First Discovery

**Philosophy:** Build trust through radical openness. Let users explore freely. Frame account creation as joining a community of contributors, not unlocking content.

### User Journey: Sarah Discovers Her Grandmother's Story

**Context:** Sarah is curious about her grandmother Emma Rodriguez who lived in Los Angeles in the 1940s. She's not sure if FamilySearch has anything, and she's never created an account.

---

#### Interaction 1: Search Entry
**Time: 0:00 | Memories viewed: 0**

**What Sarah does:**
- Visits FamilySearch.org as logged-out user
- Finds search for memories
- Types "Emma Rodriguez Los Angeles 1940s"
- Hits search

**What Sarah sees:**
- Search results page loads
- 18 results appear
- Rich card layout with prominent images
- Each card shows:
  - Large thumbnail image
  - Person name: "Emma Rodriguez"
  - Dates: "1942" or "1944-1947"
  - Location: "Los Angeles, California"
  - Memory type: "Photo" or "Story"
  - Contributor: "Uploaded by Maria Chen, 2019"
  - Brief snippet: "Emma working at the aircraft factory..."

**What Sarah can do:**
- Scroll through all 18 results
- Click any memory to view
- See everything - no "account required" badges or locked indicators
- Sort/filter results (by date, type, relevance)

**Account prompts:** None (building trust)

**Notes:**
- Feels completely open - no visual indication anything is restricted
- Results provide enough context to make informed choices
- Contributor attribution visible (social proof)

---

#### Interaction 2: First Memory View
**Time: 0:45 | Memories viewed: 1**

**What Sarah does:**
- Clicks first result: Photo of woman in factory setting, labeled "Emma Rodriguez, 1943"

**What Sarah sees:**
- Full memory preview page opens
- High-resolution image (can zoom, pan)
- Complete story/description:
  > "Emma Rodriguez worked at the Douglas Aircraft factory in Long Beach during World War II. She was one of thousands of women who joined the workforce while men served overseas. This photo was taken during her shift in 1943. Emma helped build C-47 transport planes and was proud of her contribution to the war effort."
- Full metadata displayed:
  - Date: March 1943
  - Location: Douglas Aircraft Factory, Long Beach, California
  - Tagged people: Emma Rodriguez, Dorothy Martinez (friend)
  - Memory type: Photograph
  - Uploaded by: Maria Chen (Emma's granddaughter)
  - Upload date: August 2019
  - Collections: "World War II Women Workers"
- Related memories section: "3 more memories of Emma Rodriguez"
- Educational context: Timeline showing "1943: Peak of WWII production"

**What Sarah can do:**
- Read complete story (nothing truncated)
- View full-resolution image
- Click tagged people to see who they are
- Click "3 more memories" to see related content
- Navigate freely

**What Sarah cannot do (but doesn't encounter yet):**
- Save this memory to a collection
- Download the image file
- Add her own story or tag herself

**Account prompts:** None (still building trust through value demonstration)

**Notes:**
- Complete content access - no cliffhangers or truncation
- Educational context adds value beyond just the memory
- Related content visible and accessible
- No friction or interruption yet

---

#### Interaction 3: Exploring Relationships
**Time: 2:15 | Memories viewed: 1**

**What Sarah does:**
- Clicks on tagged person "Dorothy Martinez" to learn more about Emma's friend

**What Sarah sees:**
- Brief profile info for Dorothy Martinez (name, dates: 1920-2008)
- "5 public memories of Dorothy Martinez"
- Thumbnail previews of those 5 memories
- Can click any to view

**What Sarah can do:**
- View Dorothy's profile
- Click to view any of Dorothy's memories (one-hop navigation is free)
- See who Dorothy is in relationship to Emma (friend, coworker)

**Account prompts:** None (one-hop relationship exploration is free)

**Notes:**
- Relationships are explorable, not just visible
- Sarah is learning about Emma's social context
- Deepening engagement through connection discovery

---

#### Interaction 4: Viewing Related Memories
**Time: 5:30 | Memories viewed: 4**

**What Sarah does:**
- Returns to Emma's first memory
- Clicks "3 more memories of Emma"
- Views second memory: Emma's wedding photo, 1946
- Views third memory: Emma with children, 1952
- Views fourth memory: Story about Emma's life, written by granddaughter

**What Sarah sees:**
- Each memory fully accessible (complete stories, full images, all metadata)
- Building a richer picture of Emma's life
- Educational context continues (post-war timeline, Los Angeles history)
- Starting to see narrative arc: wartime work → marriage → family

**What Sarah can do:**
- Continue viewing unlimited memories
- Navigate between related content
- Read complete stories
- Explore tagged people in each memory

**Account prompts:** None yet (trust-building phase continues)

**Sarah's internal state:**
- Increasingly engaged and emotionally connected
- Starting to wonder if this Emma might be her grandmother
- Wanting to explore more systematically

---

#### Interaction 5: First Subtle Indicator
**Time: 7:45 | Memories viewed: 6**

**What Sarah does:**
- Views fifth memory: Emma's naturalization certificate, 1955
- Views sixth memory: Emma at family gathering, 1968
- Starting to feel like she wants to organize what she's finding

**What Sarah sees:**
- All content still fully accessible
- Subtle, non-blocking indicator appears (not a popup, just a persistent subtle element):
  
  **[Indicator - not blocking, dismissible]**
  > "You're building quite a discovery journey! Sign in anytime to save your findings and contribute your family's memories."
  > [Create Free Account] [Dismiss]

**What Sarah can do:**
- Dismiss indicator and continue exploring
- Create account if ready
- Indicator doesn't interrupt viewing - just makes option visible

**Account prompts:** First gentle indicator (not a blocking prompt)

**Example messaging:**
- "You're building quite a discovery journey!"
- "Sign in anytime to save your findings and contribute your family's memories."
- Tone: Encouraging, not pressuring

**Notes:**
- Not blocking or interruptive
- Emphasizes saving and contributing, not unlocking
- Can be dismissed
- Acknowledges user's engagement

---

#### Interaction 6: Continued Exploration with Indicators
**Time: 12:20 | Memories viewed: 10**

**What Sarah does:**
- Continues exploring - now viewed 10 memories across Emma and related people
- Tries to navigate to Dorothy's friend "Robert Chen" (two hops from Emma)

**What Sarah sees:**
- All memory content still accessible
- But when clicking to Robert Chen's memories (two-hop navigation), sees:
  
  **[Lightweight overlay - contextual, dismissible]**
  > "You're exploring deep family connections. Create a free account to navigate extended relationships and build family timelines."
  > [Create Free Account] [Continue Browsing]

**What Sarah can do:**
- Dismiss overlay and return to browsing
- Can still view Robert's profile summary
- Can see that he has memories, but navigating to them requires account
- Can return to one-hop people (Dorothy, Emma) freely

**Account prompts:** Contextual overlay for multi-hop navigation

**Capability gating:**
- Multi-hop relationship navigation (2+ degrees) requires account
- One-hop navigation (Emma → Dorothy) remains free
- Content viewing never gated

**Example messaging:**
- "You're exploring deep family connections."
- "Create a free account to navigate extended relationships and build family timelines."
- Tone: Acknowledging depth of research, offering tools for serious exploration

**Notes:**
- First clear boundary: deep relationship navigation
- Boundary makes sense (casual browsing vs. serious research)
- Doesn't break flow - can dismiss and continue

---

#### Interaction 7: Time-Based Partnership Invitation
**Time: 18:00 | Memories viewed: 12**

**What Sarah does:**
- Has been exploring for 18 minutes
- Viewed 12 memories
- Navigated across multiple people
- Clearly engaged and invested

**What Sarah sees:**
- Content still fully accessible
- More prominent (but still non-blocking) prompt appears:
  
  **[Persistent panel - not blocking view, but more prominent]**
  > **"You've spent 18 minutes discovering Emma's story"**
  > 
  > "FamilySearch is free because people like you contribute and preserve family memories. Every memory you've viewed was shared by someone's family member."
  > 
  > "Create a free account to:"
  > - Save your research and discoveries
  > - Contribute your family's memories
  > - Help others discover their stories
  > 
  > "Join 2 million family historians preserving memories together."
  > 
  > [Create Free Account] [Continue Browsing]

**What Sarah can do:**
- Continue browsing (content never blocked)
- Create account if resonates
- Understand value proposition clearly

**Account prompts:** Mission-driven partnership invitation

**Example messaging:**
- Acknowledges time investment ("You've spent 18 minutes...")
- Emphasizes community and contribution ("people like you contribute")
- Shows social proof ("2 million family historians")
- Lists concrete benefits (save, contribute, help)
- Tone: Invitational, mission-focused, not sales-y

**Notes:**
- Shift from gentle indicator to partnership invitation
- Emphasizes nonprofit mission
- Creates value through contribution framing
- Not about unlocking content (content already visible)

---

#### Interaction 8: Feature Encounter - Download Attempt
**Time: 21:30 | Memories viewed: 14**

**What Sarah does:**
- Finds a particularly meaningful photo of Emma
- Wants to download the high-res version
- Looks for download button, clicks it

**What Sarah sees:**
- Download attempt triggers overlay:
  
  **[Contextual overlay]**
  > **"Download high-resolution images with a free account"**
  > 
  > "You can view all images in full resolution in your browser. Creating a free account lets you download images for safekeeping and personal use."
  > 
  > [Create Free Account] [Continue Viewing]

**What Sarah can do:**
- Create account to download
- Continue viewing in browser (full resolution still visible)
- Understand why download requires account

**Account prompts:** Feature-specific contextual prompt

**Capability gating:**
- Downloads require account
- Viewing full-resolution in browser remains free
- Clear explanation of why (safekeeping, personal use)

**Notes:**
- Natural boundary: viewing vs. possession
- Justification makes sense (not arbitrary)
- Doesn't break experience (can continue viewing)

---

#### Interaction 9: Save/Organization Attempt
**Time: 24:00 | Memories viewed: 16**

**What Sarah does:**
- Has now confirmed this is definitely her grandmother
- Wants to organize the memories she's found
- Looks for "Save" or "Bookmark" feature

**What Sarah sees:**
- "Save to Collection" or "Bookmark" button is visible but has subtle indicator
- Clicking triggers overlay:
  
  **[Contextual overlay]**
  > **"Save and organize discoveries with a free account"**
  > 
  > "You've found 16 memories of Emma and her community. Create a free account to save these discoveries, organize them into collections, and continue your research."
  > 
  > "When you sign in, we'll save everything you've explored today so you can pick up right where you left off."
  > 
  > [Create Free Account] [Continue Browsing]

**What Sarah can do:**
- Create account to save/organize
- Continue viewing (but can't save for later)
- Knows her exploration will be preserved if she signs up

**Account prompts:** Organization-focused prompt with "research journal" promise

**Capability gating:**
- Saving/bookmarking requires account
- Organization features require account
- Promise: exploration history preserved upon signup

**Notes:**
- Natural conversion moment (user wants to organize)
- "Research journal" concept introduced
- Respects effort invested (preserve exploration)

---

#### Interaction 10: Conversion or Continued Browsing
**Time: 25:00+ | Memories viewed: 16+**

**Sarah's decision point:**

**If Sarah creates account:**
- Sign-up flow initiates (simple, fast)
- Upon completion, Sarah sees:
  - "Your discoveries" collection with all 16 memories she viewed
  - Exploration timeline showing her research path
  - Prompt to contribute: "Add your own memories of Emma"
  - Immediate access to all features (save, download, organize, contribute)

**If Sarah continues browsing:**
- Can continue viewing unlimited public memory content
- Encounters capability boundaries (downloads, deep navigation, saving)
- Prompts become more frequent but never block content viewing
- Can return later - if cookies preserved, exploration can be resumed

---

### Key Interaction Moments Summary (Direction 1)

| Time | Memories | Interaction | Prompt Type | Prompt Message | Capability Boundary |
|------|----------|-------------|-------------|----------------|---------------------|
| 0:00 | 0 | Search results | None | - | None |
| 0:45 | 1 | First memory view | None | - | None |
| 2:15 | 1 | One-hop navigation (tagged person) | None | - | None (free) |
| 5:30 | 4 | Related memories | None | - | None |
| 7:45 | 6 | Continued viewing | Gentle indicator | "You're building quite a discovery journey!" | None |
| 12:20 | 10 | Multi-hop navigation attempt | Contextual overlay | "You're exploring deep family connections." | 2+ hop navigation gated |
| 18:00 | 12 | Time-based milestone | Partnership invitation | "You've spent 18 minutes discovering Emma's story..." | None (content still free) |
| 21:30 | 14 | Download attempt | Feature overlay | "Download high-resolution images with a free account" | Downloads gated |
| 24:00 | 16 | Save attempt | Organization overlay | "Save and organize discoveries with a free account" | Saving/organizing gated |

**Conversion triggers:**
- Desire to organize/save discoveries
- Desire to download images
- Desire to navigate deep relationships
- Mission-driven invitation resonates
- Time investment makes account worthwhile

**User experience qualities:**
- Trustworthy (never feels restricted)
- Generous (content always accessible)
- Mission-aligned (contribution > consumption)
- Respectful (non-interruptive prompts)
- Progressive (gentle → partnership invitation)

---

## Direction 2: Progressive Feature Introduction

**Philosophy:** Demonstrate the value of advanced capabilities progressively. Surface features gradually to create awareness and desire. Account value comes from powerful tools, not content access.

### User Journey: Michael Researches His Great-Grandfather

**Context:** Michael is a genealogy hobbyist researching his great-grandfather Thomas O'Brien who immigrated from Ireland in 1905. He's systematic and organized in his research approach.

---

#### Interaction 1: Search Entry
**Time: 0:00 | Memories viewed: 0**

**What Michael does:**
- Visits FamilySearch Memories search
- Types "Thomas O'Brien Ireland immigration 1905"
- Executes search

**What Michael sees:**
- Search results page with 24 results
- Card-based layout with prominent images and metadata
- Each card shows:
  - Thumbnail image
  - Name: "Thomas O'Brien"
  - Dates: "1905" or "1880-1950"
  - Location: "New York, NY" or "County Cork, Ireland"
  - Memory type
  - Contributor
- Subtle feature hints visible in UI:
  - Small "Save" icon on each card (grayed out with tooltip: "Sign in to save")
  - "Collections" badge visible on some memories: "Part of 'Irish Immigration 1900-1910'"

**What Michael can do:**
- Click any memory to view
- See all results
- Notice feature hints but not blocked from viewing

**Account prompts:** None yet, but features are subtly visible

**Notes:**
- Features are previewed visually (save buttons, collection badges)
- Not blocking, just creating awareness
- Michael notices organization capabilities exist

---

#### Interaction 2: First Memory View with Feature Introduction
**Time: 1:00 | Memories viewed: 1**

**What Michael does:**
- Clicks first result: Ship manifest showing Thomas O'Brien as passenger, 1905

**What Michael sees:**
- Full memory preview page
- High-resolution image of ship manifest (fully viewable, zoomable)
- Complete transcription/description
- Full metadata
- **New element - Feature introduction sidebar (non-blocking, informational):**
  
  **[Feature hint panel - subtle, not blocking content]**
  > **Research Tools Available:**
  > - 📚 Save to Collections (Sign in)
  > - 📊 Build Timeline (Sign in)
  > - 🔗 Connect to Family Tree (Sign in)
  > - ⬇️ Download High-Res (Sign in)
  > 
  > [Learn More]

**What Michael can do:**
- View complete memory content (nothing gated)
- See what's possible with an account
- Click "Learn More" to understand features
- Ignore sidebar and continue browsing

**Account prompts:** Feature awareness (not a conversion ask yet)

**Notes:**
- Early introduction of what's possible
- Creates desire through awareness
- Not pushy - informational
- Content remains fully accessible

---

#### Interaction 3: Feature Demo - Timeline Preview
**Time: 3:30 | Memories viewed: 3**

**What Michael does:**
- Views three memories: ship manifest (1905), naturalization papers (1912), family photo (1920)
- Notices timeline visualization could connect these

**What Michael sees:**
- After viewing 3 memories with clear chronological progression, subtle prompt appears:
  
  **[Feature demo - lightweight, visual]**
  > **"These memories span 1905-1920"**
  > 
  > [Visual preview: Simple timeline showing 3 dots at 1905, 1912, 1920]
  > 
  > "Sign in to build complete timelines, map relationships, and organize your research."
  > 
  > [See Demo] [Create Account] [Dismiss]

**What Michael can do:**
- Click "See Demo" to see what timeline feature looks like
- Create account if interested
- Dismiss and continue browsing
- All memory content still accessible

**Account prompts:** Feature demonstration (showing value, not blocking)

**Capability introduction:**
- Timeline building introduced as valuable research tool
- Not blocking content, demonstrating capability
- Concrete visual preview (not abstract promise)

**Notes:**
- Contextual (appeared after chronological memories)
- Visual demonstration of feature value
- Creates desire through concrete example

---

#### Interaction 4: Exploring Relationships with Progressive Awareness
**Time: 6:00 | Memories viewed: 5**

**What Michael does:**
- Clicks tagged person on memory: "Margaret O'Brien (wife)"
- Navigates to Margaret's memories

**What Michael sees:**
- Can navigate to Margaret freely (one-hop)
- Views her profile and memories
- Notices Margaret has children tagged
- Clicks child "Patrick O'Brien" (two hops from Thomas)
- Sees:
  
  **[Feature boundary overlay - contextual]**
  > **"You're exploring extended family connections"**
  > 
  > [Visual diagram showing: Thomas → Margaret → Patrick with arrow progression]
  > 
  > "You can view direct relationships freely. Create a free account to:"
  > - Navigate extended family networks
  > - Build relationship maps
  > - Discover connection pathways
  > 
  > "Your current exploration: Thomas O'Brien → Margaret O'Brien → Patrick O'Brien"
  > 
  > [Create Account] [Return to Browsing]

**What Michael can do:**
- See that extended navigation is a feature
- Understand the boundary clearly (1-hop free, 2+ needs account)
- Return to Thomas or Margaret freely
- View Patrick's profile summary but not navigate to his memories

**Account prompts:** Feature boundary with explanation and value prop

**Capability gating:**
- Multi-hop navigation gated
- Boundary explained visually and clearly
- Feature value articulated (relationship maps, connection pathways)

**Notes:**
- Boundary is clear and justified
- Visual diagram helps understanding
- Frames as research capability, not arbitrary limit

---

#### Interaction 5: Download Feature Introduction
**Time: 9:00 | Memories viewed: 8**

**What Michael does:**
- Finds important document: Thomas's naturalization certificate
- Wants to save a copy for his records
- Looks for download option

**What Michael sees:**
- Download button visible with "Account required" indicator
- Clicking shows:
  
  **[Feature explanation overlay]**
  > **"Download original documents with a free account"**
  > 
  > "You're viewing full-resolution in your browser. Creating an account lets you:"
  > - Download high-resolution originals
  > - Export collections for offline research
  > - Print documents and images
  > 
  > "All downloads preserve original quality and metadata."
  > 
  > [Create Account] [Continue Viewing]

**What Michael can do:**
- Understand download feature clearly
- Continue viewing in browser (full resolution)
- Take screenshot if needed (not blocked from that)
- Create account when ready

**Account prompts:** Feature-specific value explanation

**Capability gating:**
- Downloads require account
- Viewing remains free
- Clear explanation of what download feature provides

**Notes:**
- Natural research boundary (viewing vs. possessing)
- Feature value clearly articulated
- Not blocking current activity (viewing)

---

#### Interaction 6: Organization Feature Demo - Collections
**Time: 12:00 | Memories viewed: 11**

**What Michael does:**
- Has viewed 11 memories across Thomas, Margaret, and related people
- Starting to lose track of what he's seen
- Wishes he could organize findings

**What Michael sees:**
- Prominent feature introduction appears:
  
  **[Feature showcase - more prominent than earlier hints]**
  > **"You're building a research collection"**
  > 
  > "You've viewed 11 memories across 3 people spanning 1905-1930."
  > 
  > [Preview image: mockup of collection view with memories organized]
  > 
  > "With a free account you can:"
  > - Save memories to collections
  > - Organize by person, date, or theme
  > - Add research notes and tags
  > - Share collections with family
  > 
  > "We'll save everything you've explored today as your first collection."
  > 
  > [Create Account] [Continue Browsing]

**What Michael can do:**
- See concrete visual of what collections look like
- Understand organization value
- Know his current exploration will be preserved
- Continue browsing without account

**Account prompts:** Progressive feature showcase (more prominent, concrete value)

**Capability introduction:**
- Collections introduced with visual mockup
- "Research journal" promise (exploration preserved)
- Multiple organization benefits listed
- Social feature mentioned (share with family)

**Notes:**
- More prominent than earlier hints (progression)
- Concrete visual mockup shows feature
- Directly addresses pain point (losing track)
- Creates desire through demonstrated need

---

#### Interaction 7: Research Tools Feature Introduction
**Time: 15:00 | Memories viewed: 15**

**What Michael does:**
- Viewed 15 memories, navigating complex family relationships
- Trying to understand how everyone connects
- Manually keeping track of relationships

**What Michael sees:**
- Feature introduction for advanced research tools:
  
  **[Research tools showcase]**
  > **"Unlock powerful research tools"**
  > 
  > "You're exploring complex family connections. Free research tools help you:"
  > 
  > **Timeline Builder**
  > "Visualize 15 memories across 25 years. Spot gaps and patterns in family history."
  > [Visual preview: timeline mockup]
  > 
  > **Relationship Mapper**
  > "Explore how Thomas, Margaret, and 8 others connect. Navigate family networks visually."
  > [Visual preview: relationship diagram]
  > 
  > **Cross-Collection Search**
  > "Search across millions of memories to find more O'Brien family connections."
  > 
  > [Create Free Account] [Dismiss]

**What Michael can do:**
- See concrete examples of research tools
- Understand how they'd solve current challenges
- Create account to access tools
- Continue manual browsing

**Account prompts:** Advanced feature showcase with visuals

**Capability introduction:**
- Multiple research tools introduced
- Each with visual mockup
- Clear value proposition for each
- Addresses current pain points (tracking complexity)

**Notes:**
- Appeals to researcher mindset
- Concrete tool demonstrations
- Creates desire for capabilities
- Progression: started with hints, now showcasing tools

---

#### Interaction 8: Save Attempt - Conversion Moment
**Time: 18:00 | Memories viewed: 18**

**What Michael does:**
- Finds particularly valuable memory: Thomas's diary entry
- Wants to save it for later detailed analysis
- Clicks "Save" button

**What Michael sees:**
- Save action triggers account requirement:
  
  **[Conversion prompt - clear value]**
  > **"Save and organize your research"**
  > 
  > "You've discovered 18 memories of Thomas O'Brien and family. Create a free account to:"
  > 
  > ✓ Save these 18 memories to your collection
  > ✓ Organize and tag your discoveries
  > ✓ Build timelines and relationship maps
  > ✓ Download documents and images
  > ✓ Continue research across devices
  > ✓ Contribute your own family memories
  > 
  > "Everything you've explored today will be saved when you sign in."
  > 
  > [Create Free Account]

**What Michael can do:**
- Create account to save (natural conversion moment)
- Understand full value proposition
- See cumulative benefits of features introduced
- Know exploration will be preserved

**Account prompts:** Conversion prompt at natural save moment

**Capability summary:**
- All introduced features summarized
- Clear checklist of capabilities
- "Research journal" promise reinforced
- Action-based (user initiated)

**Notes:**
- Natural conversion moment (user wants to save)
- Consolidates all feature value communicated
- Progressive journey pays off (has seen features)
- Action-initiated, not time-based

---

#### Interaction 9: Conversion or Continued Progressive Exploration
**Time: 18:00+ | Memories viewed: 18+**

**Michael's decision point:**

**If Michael creates account:**
- Fast signup flow
- Upon completion:
  - "Your Research Collection" created with 18 memories
  - All introduced features immediately available
  - Tutorial: "Build your first timeline" or "Map Thomas's family connections"
  - Prompt to contribute: "Add documents or memories of Thomas"

**If Michael continues browsing:**
- Can continue viewing unlimited content
- Feature hints become more prominent progressively
- Encounters capability boundaries more frequently
- Each boundary reinforces feature value
- Can convert at any save/organize/download attempt

---

### Key Interaction Moments Summary (Direction 2)

| Time | Memories | Interaction | Feature Introduced | Prompt Type | Capability Boundary |
|------|----------|-------------|-------------------|-------------|---------------------|
| 0:00 | 0 | Search results | Save icons (subtle hints) | None | None |
| 1:00 | 1 | First memory view | Research tools sidebar | Awareness | None |
| 3:30 | 3 | Chronological memories | Timeline builder demo | Feature demo | None |
| 6:00 | 5 | Multi-hop navigation | Relationship mapping | Feature boundary | 2+ hop navigation |
| 9:00 | 8 | Download attempt | Download feature | Feature explanation | Downloads gated |
| 12:00 | 11 | Browsing complexity | Collections showcase | Feature showcase | Organization gated |
| 15:00 | 15 | Complex relationships | Research tools suite | Advanced feature showcase | Advanced tools gated |
| 18:00 | 18 | Save attempt | Full value summary | Conversion prompt | Saving gated |

**Feature Introduction Progression:**
1. **Subtle hints** (search results, first view)
2. **Feature awareness** (sidebar, tooltips)
3. **Concrete demos** (timeline preview, visual mockups)
4. **Feature boundaries** (contextual overlays with value)
5. **Feature showcases** (prominent, multi-capability presentations)
6. **Conversion prompt** (comprehensive value summary)

**Conversion triggers:**
- Desire to organize research (collections)
- Desire to use research tools (timeline, relationships)
- Desire to save findings (bookmarking)
- Desire to download documents
- Accumulated awareness of feature value

**User experience qualities:**
- Educational (learns what's possible)
- Progressive (gentle → prominent feature introduction)
- Value-focused (concrete tool demonstrations)
- Capability-driven (account = research tools)
- Research-oriented (appeals to systematic researchers)

---

## Direction Comparison: Trust-First vs Progressive Features

### Key Differences

| Aspect | Direction 1: Trust-First | Direction 2: Progressive Features |
|--------|-------------------------|----------------------------------|
| **Initial Experience** | Completely silent, no hints | Subtle feature hints visible early |
| **Feature Communication** | Minimal until boundaries encountered | Progressive demonstrations throughout |
| **Prompt Timing** | Time/depth-based (6+ memories, 18+ min) | Action/feature-based (save, download attempts) |
| **Messaging Focus** | Mission, community, contribution | Capabilities, research tools, organization |
| **Visual Approach** | Clean, minimal, content-focused | Feature hints, tooltips, mockups visible |
| **Account Value Prop** | "Join the community and contribute" | "Unlock powerful research tools" |
| **Conversion Trigger** | Mission alignment + time investment | Desire for specific capabilities |
| **Best For** | Casual explorers, emotionally-driven | Systematic researchers, tool-oriented |

### Similarities (Both Directions)

✓ **Content never gated:** Public memories always viewable  
✓ **Capability boundaries:** Saving, downloading, deep navigation requires account  
✓ **Non-blocking:** Prompts dismissible, don't interrupt viewing  
✓ **Progressive:** Starts gentle, becomes more prominent  
✓ **Research journal:** Promise to preserve exploration upon signup  
✓ **One-hop navigation:** Free relationship exploration (direct connections)  
✓ **Multi-hop gating:** Extended relationships require account  

### User Personas

**Direction 1 works best for:**
- First-time family history explorers
- Emotionally-driven discovery
- Users who value mission/community
- Casual browsers who might convert
- Users skeptical of "freemium" models

**Direction 2 works best for:**
- Active genealogy researchers
- Systematic, organized researchers
- Tool-oriented users
- Users who want to understand capabilities upfront
- Power users who appreciate feature depth

---

## Example Account Prompts by Type

### Trust-First Prompts (Direction 1)

**Gentle Indicator (6+ memories):**
> "You're building quite a discovery journey! Sign in anytime to save your findings and contribute your family's memories."

**Partnership Invitation (18+ minutes):**
> "You've spent 18 minutes discovering Emma's story. FamilySearch is free because people like you contribute and preserve family memories. Join 2 million family historians preserving memories together."

**Feature Boundary (Multi-hop navigation):**
> "You're exploring deep family connections. Create a free account to navigate extended relationships and build family timelines."

**Download Attempt:**
> "Download high-resolution images with a free account. You can view all images in full resolution in your browser. Creating an account lets you download images for safekeeping and personal use."

**Save Attempt:**
> "Save and organize discoveries with a free account. You've found 16 memories of Emma and her community. When you sign in, we'll save everything you've explored today."

---

### Progressive Feature Prompts (Direction 2)

**Feature Awareness (First view):**
> "Research Tools Available: Save to Collections, Build Timeline, Connect to Family Tree, Download High-Res. [Learn More]"

**Timeline Demo (3 chronological memories):**
> "These memories span 1905-1920. Sign in to build complete timelines, map relationships, and organize your research. [See Demo]"

**Relationship Boundary (Multi-hop):**
> "You're exploring extended family connections. You can view direct relationships freely. Create a free account to navigate extended family networks and build relationship maps."

**Collections Showcase (11+ memories):**
> "You're building a research collection. You've viewed 11 memories across 3 people spanning 1905-1930. With a free account you can save, organize, add notes, and share collections with family."

**Research Tools (15+ memories):**
> "Unlock powerful research tools. Timeline Builder: Visualize 15 memories across 25 years. Relationship Mapper: Explore how Thomas, Margaret, and 8 others connect. Cross-Collection Search: Find more O'Brien family connections."

**Conversion (Save attempt):**
> "You've discovered 18 memories of Thomas O'Brien. Create a free account to save, organize, build timelines, download documents, continue research across devices, and contribute your own memories."

---

## Exploration Continuity Patterns

Both directions maintain exploration continuity through:

### Free Navigation Patterns:
- Search results → Memory view (unlimited)
- Memory → Related memories (unlimited viewing)
- Memory → Tagged person (one hop, can view profile and memories)
- Memory → Educational context (always free)
- Memory → Geographic/temporal context (always free)

### Gated Navigation Patterns:
- Tagged person → Their connections (2+ hops requires account)
- Memory → Download file (requires account)
- Memory → Save/bookmark (requires account)
- Memory → Advanced research tools (requires account)
- Cross-collection advanced search (requires account)

### Resumption After Account Creation:
- All explored memories saved to "Your Discoveries" collection
- Exploration timeline/map visualized
- Can pick up exactly where left off
- All gated features immediately accessible
- Suggested next actions based on research pattern

---

## Open Design Questions

1. **Prompt Frequency:**
   - Direction 1: How long between gentle indicator and partnership invitation?
   - Direction 2: How many feature demos before feeling overwhelming?
   - Both: What happens if user dismisses repeatedly?

2. **Feature Boundaries:**
   - Is "one-hop free, two-hop gated" the right relationship boundary?
   - Should we allow one free download as a taste?
   - Do different memory types (photos vs documents) need different rules?

3. **Visual Treatment:**
   - Direction 1: How subtle should indicators be?
   - Direction 2: How prominent should feature hints be without cluttering?
   - Both: What visual language communicates "account required" without feeling locked?

4. **Messaging Tone:**
   - Direction 1: Does mission-driven messaging resonate or feel preachy?
   - Direction 2: Does feature-focus feel too "sales-y" or appropriately educational?
   - Both: How do we balance encouragement with respect for browsing?

5. **Success Metrics:**
   - What conversion rate is success for each direction?
   - How do we measure quality of conversions (contributors vs passive users)?
   - What engagement depth indicates likelihood to convert?

6. **Technical Implementation:**
   - How do we track exploration across sessions (cookies, anonymous IDs)?
   - How do we generate "research journals" automatically?
   - What's involved in relationship hop counting?

---

## Next Steps for Validation

1. **User Testing:**
   - Test both directions with different user personas
   - Measure conversion rates and user sentiment
   - Identify which prompts resonate vs feel pushy

2. **Message Testing:**
   - A/B test mission-driven vs feature-driven messaging
   - Test different prompt timing (time-based vs action-based)
   - Validate tone (encouraging vs educational vs neutral)

3. **Boundary Refinement:**
   - Test one-hop vs two-hop navigation boundaries
   - Validate download gating vs allowing taste
   - Explore memory type differentiation

4. **Feature Prioritization:**
   - Which advanced features create most conversion desire?
   - What's the minimum viable feature set for account value?
   - Which research tools matter most to target users?

5. **Mission Alignment Validation:**
   - Does Direction 1 feel authentic to FamilySearch's mission?
   - Does Direction 2 sacrifice mission for conversion?
   - Can we measure "long-term contributor" conversion vs just accounts?

