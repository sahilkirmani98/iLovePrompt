import { useState, useCallback, useEffect } from "react";

// ─── PROMPT DATA ─────────────────────────────────────────────────────────────
const STYLES = [
  {
    id: "cyberpunk",
    title: "Cyberpunk Neon",
    category: "Cinematic",
    tagline: "Rain-slicked streets. Electric soul.",
    color: "#00f5ff",
    glow: "rgba(0,245,255,0.4)",
    bg: "linear-gradient(135deg,#000d1a 0%,#001a2e 100%)",
    image: "https://images.unsplash.com/photo-1542327897-d73f4005b533?w=600&q=80",
    prompt: `[MULTI-MODAL PORTRAIT TRANSFORMATION — CYBERPUNK NEON]

IDENTITY PRESERVATION DIRECTIVE:
The subject's facial geometry, bone structure, eye shape, nose profile, lip form, and all unique identifying features must remain 100% faithful to the uploaded reference photo. Do not alter, beautify, or normalize any facial features. Treat the face as a locked layer.

SCENE CONSTRUCTION:
Re-render the entire image into a hyper-stylized Neo-Tokyo cyberpunk environment. The subject stands in a narrow rain-soaked alley at 02:00 AM. Surfaces are reflective black asphalt and wet concrete. Neon signage in Japanese kanji and English (HOTEL / BAR / OPEN 24H) bleeds pink, cyan, and electric violet light across all surfaces.

LIGHTING SCHEMA:
Primary: a large cyan neon tube off-frame left casting a cool rim light that wraps the jawline. Secondary fill: warm magenta neon from below-right creating split-color skin illumination — half cyan, half magenta. Add volumetric rain particles catching the neon.

MATERIAL & TEXTURE:
High-collar black leather jacket with holographic trim. Skin: ultra-sharp photorealistic pores. Hair: wet, individually rendered strands catching neon glints. Background: deep-focus city layers receding into purple haze.

COMPOSITION: 3:4 portrait. Eyes at upper third line. Subject fills 60% of frame.

OUTPUT MOOD: Blade Runner 2049 × Ghost in the Shell. Cinematic, lonely, electric.`,
  },
  {
    id: "claymation",
    title: "3D Claymation",
    category: "Fantasy",
    tagline: "Handcrafted warmth. Infinite charm.",
    color: "#ff9500",
    glow: "rgba(255,149,0,0.4)",
    bg: "linear-gradient(135deg,#1a0a00 0%,#2e1500 100%)",
    image: "https://images.unsplash.com/photo-1531746020798-e6953c6e8e04?w=600&q=80",
    prompt: `[MULTI-MODAL PORTRAIT TRANSFORMATION — 3D CLAYMATION]

IDENTITY PRESERVATION DIRECTIVE:
Slight softening of sharp edges is acceptable as a byproduct of the clay medium, but preserve all facial proportions — interocular distance, nose length, lip fullness, ear shape, jawline — faithfully translated into the new material. The person must be immediately recognizable. No caricature exaggeration.

MEDIUM SIMULATION:
Re-render the subject as if physically constructed from polymer clay and captured under studio photography. Every element — skin, hair, clothing — should appear as hand-sculpted clay with visible tool marks, finger-impression textures, and authentic imperfections. NOT a smooth 3D render — a physical-craft simulation.

MATERIAL PROPERTIES:
Skin: matte clay in the subject's accurate tone with fingerprint micro-texture. Eyes: smooth glossy acrylic spheres with a single white highlight dot. Hair: individual clay ropes bundled and shaped. Lips: slightly over-rounded, waxy clay.

ENVIRONMENT:
A cozy miniature world — small wooden shelf, tiny potted succulents, miniature bookshelf with clay book spines, warm incandescent light from a tiny clay lamp.

OUTPUT MOOD: Laika Studios × Aardman. Warmth, craft, handmade soul.`,
  },
  {
    id: "editorial",
    title: "Editorial Fashion",
    category: "Editorial",
    tagline: "Vogue-ready. Architecturally lit.",
    color: "#e8e8e8",
    glow: "rgba(232,232,232,0.3)",
    bg: "linear-gradient(135deg,#0d0d0d 0%,#1a1a1a 100%)",
    image: "https://images.unsplash.com/photo-1509631179647-0177331693ae?w=600&q=80",
    prompt: `[MULTI-MODAL PORTRAIT TRANSFORMATION — EDITORIAL STUDIO FASHION]

IDENTITY PRESERVATION DIRECTIVE:
Skin texture, freckles, asymmetry, and unique facial geometry are editorial assets — preserve them completely. Do not apply beauty filters, skin smoothing, or feature correction of any kind. This is photojournalistic fidelity in a fashion context.

PHOTOGRAPHIC PARAMETERS:
Simulate a Hasselblad H6D with 80mm portrait lens, f/2.8, shooting on seamless white cyclorama. The image belongs between the pages of Italian Vogue or AnOther Magazine.

LIGHTING SCHEMA:
One large Profoto 7-foot octabank at 45° above-left. No fill — natural shadow falloff creates sculptural face definition. A subtle silver reflector provides the only bounce from below-right. The result: dramatic Rembrandt-adjacent lighting with fashion-forward sensibility.

STYLING:
Architectural oversized black wool coat, sharp lapels, no pattern, no logo. No jewelry. Expression: direct gaze, calm authority, no smile.

POSTPROCESSING:
Slightly desaturated skin tones. Elevated blacks. Ultra-sharp midtones. Film-shot aesthetic, not digital.

OUTPUT MOOD: Helmut Newton × Peter Lindbergh. Power, restraint, precision.`,
  },
  {
    id: "oilpainting",
    title: "Fine Art Oil",
    category: "Artistic",
    tagline: "Flemish masters. Living canvas.",
    color: "#d4a054",
    glow: "rgba(212,160,84,0.4)",
    bg: "linear-gradient(135deg,#0f0800 0%,#1e1000 100%)",
    image: "https://images.unsplash.com/photo-1579783902614-a3fb3927b6a5?w=600&q=80",
    prompt: `[MULTI-MODAL PORTRAIT TRANSFORMATION — FINE ART OIL PAINTING]

IDENTITY PRESERVATION DIRECTIVE:
You are translating the subject into a painted medium with commission-portrait faithfulness. Every distinguishing characteristic — curvature of the nose, the specific set of the eyes, the exact mouth shape — must be maintained. The result must be unmistakably this person, rendered in oil.

ARTISTIC PERIOD:
Dutch Golden Age / Flemish Baroque (circa 1630–1670). The visual grammar of Rembrandt van Rijn, Johannes Vermeer, Frans Hals. Loose gestural brushwork in fabric and background; tight glazed detail in face and hands; warm varnished tonal palette dominated by umbers, siennas, ochres; near-black background receding into atmospheric shadow.

PAINT RENDERING:
Skin built in visible glazing layers — raw umber underpainting showing through warm flesh-tone upper layers. Impasto texture on highlighted areas (forehead, nose tip, cheekbone). Visible individual brushstrokes in hair, cloth, background. Canvas linen-weave grain pressing through every passage.

LIGHTING: Single natural north-light source from the left. Classic Dutch chiaroscuro — the unlit side dissolving into warm shadow.

FRAME SIMULATION: Add aged gilt frame suggestion at image border.

OUTPUT MOOD: Rijksmuseum permanent collection. Gravitas, humanity, timelessness.`,
  },
  {
    id: "anime",
    title: "Anime Cel Portrait",
    category: "Fantasy",
    tagline: "Studio-grade. Unmistakably you.",
    color: "#ff4eb8",
    glow: "rgba(255,78,184,0.4)",
    bg: "linear-gradient(135deg,#0d001a 0%,#1a0033 100%)",
    image: "https://images.unsplash.com/photo-1534528741775-53994a69daeb?w=600&q=80",
    prompt: `[MULTI-MODAL PORTRAIT TRANSFORMATION — ANIME CEL PORTRAIT]

IDENTITY PRESERVATION DIRECTIVE:
The subject's most identifying features — eye shape, nose, lip form, facial structure, distinguishing marks — must be faithfully translated into the anime visual language. Do not default to generic anime eyes or simplified features. This person must be recognizable in the final result.

PRODUCTION STYLE:
Premium Japanese animation studio quality (Kyoto Animation, MAPPA, Production I.G. tier). This is a key visual or character art poster from a prestige anime series — not a filter, a genuine studio illustration.

LINEWORK:
Clean, confident black outlines of variable weight — thicker at outer contours, thinner for interior detail. No sketch marks, no rough lines.

COLORING METHOD:
Flat base colors with hard-edged cel shading — two or three tones per surface. Hair highlights: a single oval or angular specular shine mark. Skin tones: accurate to subject's real skin tone, adapted to anime palette conventions.

EYES: Adapted to anime proportion but maintaining the subject's unique eye shape. Iris: large, richly colored, multi-layered highlight system.

BACKGROUND: Soft bokeh light particles on a twilight blue-to-purple gradient.

OUTPUT MOOD: Demon Slayer × Your Name visual quality. Emotion, craft, identity.`,
  },
  {
    id: "watercolor",
    title: "Watercolor Botanica",
    category: "Artistic",
    tagline: "Ink blooms. Soft as morning.",
    color: "#4ade80",
    glow: "rgba(74,222,128,0.35)",
    bg: "linear-gradient(135deg,#001a0d 0%,#002e1a 100%)",
    image: "https://images.unsplash.com/photo-1557804506-669a67965ba0?w=600&q=80",
    prompt: `[MULTI-MODAL PORTRAIT TRANSFORMATION — WATERCOLOR BOTANICA]

IDENTITY PRESERVATION DIRECTIVE:
Watercolor introduces natural softening. Within those constraints, the subject's fundamental facial structure — proportions, eye placement, nose and lip form — must remain recognizable. The face receives more detail and restraint than surrounding botanical elements.

MEDIUM SIMULATION:
Authentic wet-on-wet and wet-on-dry watercolor on cold-press Arches 300gsm paper. Paper texture visible throughout — rough tooth catching pigment at unpredictable micro-points. Water blooms (backruns, cauliflower effects, tide marks) visible and intentional in background and foliage passages.

PORTRAIT TECHNIQUE:
The face rendered in controlled washes, wet-on-dry for sharp detail in eyes and lips, granulating pigments (ultramarine, burnt sienna) for skin passages. Lost and found edges: some face edges dissolve into the surrounding botanical wash; others are crisply defined.

BOTANICAL INTEGRATION:
Subject emerges from overscale botanical elements: peonies, Japanese anemone, fern fronds, eucalyptus stems. Painted with wet-on-wet abandon — blooming, flowing, color-mixing directly on page. Palette: sage green, warm rose, dusty mauve, golden ochre, deep forest.

BACKGROUND: White paper preserved in passages — the composition breathes.

OUTPUT MOOD: Sargent botanical studies × contemporary illustration. Alive, loose, luminous.`,
  },
  {
    id: "synthwave",
    title: "Retrowave Synthwave",
    category: "Editorial",
    tagline: "1987 never looked this good.",
    color: "#ff2d78",
    glow: "rgba(255,45,120,0.4)",
    bg: "linear-gradient(135deg,#0d0020 0%,#200040 100%)",
    image: "https://images.unsplash.com/photo-1518609571773-39b7d303a87b?w=600&q=80",
    prompt: `[MULTI-MODAL PORTRAIT TRANSFORMATION — RETROWAVE SYNTHWAVE]

IDENTITY PRESERVATION DIRECTIVE:
The subject's face must survive the aesthetic transformation intact. The Synthwave aesthetic is about environment, color palette, and light — not about altering the person. Maintain all facial features, proportions, and unique identifiers with precision.

ERA & AESTHETIC:
Hyper-stylized interpretation of 1980s retrofuturism through the modern Outrun / Synthwave visual movement. Kavinsky artwork, the Drive (2011) poster, Hotline Miami visual language. Not a lo-fi retro filter — a cinematic, ultra-high-resolution evocation.

ENVIRONMENT:
Open desert highway at dusk. Horizon gradient: hot magenta at base bleeding through orange and violet into deep purple-black sky. Large full moon on the horizon. Receding neon-pink wireframe grid extends to horizon. Low silhouetted palm trees at frame sides.

SUBJECT LIGHTING:
Backlit by the sunset gradient — warm orange/magenta rim light wrapping the silhouette. Face fill-lit by implied neon sign in cool pink. Chrome and glass catch anamorphic oval lens flares.

GRAPHIC ELEMENTS:
Fine horizontal scan lines at 5% opacity across the full image (CRT reference).

COLOR GRADE: Heavy teal/magenta split-tone. Crushed blacks. Glowing highlights. Extreme saturation in the magenta-cyan spectrum.

OUTPUT MOOD: Stranger Things × Miami Vice × Outrun. Pure nostalgia weaponized.`,
  },
  {
    id: "brutalist",
    title: "Brutalist Concrete",
    category: "Cinematic",
    tagline: "Soviet geometry. Human defiance.",
    color: "#a0a0a0",
    glow: "rgba(160,160,160,0.3)",
    bg: "linear-gradient(135deg,#080808 0%,#141414 100%)",
    image: "https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?w=600&q=80",
    prompt: `[MULTI-MODAL PORTRAIT TRANSFORMATION — BRUTALIST ENVIRONMENT PORTRAIT]

IDENTITY PRESERVATION DIRECTIVE:
The subject is the human focal point placed within an architectural environment. Their facial geometry, structure, and identifying features must remain completely unchanged. The transformation applies to the environment, lighting, and atmosphere — not the person.

ENVIRONMENT CONSTRUCTION:
Place the subject within a monumental Brutalist architectural interior — raw exposed concrete of National Theatre (London), Barbican Centre atrium, or Soviet-era Constructivist civic building. Characteristics: raw board-formed concrete with timber grain impressed into surface; massive geometric volumes; narrow slot windows letting in dramatic shafts of hard daylight; overwhelming scale that dwarfs the human subject.

COMPOSITIONAL RELATIONSHIP:
Subject in middle distance, facing camera, occupying 30–40% of frame height. Rest of frame dominated by concrete architecture — walls, monumental staircase, or vast ceiling — rendered in extreme detail.

PHOTOGRAPHIC STYLE:
Black and white, or deeply desaturated with slight warm sepia cast in highlights. Wide-to-normal lens (28–35mm equivalent). Grain: heavy, intentional — 35mm Kodak Tri-X film simulation.

LIGHTING: Harsh overhead daylight from a single slot window. Hard shadows. No fill.

OUTPUT MOOD: SOM Architecture × Sebastião Salgado. Monument, resistance, weight.`,
  },
];

