# JIF Cookbook - Handover for Next Session (Static Site Build)

**Date:** July 22, 2026  
**Status:** Docsify approach abandoned. Reverting to working version. Ready for static site rebuild.

---

## CURRENT STATE

**Live Site:** https://anyashina.github.io/jif-cookbook/#/

**What's Working:**
- JIF SVG logo displaying in sidebar (sand/gold geometric typeface)
- Firebird feather at bottom with "Prepared by ANyashina LLC"
- All 5 cookbook sections complete and accessible
- All supporting materials linked
- Professional styling (Cormorant Garamond, DM Sans, JIF brand colors)
- Sidebar visible, home page accessible
- All links working (no 404s)

**What's NOT Working:**
- Docsify's native sidebar TOC not rendering properly
- No visible navigation menu on left side to click through sections
- Users must use main content links to navigate (works, but not ideal)
- Docsify injection scripts conflict with sidebar rendering

**Current Tech Stack:**
- GitHub Pages + Docsify static site generator
- Local repo at `/home/claude/jif-cookbook/`
- Remote: `https://github.com/anyashina/jif-cookbook.git`

---

## WHAT NEEDS TO HAPPEN (NEXT SESSION)

**Build a proper static site using Hugo or Jekyll instead of Docsify.**

### Why Static Site is Better:
1. Full control over layout and navigation
2. No framework limitations on sidebar TOC
3. Can implement custom left sidebar with full TOC
4. Cleaner, faster, more maintainable
5. Better for tablet/mobile navigation

### Goals for Static Rebuild:
1. **Left sidebar with full TOC**
   - JIF logo (right-aligned, SVG)
   - Organized navigation sections:
     - THE COOKBOOK (5 sections)
     - FOR REPLICATORS (4 guides)
     - OPERATIONS (2 financial docs)
     - SUPPORTING MATERIALS (4 docs)
   - Feather + "Prepared by ANyashina LLC" at bottom

2. **Main content area**
   - Home page overview
   - All 5 sections accessible and readable
   - Links between sections working
   - Search functionality (if possible)

3. **Mobile/Tablet responsive**
   - Sidebar collapses on small screens
   - Full navigation accessible on Chromebook and Android devices
   - Touch-friendly interface

4. **Brand compliance**
   - JIF geometric typeface (SVG logo at top)
   - Cormorant Garamond for headings
   - DM Sans for body
   - Brand colors: Teal #3A8A88, Navy #2C4B6E, Sand #C8BBAA, Warm White #F7F4F0
   - No em dashes
   - Footer: ANyashina LLC info only (no client contact details)

---

## COMPLETE CONTENT INVENTORY

All files ready in `/home/claude/jif-cookbook/docs/`:

### Cookbook Sections (5 complete)
1. `01-timeline.md` - Program evolution 2006-2023
2. `02-kitchen-notes.md` - Stakeholder voices (Fellows, hosts, staff)
3. `03-recipes.md` - Operational how-to + expanded budget framework
4. `03-recipes-EXPANDED-Jul22.md` - Detailed budget breakdown
5. `04-network.md` - 35+ people mapped by role
6. `05-vision.md` - Elise's reflection + Methodology of Serendipity

### Financial Docs
- `playbook.md` - Financial operations architecture
- `budget-framework-detailed.md` - Cost models for Kyiv, Krakow, Chicago
- `materials-inventory.md` - Source material reference

### Supporting Materials
- `2022-evaluation.md` - Independent assessment
- `strategic-plan-2014-2018.md` - Historical context
- `mailchimp-voice.md` - Communication patterns
- `press-archive.md` - Media coverage

### Replicator Guides
- `selection-process.md`
- `host-org-vetting.md`
- `staffing.md`
- `budgets.md`
- `methodology.md`

### Assets
- `jif-logo.svg` - Geometric/architectural typeface (sand/gold)
- `feather.png` - Firebird feather (teal with amber glow)

### Home Page
- `home.md` - Landing page with two user paths (Next Director / Replicators)

---

## WHAT TO KEEP / WHAT TO REBUILD

### KEEP (No changes needed):
- All markdown content files (.md) - they're perfect
- SVG logo and feather graphics
- Brand colors and typography specs
- All 21+ complete documents and guides

### REBUILD (New static site):
- index.html → Hugo/Jekyll theme or custom HTML
- Docsify config → Hugo config.toml or Jekyll _config.yml
- Sidebar injection JavaScript → Native template navigation
- Overall page structure and layout

---

## GITHUB SETUP

**Current Status:**
- Repo: `anyashina/jif-cookbook`
- Branch: `main`
- Pages enabled: Yes (publishing from `main` branch)
- Last commit: `5f92a6c` (Docsify config - working version, reverted)

**For Next Session:**
- Option A: Continue using GitHub Pages + new static generator
- Option B: Use different hosting if needed (but GitHub Pages is simpler)

---

## FILES & LOCATIONS

**Local Development:**
- `/home/claude/jif-cookbook/` - Full repo with all content
- `/mnt/user-data/outputs/` - All backups and reference files

**GitHub:**
- Source: `https://github.com/anyashina/jif-cookbook`
- Live: `https://anyashina.github.io/jif-cookbook/#/`

**Token Budget:**
- Used: ~145,000 / 190,000
- Remaining: ~45,000
- Enough for: Planning, architecture, initial build setup
- May need new token allocation for full implementation

---

## KEY DECISIONS MADE (DON'T REPEAT)

1. ✅ **JIF custom geometric typeface as SVG** - This is CORRECT. Keep it.
2. ✅ **Markdown-based content** - This works perfectly. Keep it.
3. ❌ **Docsify with Sidebar Injection** - DON'T use this. Framework limitations made sidebar impossible to customize.
4. ✅ **GitHub Pages hosting** - Works well, keep this.
5. ✅ **Brand colors and typography** - Locked in, looking professional.

---

## RECOMMENDED NEXT STEPS

**Session Start:**
1. Review this handover
2. Decide: Hugo vs Jekyll vs custom HTML build
3. Set up development environment
4. Create new static site structure
5. Migrate content (copy .md files to new structure)
6. Build custom left sidebar + TOC
7. Test responsive design
8. Deploy to GitHub Pages

**Time Estimate:**
- Planning & setup: 30 min
- Build template/theme: 45 min
- Migrate content: 15 min
- Testing & refinement: 30 min
- Total: ~2 hours

---

## CONTACT & REFERENCE

**Prepared by:** Alexandra Nyashina, ANyashina LLC  
**For:** Elise Bernhardt, Jerusalem International Fellows  
**Date:** July 22, 2026  

**Resources:**
- Hugo quickstart: https://gohugo.io/getting-started/quick-start/
- Jekyll quickstart: https://jekyllrb.com/docs/
- GitHub Pages docs: https://docs.github.com/en/pages

---

## FINAL NOTE

The Cookbook content is **excellent and complete.** All 5 sections, all supporting materials, all budget frameworks - ready to go. The only issue is the *presentation layer* (navigation + layout). 

Switching to a static site generator will solve this in one session. The content doesn't need to change at all.

**You're ready to cook. Just need a better kitchen layout.**

