# Installed OpenCode Skills

**Installation Date:** March 3, 2026  
**Source:** [Claude Code Templates](https://www.aitmpl.com/skills)  
**Installed by:** AI Assistant  

---

## 🎨 Creative Skills

### 1. **algorithmic-art**
Create generative art using p5.js with seeded randomness and interactive parameter exploration.

**Use when:** Creating art with code, generative art, algorithmic art, flow fields, or particle systems.

**Features:**
- Algorithmic philosophy creation
- p5.js generative algorithms
- Seeded randomness and noise fields
- Interactive parameter exploration
- Multiple aesthetic movements (Organic Turbulence, Quantum Harmonics, etc.)

**Example:** "Create generative art representing quantum entanglement"

---

### 2. **game-development** (Orchestrator)
Master skill that routes to platform-specific game development sub-skills.

**Use when:** Starting any game development project.

**Routes to:**
- `web-games` - HTML5, WebGL games
- `mobile-games` - iOS, Android games
- `pc-games` - Steam, Desktop games
- `vr-ar` - VR/AR headset games
- `2d-games` - Sprite-based games
- `3d-games` - 3D mesh games
- `multiplayer` - Networking
- `game-design` - GDD, balancing, psychology
- `game-art` - Visual style, animation
- `game-audio` - Sound design, music

**Example:** "Create a 2D platformer game for the web"

---

### 3. **game-design**
Game design principles including GDD structure, balancing, player psychology, and progression systems.

**Use when:** Designing game mechanics, writing game design documents, or balancing gameplay.

**Features:**
- Core loop design (30-second test)
- Game Design Document (GDD) templates
- Player psychology principles
- Progression system design
- Balance and tuning guidance

**Example:** "Design a progression system for an RPG"

---

### 4. **remotion-best-practices**
Best practices for Remotion - creating videos programmatically with React.

**Use when:** Creating videos, animations, or motion graphics with React/Remotion.

**Features:**
- 3D content with Three.js
- Animation fundamentals
- Asset management (images, videos, audio, fonts)
- Audio synchronization
- Chart and data visualization
- Caption display
- GIF support
- Lottie animations
- Tailwind integration
- Text animations

**Example:** "Create an animated video infographic with Remotion"

---

### 5. **marp-slide**
Create professional Marp presentation slides with 7 beautiful themes.

**Use when:** Creating presentations, slide decks, or Marp documents.

**Themes:**
- `default` - Clean, professional
- `minimal` - Simple, academic
- `colorful` - Creative, events
- `dark` - Dark background
- `gradient` - Modern gradients
- `tech` - Technology-focused
- `business` - Corporate style

**Features:**
- Custom theme support
- Image layouts and patterns
- Math equations (LaTeX)
- Emoji support
- Auto-formatting

**Example:** "Create a tech presentation about AI agents"

---

## 🔬 Scientific Skills

### 6. **literature-review**
Conduct comprehensive, systematic literature reviews using multiple academic databases.

**Use when:** Conducting systematic reviews, meta-analyses, or research synthesis.

**Features:**
- Multi-database search (PubMed, arXiv, bioRxiv, Semantic Scholar)
- Thematic synthesis
- Citation verification
- Multiple citation styles (APA, Nature, Vancouver)
- Professional markdown and PDF output
- AI-generated figures with scientific-schematics

**Example:** "Conduct a literature review on transformer architectures"

---

### 7. **hypothesis-generation**
Generate testable hypotheses from observations and design experiments.

**Use when:** Formulating research hypotheses, designing experiments, or exploring competing theories.

**Features:**
- Observation-based hypothesis generation
- Experimental design
- Competing hypothesis exploration
- Mechanistic pathway diagrams
- Experimental design flowcharts
- Prediction decision trees
- AI-generated schematics

**Example:** "Generate hypotheses about why model performance degrades over time"

---

## How to Use

### Method 1: Direct Invocation
Simply ask to use the skill:

```
"Use the algorithmic-art skill to create a generative piece about entropy"
"Use the game-design skill to help me design a card game"
"Use the literature-review skill to research RAG systems"
```

### Method 2: Natural Request
The skills will activate automatically when you request work in their domain:

```
"Create a presentation about machine learning"
→ Uses marp-slide skill

"Design a game about space exploration"
→ Uses game-development skill

"Generate some algorithmic art"
→ Uses algorithmic-art skill
```

---

## Skill Locations

All skills are installed in: `~/.config/opencode/skills/`

Each skill contains:
- `SKILL.md` - Main skill instructions
- `references/` - Detailed guides and examples
- `rules/` - Specific rules and patterns (where applicable)

---

## Example Workflows

### Create Generative Art
```
1. "Use algorithmic-art to create a piece about 'Digital Erosion'"
2. Skill generates philosophy and aesthetic movement
3. Skill creates p5.js code (HTML + JS)
4. You get an interactive, generative artwork
```

### Design a Game
```
1. "Use game-design to create a GDD for a puzzle game"
2. Skill guides through core loop, mechanics, progression
3. Skill helps balance and refine systems
4. You get a complete Game Design Document
```

### Create a Video
```
1. "Use remotion-best-practices to create an animated chart video"
2. Skill provides Remotion + React patterns
3. Skill guides animation timing and composition
4. You get production-ready video code
```

### Conduct Research
```
1. "Use literature-review to research multi-agent systems"
2. Skill searches multiple academic databases
3. Skill synthesizes findings thematically
4. You get a formatted literature review with citations
```

---

## Notes

- All skills are designed for **OpenCode** (not Claude Code)
- Skills integrate with your existing tools (Read, Write, Edit, Bash)
- Skills can be combined (e.g., game-design + algorithmic-art for procedural games)
- Each skill includes comprehensive documentation and examples

---

## Updating Skills

To update skills in the future:

```bash
cd /tmp
git clone --depth 1 https://github.com/davila7/claude-code-templates.git
cd claude-code-templates/cli-tool/components/skills
# Copy desired skills to ~/.config/opencode/skills/
```

---

**Enjoy creating with your new skills!** 🚀