const CATEGORIES = ["All", "Cinematic", "Fantasy", "Editorial", "Artistic"];

// ─── PARTICLES BACKGROUND ─────────────────────────────────────────────────────
function Particles() {
  return (
    <div style={{ position: "fixed", inset: 0, pointerEvents: "none", zIndex: 0, overflow: "hidden" }}>
      {/* Ambient orbs */}
      <div style={{
        position: "absolute", width: 600, height: 600, borderRadius: "50%",
        background: "radial-gradient(circle, rgba(99,102,241,0.12) 0%, transparent 70%)",
        top: -200, left: "50%", transform: "translateX(-50%)",
        animation: "orb1 8s ease-in-out infinite alternate"
      }} />
      <div style={{
        position: "absolute", width: 400, height: 400, borderRadius: "50%",
        background: "radial-gradient(circle, rgba(168,85,247,0.08) 0%, transparent 70%)",
        bottom: "10%", right: "-10%",
        animation: "orb2 10s ease-in-out infinite alternate"
      }} />
      {/* Grid lines */}
      <svg style={{ position: "absolute", inset: 0, width: "100%", height: "100%", opacity: 0.03 }}>
        <defs>
          <pattern id="grid" width="60" height="60" patternUnits="userSpaceOnUse">
            <path d="M 60 0 L 0 0 0 60" fill="none" stroke="#6366f1" strokeWidth="0.5"/>
          </pattern>
        </defs>
        <rect width="100%" height="100%" fill="url(#grid)" />
      </svg>
      <style>{`
        @keyframes orb1 { from { transform: translateX(-50%) scale(1); } to { transform: translateX(-50%) scale(1.15); } }
        @keyframes orb2 { from { transform: scale(1); } to { transform: scale(1.2) translate(-20px, -30px); } }
        @keyframes fadeUp { from { opacity:0; transform:translateY(24px); } to { opacity:1; transform:translateY(0); } }
        @keyframes shimmer { 0%,100% { opacity:0.5; } 50% { opacity:1; } }
        @keyframes spin { to { transform: rotate(360deg); } }
        @keyframes pulseRing { 0% { transform:scale(1); opacity:0.8; } 100% { transform:scale(1.8); opacity:0; } }
        @keyframes slideIn { from { opacity:0; transform:translateY(32px) scale(0.97); } to { opacity:1; transform:translateY(0) scale(1); } }
        @keyframes scanline { from { transform:translateY(-100%); } to { transform:translateY(100%); } }
      `}</style>
    </div>
  );
}

// ─── STYLE CARD ────────────────────────────────────────────────────────────────
function StyleCard({ style, isSelected, onClick }) {
  const [hovered, setHovered] = useState(false);

  return (
    <div
      onClick={onClick}
      onMouseEnter={() => setHovered(true)}
      onMouseLeave={() => setHovered(false)}
      style={{
        cursor: "pointer",
        borderRadius: 20,
        overflow: "hidden",
        border: `1px solid ${isSelected ? style.color : hovered ? "rgba(255,255,255,0.12)" : "rgba(255,255,255,0.06)"}`,
        background: "#0a0a14",
        boxShadow: isSelected
          ? `0 0 0 1px ${style.color}, 0 20px 60px -10px ${style.glow}, inset 0 1px 0 rgba(255,255,255,0.05)`
          : hovered
          ? `0 20px 40px -15px ${style.glow}, inset 0 1px 0 rgba(255,255,255,0.04)`
          : "inset 0 1px 0 rgba(255,255,255,0.03)",
        transform: isSelected ? "translateY(-4px) scale(1.01)" : hovered ? "translateY(-2px)" : "none",
        transition: "all 0.3s cubic-bezier(0.34,1.56,0.64,1)",
        position: "relative",
      }}
    >
      {/* Image */}
      <div style={{ position: "relative", aspectRatio: "3/4", overflow: "hidden" }}>
        <img
          src={style.image}
          alt={style.title}
          style={{
            width: "100%", height: "100%", objectFit: "cover",
            transform: hovered ? "scale(1.06)" : "scale(1)",
            transition: "transform 0.5s ease",
            display: "block",
          }}
        />
        {/* Gradient overlays */}
        <div style={{
          position: "absolute", inset: 0,
          background: "linear-gradient(to top, #0a0a14 0%, rgba(10,10,20,0.4) 50%, transparent 100%)"
        }} />
        <div style={{
          position: "absolute", inset: 0,
          background: `linear-gradient(135deg, ${style.color}22 0%, transparent 60%)`,
          opacity: hovered || isSelected ? 1 : 0,
          transition: "opacity 0.4s ease",
        }} />

        {/* Category badge */}
        <div style={{
          position: "absolute", top: 12, left: 12,
          background: "rgba(0,0,0,0.6)",
          backdropFilter: "blur(12px)",
          border: `1px solid ${style.color}50`,
          borderRadius: 100,
          padding: "4px 10px",
          display: "flex", alignItems: "center", gap: 5,
        }}>
          <div style={{ width: 5, height: 5, borderRadius: "50%", background: style.color, boxShadow: `0 0 6px ${style.color}` }} />
          <span style={{ fontSize: 9, letterSpacing: "0.15em", fontFamily: "monospace", color: style.color, fontWeight: 700, textTransform: "uppercase" }}>
            {style.category}
          </span>
        </div>

        {/* Selected checkmark */}
        {isSelected && (
          <div style={{
            position: "absolute", top: 12, right: 12,
            width: 28, height: 28, borderRadius: "50%",
            background: style.color,
            display: "flex", alignItems: "center", justifyContent: "center",
            fontSize: 14, color: "#000", fontWeight: 900,
            boxShadow: `0 0 20px ${style.glow}`,
            animation: "fadeUp 0.25s ease",
          }}>✓</div>
        )}
      </div>

      {/* Info */}
      <div style={{ padding: "16px 18px 18px" }}>
        <div style={{ fontSize: 15, fontWeight: 700, color: "#f1f5f9", marginBottom: 4, letterSpacing: "-0.02em" }}>
          {style.title}
        </div>
        <div style={{ fontSize: 11, color: "#64748b", fontStyle: "italic", marginBottom: 14 }}>
          {style.tagline}
        </div>
        <div style={{
          display: "flex", alignItems: "center", gap: 8,
          padding: "8px 12px",
          borderRadius: 8,
          background: isSelected ? `${style.color}18` : "rgba(255,255,255,0.03)",
          border: `1px solid ${isSelected ? style.color + "40" : "rgba(255,255,255,0.06)"}`,
          transition: "all 0.3s ease",
        }}>
          <div style={{
            width: 6, height: 6, borderRadius: "50%",
            background: style.color,
            boxShadow: isSelected ? `0 0 8px ${style.color}` : "none",
            animation: isSelected ? "shimmer 1.5s ease infinite" : "none",
          }} />
          <span style={{ fontSize: 9, fontFamily: "monospace", letterSpacing: "0.15em", textTransform: "uppercase", color: isSelected ? style.color : "#475569", fontWeight: 700 }}>
            {isSelected ? "Prompt Ready →" : "View Prompt"}
          </span>
        </div>
      </div>
    </div>
  );
}

// ─── PROMPT PANEL ──────────────────────────────────────────────────────────────
function PromptPanel({ style, onClose }) {
  const [copied, setCopied] = useState(false);
  const [activeTab, setActiveTab] = useState("prompt");

  const handleCopy = useCallback(async () => {
    try {
      await navigator.clipboard.writeText(style.prompt);
    } catch {
      const ta = document.createElement("textarea");
      ta.value = style.prompt;
      document.body.appendChild(ta);
      ta.select();
      document.execCommand("copy");
      document.body.removeChild(ta);
    }
    setCopied(true);
    setTimeout(() => setCopied(false), 2500);
  }, [style.prompt]);

  return (
    <div style={{
      borderRadius: 24,
      overflow: "hidden",
      border: `1px solid ${style.color}40`,
      background: "linear-gradient(145deg, #0c0c1a 0%, #08080f 100%)",
      boxShadow: `0 40px 80px -20px ${style.glow}, 0 0 0 1px ${style.color}20, inset 0 1px 0 rgba(255,255,255,0.05)`,
      animation: "slideIn 0.35s cubic-bezier(0.34,1.2,0.64,1) both",
    }}>
      {/* Panel header */}
      <div style={{
        display: "flex", alignItems: "center", justifyContent: "space-between",
        padding: "18px 24px",
        borderBottom: "1px solid rgba(255,255,255,0.05)",
        background: "rgba(255,255,255,0.02)",
      }}>
        <div style={{ display: "flex", alignItems: "center", gap: 12 }}>
          <div style={{
            width: 10, height: 10, borderRadius: "50%",
            background: style.color,
            boxShadow: `0 0 16px ${style.glow}`,
          }} />
          <div>
            <div style={{ fontSize: 15, fontWeight: 700, color: "#f1f5f9", letterSpacing: "-0.02em" }}>
              {style.title}
            </div>
            <div style={{ fontSize: 10, fontFamily: "monospace", color: "#475569", letterSpacing: "0.1em", textTransform: "uppercase", marginTop: 1 }}>
              Multi-Modal Prompt Script · Identity Preserved
            </div>
          </div>
        </div>
        <button
          onClick={onClose}
          style={{
            width: 32, height: 32, borderRadius: "50%",
            border: "1px solid rgba(255,255,255,0.08)",
            background: "rgba(255,255,255,0.04)",
            color: "#64748b", fontSize: 14, cursor: "pointer",
            display: "flex", alignItems: "center", justifyContent: "center",
            transition: "all 0.2s",
          }}
        >✕</button>
      </div>

      {/* Two-column layout */}
      <div style={{ display: "flex", flexDirection: "row", minHeight: 420 }}>
        {/* Left: image + how-to */}
        <div style={{ width: "38%", minWidth: 220, position: "relative", flexShrink: 0 }}>
          <div style={{ height: "100%", minHeight: 420, position: "relative", overflow: "hidden" }}>
            <img
              src={style.image}
              alt={style.title}
              style={{ width: "100%", height: "100%", objectFit: "cover", display: "block" }}
            />
            <div style={{
              position: "absolute", inset: 0,
              background: `linear-gradient(to right, transparent 50%, #0c0c1a 100%), linear-gradient(to top, #0c0c1a 0%, transparent 50%)`
            }} />
            <div style={{
              position: "absolute", inset: 0,
              background: `${style.color}15`
            }} />
            {/* Steps overlay */}
            <div style={{ position: "absolute", bottom: 0, left: 0, right: 0, padding: 20 }}>
              <div style={{ fontSize: 9, fontFamily: "monospace", color: style.color, letterSpacing: "0.15em", textTransform: "uppercase", marginBottom: 10, fontWeight: 700 }}>
                How to use
              </div>
              {[
                "Copy the prompt below",
                "Open ChatGPT, Gemini, or Claude",
                "Upload your portrait photo",
                "Paste prompt alongside it",
              ].map((step, i) => (
                <div key={i} style={{ display: "flex", alignItems: "flex-start", gap: 8, marginBottom: 7 }}>
                  <div style={{
                    width: 16, height: 16, borderRadius: "50%", flexShrink: 0,
                    background: `${style.color}25`, border: `1px solid ${style.color}60`,
                    display: "flex", alignItems: "center", justifyContent: "center",
                    fontSize: 8, color: style.color, fontFamily: "monospace", fontWeight: 700,
                  }}>{i + 1}</div>
                  <span style={{ fontSize: 10, color: "rgba(255,255,255,0.6)", lineHeight: 1.5 }}>{step}</span>
                </div>
              ))}
            </div>
          </div>
        </div>

        {/* Right: prompt */}
        <div style={{ flex: 1, display: "flex", flexDirection: "column", borderLeft: "1px solid rgba(255,255,255,0.05)" }}>
          {/* Tab bar */}
          <div style={{
            display: "flex", alignItems: "center", justifyContent: "space-between",
            padding: "12px 20px",
            borderBottom: "1px solid rgba(255,255,255,0.05)",
          }}>
            <div style={{ display: "flex", gap: 4 }}>
              {["prompt", "tips"].map((tab) => (
                <button
                  key={tab}
                  onClick={() => setActiveTab(tab)}
                  style={{
                    padding: "5px 14px", borderRadius: 8, cursor: "pointer",
                    fontSize: 10, fontFamily: "monospace", letterSpacing: "0.1em", textTransform: "uppercase", fontWeight: 700,
                    border: `1px solid ${activeTab === tab ? style.color + "50" : "transparent"}`,
                    background: activeTab === tab ? `${style.color}15` : "transparent",
                    color: activeTab === tab ? style.color : "#475569",
                    transition: "all 0.2s",
                  }}
                >{tab}</button>
              ))}
            </div>
            <button
              onClick={handleCopy}
              style={{
                display: "flex", alignItems: "center", gap: 8,
                padding: "8px 20px", borderRadius: 10, cursor: "pointer",
                fontSize: 10, fontFamily: "monospace", letterSpacing: "0.12em", textTransform: "uppercase", fontWeight: 800,
                border: copied ? "1px solid #22c55e80" : `1px solid ${style.color}`,
                background: copied
                  ? "linear-gradient(135deg,#14532d20,#16a34a20)"
                  : `linear-gradient(135deg,${style.color}25,${style.color}10)`,
                color: copied ? "#22c55e" : style.color,
                boxShadow: copied ? "0 0 20px rgba(34,197,94,0.3)" : `0 0 20px ${style.glow}`,
                transition: "all 0.3s cubic-bezier(0.34,1.56,0.64,1)",
                transform: copied ? "scale(0.97)" : "scale(1)",
              }}
            >
              <span style={{ fontSize: 14 }}>{copied ? "✓" : "⎘"}</span>
              <span>{copied ? "Copied!" : "Copy Prompt"}</span>
            </button>
          </div>

          {/* Content */}
          <div style={{ flex: 1, overflow: "auto", padding: 20, maxHeight: 360 }}>
            {activeTab === "prompt" ? (
              <pre style={{
                fontFamily: "monospace", fontSize: 11, lineHeight: 1.9,
                color: "#94a3b8", whiteSpace: "pre-wrap", wordBreak: "break-word",
                margin: 0,
              }}>
                <span style={{ color: style.color, fontWeight: 700 }}>{style.prompt.split("\n")[0]}</span>
                {"\n" + style.prompt.split("\n").slice(1).join("\n")}
              </pre>
            ) : (
              <div style={{ display: "flex", flexDirection: "column", gap: 12 }}>
                {[
                  { icon: "🔒", title: "Identity Lock", desc: "These prompts are specifically engineered to preserve your facial structure. The AI reads your face as a 'locked layer' — only the environment transforms." },
                  { icon: "🎯", title: "Best Models", desc: "Works best with GPT-4o, Gemini 1.5 Pro, and Claude 3.5 Sonnet (multimodal). Upload your photo first, then paste the prompt." },
                  { icon: "📸", title: "Photo Tips", desc: "Use a high-quality frontal portrait with good lighting. Clear face visibility = better identity preservation in the output." },
                  { icon: "⚡", title: "Iterate Fast", desc: "If the first result isn't perfect, try adding 'Pay special attention to preserving the subject's exact facial features' at the end of the prompt." },
                ].map((tip, i) => (
                  <div key={i} style={{
                    padding: "12px 14px", borderRadius: 10,
                    background: "rgba(255,255,255,0.02)",
                    border: "1px solid rgba(255,255,255,0.05)",
                  }}>
                    <div style={{ display: "flex", alignItems: "center", gap: 8, marginBottom: 5 }}>
                      <span>{tip.icon}</span>
                      <span style={{ fontSize: 11, fontWeight: 700, color: "#e2e8f0" }}>{tip.title}</span>
                    </div>
                    <p style={{ fontSize: 11, color: "#64748b", lineHeight: 1.6, margin: 0 }}>{tip.desc}</p>
                  </div>
                ))}
              </div>
            )}
          </div>
        </div>
      </div>
    </div>
  );
}

// ─── MAIN APP ──────────────────────────────────────────────────────────────────
export default function ILovePrompt() {
  const [activeCategory, setActiveCategory] = useState("All");
  const [selectedId, setSelectedId] = useState(null);

  const filtered = STYLES.filter(
    (s) => activeCategory === "All" || s.category === activeCategory
  );
  const selected = STYLES.find((s) => s.id === selectedId);

  const handleCardClick = (id) => {
    setSelectedId((prev) => (prev === id ? null : id));
  };

  return (
    <div style={{
      minHeight: "100vh",
      background: "#06060f",
      color: "#f1f5f9",
      fontFamily: "-apple-system, BlinkMacSystemFont, 'Inter', 'Segoe UI', sans-serif",
      position: "relative",
    }}>
      <Particles />

      {/* ── HEADER ── */}
      <header style={{
        position: "sticky", top: 0, zIndex: 50,
        borderBottom: "1px solid rgba(255,255,255,0.05)",
        background: "rgba(6,6,15,0.85)",
        backdropFilter: "blur(20px)",
      }}>
        <div style={{ maxWidth: 1280, margin: "0 auto", padding: "0 24px", height: 64, display: "flex", alignItems: "center", justifyContent: "space-between" }}>
          {/* Logo */}
          <div style={{ display: "flex", alignItems: "center", gap: 10 }}>
            <div style={{
              width: 36, height: 36, borderRadius: 10,
              background: "linear-gradient(135deg, #6366f1 0%, #a855f7 100%)",
              display: "flex", alignItems: "center", justifyContent: "center",
              boxShadow: "0 0 24px rgba(99,102,241,0.5)",
              fontSize: 18, fontWeight: 900, color: "#fff",
            }}>✦</div>
            <div>
              <div style={{ fontSize: 16, fontWeight: 800, letterSpacing: "-0.03em", color: "#fff" }}>
                iLovePrompt
              </div>
              <div style={{ fontSize: 9, fontFamily: "monospace", color: "#475569", letterSpacing: "0.15em", textTransform: "uppercase", marginTop: -1 }}>
                Portrait AI
              </div>
            </div>
          </div>

          {/* Center label */}
          <div style={{
            display: "flex", alignItems: "center", gap: 8,
            padding: "6px 14px", borderRadius: 100,
            border: "1px solid rgba(99,102,241,0.3)",
            background: "rgba(99,102,241,0.06)",
          }}>
            <div style={{ width: 5, height: 5, borderRadius: "50%", background: "#818cf8", animation: "shimmer 2s ease infinite" }} />
            <span style={{ fontSize: 10, fontFamily: "monospace", color: "#818cf8", letterSpacing: "0.1em" }}>
              ZERO API · 100% CLIENT-SIDE · FREE FOREVER
            </span>
          </div>

          <div style={{ fontSize: 11, fontFamily: "monospace", color: "#334155", letterSpacing: "0.05em" }}>
            {STYLES.length} Styles Available
          </div>
        </div>
      </header>

      <main style={{ maxWidth: 1280, margin: "0 auto", padding: "0 24px 80px", position: "relative", zIndex: 1 }}>

        {/* ── HERO ── */}
        <div style={{ textAlign: "center", padding: "72px 0 60px", animation: "fadeUp 0.6s ease both" }}>
          <div style={{
            display: "inline-flex", alignItems: "center", gap: 8,
            padding: "6px 18px", borderRadius: 100,
            border: "1px solid rgba(168,85,247,0.3)",
            background: "rgba(168,85,247,0.06)",
            marginBottom: 28,
          }}>
            <span style={{ fontSize: 12 }}>✦</span>
            <span style={{ fontSize: 10, fontFamily: "monospace", color: "#c084fc", letterSpacing: "0.15em", textTransform: "uppercase" }}>
              Your face, preserved. The world, transformed.
            </span>
          </div>

          <h1 style={{
            fontSize: "clamp(40px, 7vw, 72px)",
            fontWeight: 900,
            letterSpacing: "-0.04em",
            lineHeight: 1.05,
            margin: "0 0 20px",
            color: "#fff",
          }}>
            Pick a style.{" "}
            <span style={{
              background: "linear-gradient(135deg, #6366f1 0%, #a855f7 50%, #ec4899 100%)",
              WebkitBackgroundClip: "text",
              WebkitTextFillColor: "transparent",
              backgroundClip: "text",
            }}>
              Copy the prompt.
            </span>
            <br />Transform yourself.
          </h1>

          <p style={{ fontSize: "clamp(14px, 2vw, 17px)", color: "#64748b", maxWidth: 560, margin: "0 auto 40px", lineHeight: 1.7 }}>
            Precision-engineered AI prompts that preserve your identity while transforming your portrait into any aesthetic. Works with ChatGPT, Gemini, and Claude.
          </p>

          {/* Steps row */}
          <div style={{ display: "flex", justifyContent: "center", gap: 0, flexWrap: "wrap" }}>
            {[
              { n: 1, label: "Choose a style", icon: "◉" },
              { n: 2, label: "Copy the prompt", icon: "⎘" },
              { n: 3, label: "Paste + upload photo", icon: "✦" },
            ].map((step, i) => (
              <div key={i} style={{ display: "flex", alignItems: "center" }}>
                <div style={{
                  display: "flex", alignItems: "center", gap: 10,
                  padding: "10px 20px", borderRadius: 12,
                  background: "rgba(255,255,255,0.02)",
                  border: "1px solid rgba(255,255,255,0.06)",
                  margin: "4px",
                }}>
                  <div style={{
                    width: 28, height: 28, borderRadius: 8,
                    background: "linear-gradient(135deg, #6366f1, #a855f7)",
                    display: "flex", alignItems: "center", justifyContent: "center",
                    fontSize: 13, color: "#fff",
                  }}>{step.icon}</div>
                  <span style={{ fontSize: 12, color: "#94a3b8", fontWeight: 500 }}>{step.label}</span>
                </div>
                {i < 2 && (
                  <div style={{ color: "#1e293b", fontSize: 18, margin: "0 -2px" }}>→</div>
                )}
              </div>
            ))}
          </div>
        </div>

        {/* ── FILTER PILLS ── */}
        <div style={{ display: "flex", alignItems: "center", gap: 8, marginBottom: 32, flexWrap: "wrap" }}>
          <span style={{ fontSize: 10, fontFamily: "monospace", color: "#334155", letterSpacing: "0.15em", textTransform: "uppercase", marginRight: 4 }}>Filter:</span>
          {CATEGORIES.map((cat) => {
            const isActive = activeCategory === cat;
            return (
              <button
                key={cat}
                onClick={() => { setActiveCategory(cat); setSelectedId(null); }}
                style={{
                  padding: "6px 16px", borderRadius: 100, cursor: "pointer",
                  fontSize: 10, fontFamily: "monospace", letterSpacing: "0.12em", textTransform: "uppercase", fontWeight: 700,
                  border: isActive ? "1px solid #6366f1" : "1px solid rgba(255,255,255,0.08)",
                  background: isActive ? "linear-gradient(135deg,#6366f1,#7c3aed)" : "rgba(255,255,255,0.02)",
                  color: isActive ? "#fff" : "#475569",
                  boxShadow: isActive ? "0 0 20px rgba(99,102,241,0.4)" : "none",
                  transition: "all 0.2s ease",
                }}
              >{cat}</button>
            );
          })}
          <span style={{ marginLeft: "auto", fontSize: 10, fontFamily: "monospace", color: "#334155" }}>
            {filtered.length} styles
          </span>
        </div>

        {/* ── GRID ── */}
        <div style={{ display: "grid", gridTemplateColumns: "repeat(auto-fill, minmax(220px, 1fr))", gap: 20 }}>
          {filtered.map((style) => (
            <StyleCard
              key={style.id}
              style={style}
              isSelected={selectedId === style.id}
              onClick={() => handleCardClick(style.id)}
            />
          ))}
        </div>

        {/* ── PROMPT PANEL ── */}
        {selected && filtered.some((s) => s.id === selectedId) && (
          <div style={{ marginTop: 32 }}>
            <PromptPanel
              key={selectedId}
              style={selected}
              onClose={() => setSelectedId(null)}
            />
          </div>
        )}

        {/* ── FOOTER ── */}
        <div style={{
          marginTop: 80, paddingTop: 32,
          borderTop: "1px solid rgba(255,255,255,0.04)",
          display: "flex", alignItems: "center", justifyContent: "space-between",
          flexWrap: "wrap", gap: 12,
        }}>
          <div style={{ display: "flex", alignItems: "center", gap: 8 }}>
            <div style={{
              width: 24, height: 24, borderRadius: 6,
              background: "linear-gradient(135deg,#6366f1,#a855f7)",
              display: "flex", alignItems: "center", justifyContent: "center",
              fontSize: 11, color: "#fff",
            }}>✦</div>
            <span style={{ fontSize: 12, color: "#334155", fontWeight: 600 }}>iLovePrompt</span>
          </div>
          <span style={{ fontSize: 10, fontFamily: "monospace", color: "#1e293b", letterSpacing: "0.1em" }}>
            WORKS WITH CHATGPT · GEMINI · CLAUDE · GROK
          </span>
          <span style={{ fontSize: 10, fontFamily: "monospace", color: "#1e293b" }}>
            NO BACKEND · FREE FOREVER
          </span>
        </div>
      </main>
    </div>
  );
}
