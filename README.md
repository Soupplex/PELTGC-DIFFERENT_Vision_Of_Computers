  PELTGC — Complete Documentation  :root { --bg: #050507; --surface: #0a0a0f; --border: #151520; --border-bright: #1e1e30; --accent: #00ff88; --accent2: #00aaff; --warn: #ffaa00; --danger: #ff4455; --text: #ff3333; --text-dim: #aa2222; --text-muted: #cc2222; --font-display: 'Syne', sans-serif; --font-mono: 'IBM Plex Mono', monospace; } \* { margin: 0; padding: 0; box-sizing: border-box; } html { scroll-behavior: smooth; } body { background: var(--bg); color: var(--text); font-family: var(--font-mono); font-size: 13px; line-height: 1.7; overflow-x: hidden; } body::before { content: ''; position: fixed; inset: 0; background-image: url("data:image/svg+xml,%3Csvg viewBox='0 0 256 256' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noise'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.9' numOctaves='4' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noise)' opacity='0.04'/%3E%3C/svg%3E"); pointer-events: none; z-index: 1000; opacity: 0.35; } body::after { content: ''; position: fixed; inset: 0; background: repeating-linear-gradient(0deg, transparent, transparent 2px, rgba(0,0,0,0.07) 2px, rgba(0,0,0,0.07) 4px); pointer-events: none; z-index: 999; } /\* NAV \*/ .sidenav { position: fixed; left: 0; top: 0; bottom: 0; width: 220px; background: rgba(5,5,7,0.97); border-right: 1px solid var(--border-bright); padding: 40px 0; overflow-y: auto; z-index: 100; } .sidenav-title { font-family: var(--font-display); font-size: 0.9em; font-weight: 800; color: var(--accent); padding: 0 20px 24px; letter-spacing: -0.5px; border-bottom: 1px solid var(--border); margin-bottom: 16px; } .sidenav a { display: block; padding: 6px 20px; font-size: 0.62em; color: var(--text-muted); text-decoration: none; letter-spacing: 1px; transition: color 0.15s, border-color 0.15s; border-left: 2px solid transparent; } .sidenav a:hover { color: var(--text); border-left-color: var(--accent); } .sidenav .nav-group { font-size: 0.58em; color: var(--text-muted); letter-spacing: 3px; text-transform: uppercase; padding: 16px 20px 6px; opacity: 0.5; } /\* MAIN \*/ .main { margin-left: 220px; max-width: 860px; padding: 0 48px 100px; } @media (max-width: 768px) { .sidenav { display: none; } .main { margin-left: 0; padding: 0 20px 80px; } } /\* HERO \*/ .hero { padding: 80px 0 56px; border-bottom: 1px solid var(--border-bright); margin-bottom: 64px; position: relative; } .hero-eyebrow { font-size: 0.62em; color: var(--accent); letter-spacing: 4px; text-transform: uppercase; margin-bottom: 20px; display: flex; align-items: center; gap: 10px; } .hero-eyebrow::before { content: ''; display: block; width: 24px; height: 1px; background: var(--accent); } h1 { font-family: var(--font-display); font-size: clamp(3em, 7vw, 5.5em); font-weight: 800; color: #fff; line-height: 1; letter-spacing: -3px; margin-bottom: 14px; } h1 .acc { color: var(--accent); } .hero-tagline { font-size: 0.72em; color: var(--text-dim); letter-spacing: 3px; text-transform: uppercase; margin-bottom: 28px; } .hero-manifesto { font-family: var(--font-display); font-size: 1.2em; font-weight: 700; color: rgba(255,255,255,0.12); line-height: 1.6; max-width: 560px; } .hero-manifesto strong { color: rgba(255,255,255,0.85); } .hero-bar { position: absolute; bottom: -1px; left: 0; height: 2px; width: 100px; background: linear-gradient(90deg, var(--accent), transparent); } /\* CHAPTER \*/ .chapter { margin-bottom: 80px; scroll-margin-top: 40px; } .chapter-header { display: flex; align-items: flex-start; gap: 20px; margin-bottom: 32px; padding-bottom: 16px; border-bottom: 1px solid var(--border-bright); } .chapter-num { font-family: var(--font-display); font-size: 3em; font-weight: 800; color: var(--border-bright); line-height: 1; flex-shrink: 0; margin-top: -4px; } .chapter-meta { flex: 1; } .chapter-label { font-size: 0.6em; letter-spacing: 4px; text-transform: uppercase; color: var(--accent2); margin-bottom: 4px; } h2 { font-family: var(--font-display); font-size: 1.5em; font-weight: 700; color: #fff; letter-spacing: -0.5px; } h3 { font-family: var(--font-display); font-size: 0.95em; font-weight: 700; color: var(--text); margin: 28px 0 12px; letter-spacing: -0.3px; } p { color: var(--text-dim); font-size: 0.75em; line-height: 1.9; margin-bottom: 14px; max-width: 640px; } p strong { color: var(--text); font-weight: 500; } .highlight { background: rgba(0,255,136,0.05); border: 1px solid rgba(0,255,136,0.15); border-radius: 6px; padding: 16px 20px; margin: 20px 0; } .highlight p { color: var(--text); margin: 0; } /\* SUBSECTION \*/ .sub { margin: 24px 0; } .sub-label { font-size: 0.6em; letter-spacing: 3px; text-transform: uppercase; color: var(--accent2); margin-bottom: 12px; display: flex; align-items: center; gap: 8px; } .sub-label::after { content: ''; flex: 1; height: 1px; background: linear-gradient(90deg, var(--border-bright), transparent); } /\* COMPARE \*/ .compare { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; margin: 16px 0; } @media (max-width: 600px) { .compare { grid-template-columns: 1fr; } } .cblock { border-radius: 6px; padding: 16px 18px; border: 1px solid var(--border-bright); } .cblock.bad { border-color: rgba(255,68,85,0.2); background: rgba(255,68,85,0.025); } .cblock.good { border-color: rgba(0,255,136,0.2); background: rgba(0,255,136,0.025); } .cblock-title { font-size: 0.6em; letter-spacing: 2px; margin-bottom: 12px; font-weight: 500; } .cblock.bad .cblock-title { color: var(--danger); } .cblock.good .cblock-title { color: var(--accent); } .code-line { font-size: 0.68em; line-height: 2.2; } .cblock.bad .code-line { color: rgba(255,136,136,0.65); } .cblock.good .code-line { color: rgba(136,255,136,0.85); } .code-dim { color: var(--text-muted) !important; font-style: italic; } /\* POOL VIZ \*/ .pool-box { border: 1px solid rgba(0,255,136,0.3); border-radius: 8px; padding: 20px; background: rgba(0,255,136,0.015); position: relative; box-shadow: 0 0 60px rgba(0,255,136,0.04); margin: 16px 0; } .pool-box-label { position: absolute; top: -10px; left: 14px; background: var(--bg); color: var(--accent); font-size: 0.6em; padding: 0 8px; letter-spacing: 2px; } .sub-pools { display: grid; grid-template-columns: repeat(auto-fill, minmax(120px, 1fr)); gap: 10px; } .sp { border: 1px solid var(--border-bright); border-radius: 6px; padding: 12px; background: var(--surface); transition: border-color 0.2s; } .sp:hover { border-color: var(--accent2); } .sp-title { color: var(--warn); font-size: 0.6em; letter-spacing: 2px; margin-bottom: 10px; } .ins { display: flex; justify-content: space-between; gap: 8px; padding: 3px 0; font-size: 0.63em; border-bottom: 1px solid var(--border); } .ins:last-child { border: none; } .idx { color: var(--danger); opacity: 0.6; } .ok { color: var(--accent); } .lazy { color: var(--text-muted); } .merged { color: var(--accent2); } /\* THREAD VIZ \*/ .thread-diagram { display: flex; flex-direction: column; gap: 10px; margin: 16px 0; } .thread-row { display: flex; align-items: center; gap: 10px; font-size: 0.68em; } .thread-label { width: 70px; color: var(--accent2); flex-shrink: 0; } .thread-bar { height: 32px; border-radius: 4px; display: flex; align-items: center; padding: 0 12px; font-size: 0.85em; flex: 1; } .tbar-dup { background: rgba(255,68,85,0.1); border: 1px solid rgba(255,68,85,0.2); color: rgba(255,136,136,0.7); } .tbar-work { background: rgba(0,255,136,0.08); border: 1px solid rgba(0,255,136,0.2); color: rgba(136,255,136,0.9); } .tbar-ahead { background: rgba(0,170,255,0.08); border: 1px solid rgba(0,170,255,0.2); color: rgba(136,200,255,0.9); } .tbar-free { background: transparent; border: 1px solid var(--border); color: var(--text-muted); } .thread-result { width: 120px; color: var(--text-dim); font-size: 0.85em; flex-shrink: 0; } /\* TIERS \*/ .tiers { display: flex; flex-direction: column; gap: 8px; margin: 16px 0; } .tier { display: flex; align-items: flex-start; gap: 16px; padding: 14px 18px; border: 1px solid var(--border-bright); border-radius: 6px; transition: transform 0.2s; } .tier:hover { transform: translateX(4px); } .tier.common { border-left: 3px solid var(--accent); } .tier.rare { border-left: 3px solid var(--warn); } .tier.promoted { border-left: 3px solid var(--accent2); } .tier-lbl { width: 80px; font-size: 0.62em; letter-spacing: 2px; font-weight: 500; flex-shrink: 0; } .tier.common .tier-lbl { color: var(--accent); } .tier.rare .tier-lbl { color: var(--warn); } .tier.promoted .tier-lbl { color: var(--accent2); } .tier-desc { color: var(--text-dim); font-size: 0.68em; flex: 1; } .tier-tag { font-size: 0.58em; padding: 2px 10px; border-radius: 20px; flex-shrink: 0; align-self: center; } .tier.common .tier-tag { background: rgba(0,255,136,0.1); color: var(--accent); } .tier.rare .tier-tag { background: rgba(255,170,0,0.1); color: var(--warn); } .tier.promoted .tier-tag { background: rgba(0,170,255,0.1); color: var(--accent2); } /\* POOL HIERARCHY \*/ .hierarchy { display: flex; flex-direction: column; gap: 6px; margin: 16px 0; } .hlevel { border: 1px solid var(--border-bright); border-radius: 6px; padding: 12px 16px; font-size: 0.68em; display: flex; align-items: center; gap: 14px; } .hlevel.os { border-color: rgba(0,255,136,0.3); background: rgba(0,255,136,0.03); } .hlevel.game { border-color: rgba(0,170,255,0.3); background: rgba(0,170,255,0.03); } .hlevel.session { border-color: rgba(255,170,0,0.3); background: rgba(255,170,0,0.03); } .hlevel-name { width: 80px; font-weight: 500; flex-shrink: 0; } .hlevel.os .hlevel-name { color: var(--accent); } .hlevel.game .hlevel-name { color: var(--accent2); } .hlevel.session .hlevel-name { color: var(--warn); } .hlevel-desc { color: var(--text-dim); flex: 1; } .hlevel-tag { color: var(--text-muted); font-size: 0.85em; } /\* NETWORK \*/ .net-compare { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; margin: 16px 0; } .net-block { border: 1px solid var(--border-bright); border-radius: 6px; padding: 16px; } .net-block.bad { border-color: rgba(255,68,85,0.2); } .net-block.good { border-color: rgba(0,255,136,0.2); } .net-title { font-size: 0.6em; letter-spacing: 2px; margin-bottom: 12px; } .net-block.bad .net-title { color: var(--danger); } .net-block.good .net-title { color: var(--accent); } .pkt { background: rgba(255,255,255,0.02); border-radius: 4px; padding: 10px; font-size: 0.65em; line-height: 2.2; } .pkt.bad-pkt { color: rgba(255,136,136,0.6); } .pkt-number { font-family: var(--font-display); font-size: 4em; font-weight: 800; color: var(--accent); text-align: center; padding: 20px 0; line-height: 1; } .pkt-note { color: var(--text-dim); font-size: 0.62em; margin-top: 8px; } /\* PGRID \*/ .pgrid { display: grid; grid-template-columns: repeat(4, 1fr); gap: 8px; margin: 16px 0; } .pcell { border: 1px solid var(--border-bright); border-radius: 6px; padding: 14px 10px; text-align: center; font-size: 0.63em; } .pcell.active { border-color: rgba(0,255,136,0.35); background: rgba(0,255,136,0.03); } .pcell-size { font-family: var(--font-display); font-size: 1.8em; font-weight: 700; color: var(--accent2); display: block; margin-bottom: 4px; } .pcell-core { color: var(--text-dim); font-size: 0.85em; margin-top: 4px; } /\* SECURITY \*/ .sec-rows { display: flex; flex-direction: column; gap: 6px; margin: 16px 0; } .sec-row { display: flex; align-items: center; gap: 14px; padding: 10px 16px; border: 1px solid var(--border-bright); border-radius: 6px; font-size: 0.68em; transition: border-color 0.2s; } .sec-row.death { border-color: rgba(255,0,0,0.2); background: rgba(255,0,0,0.02); } .sec-attempt { color: var(--danger); width: 80px; flex-shrink: 0; font-size: 0.9em; } .sec-desc { color: var(--text-dim); flex: 1; } .sec-result { color: var(--text-muted); font-size: 0.9em; } .sec-row.death .sec-result { color: var(--danger); } /\* NDF \*/ .ndf { display: flex; flex-direction: column; gap: 8px; margin: 16px 0; } .nrow { display: flex; align-items: center; gap: 12px; font-size: 0.68em; } .nframe { border: 1px solid var(--border-bright); border-radius: 4px; padding: 4px 12px; width: 80px; text-align: center; } .nframe.changed { border-color: rgba(255,170,0,0.4); color: var(--warn); } .nframe.same { border-color: rgba(0,255,136,0.4); color: var(--accent); } .narr { color: var(--text-muted); } .nres { color: var(--text-dim); } .nres.skip { color: var(--accent); } .nres.render { color: var(--warn); } /\* VIDEO FRAMES \*/ .vframes { display: flex; gap: 6px; flex-wrap: wrap; margin: 16px 0; } .vf { border: 1px solid var(--border-bright); border-radius: 4px; padding: 8px 12px; font-size: 0.62em; text-align: center; line-height: 2; min-width: 60px; transition: transform 0.15s; } .vf:hover { transform: translateY(-2px); } .vf.new { border-color: rgba(255,170,0,0.4); color: var(--warn); } .vf.hit { border-color: rgba(0,255,136,0.4); color: var(--accent); } .vf-label { color: var(--text-muted); font-size: 0.9em; } /\* POINTER \*/ .ptr-grid { display: grid; grid-template-columns: 1fr 1fr; gap: 12px; margin: 16px 0; } .ptr-section { padding: 16px; border: 1px solid var(--border-bright); border-radius: 6px; } .ptr-title { font-size: 0.6em; letter-spacing: 2px; margin-bottom: 14px; font-weight: 500; } .ptr-title.bad { color: var(--danger); } .ptr-title.good { color: var(--accent); } .ptr-row { display: flex; align-items: center; gap: 10px; margin-bottom: 8px; font-size: 0.68em; } .pname { color: var(--text-dim); width: 60px; } .arrow { color: var(--text-muted); } .addr { padding: 2px 10px; border-radius: 3px; font-size: 0.9em; } .addr.da { background: rgba(255,68,85,0.1); border: 1px solid rgba(255,68,85,0.2); color: rgba(255,136,136,0.8); } .addr.ma { background: rgba(0,255,136,0.08); border: 1px solid rgba(0,255,136,0.2); color: rgba(136,255,136,0.9); } /\* LANGUAGE \*/ .code-block { background: var(--surface); border: 1px solid var(--border-bright); border-radius: 6px; padding: 18px 20px; margin: 16px 0; font-size: 0.72em; line-height: 2.2; position: relative; } .code-block.bad { border-color: rgba(255,68,85,0.2); } .code-block.good { border-color: rgba(0,255,136,0.2); } .code-tag { position: absolute; top: -9px; right: 12px; background: var(--bg); font-size: 0.58em; padding: 0 8px; letter-spacing: 2px; } .code-block.bad .code-tag { color: var(--danger); } .code-block.good .code-tag { color: var(--accent); } .kw { color: var(--accent2); } .kw2 { color: var(--accent); } .kw3 { color: var(--warn); } .val { color: rgba(255,170,100,0.9); } .cmt { color: var(--text-muted); font-style: italic; } .bad-code { color: rgba(255,136,136,0.6); } .good-code { color: rgba(136,255,136,0.85); } /\* ERROR MESSAGES \*/ .error-msgs { display: flex; flex-direction: column; gap: 8px; margin: 16px 0; } .err-row { display: flex; align-items: flex-start; gap: 14px; padding: 12px 16px; border: 1px solid var(--border-bright); border-radius: 6px; font-size: 0.68em; } .err-row.old { border-color: rgba(255,68,85,0.2); background: rgba(255,68,85,0.02); } .err-row.new { border-color: rgba(0,255,136,0.2); background: rgba(0,255,136,0.02); } .err-tag { width: 70px; flex-shrink: 0; font-size: 0.85em; font-weight: 500; } .err-row.old .err-tag { color: var(--danger); } .err-row.new .err-tag { color: var(--accent); } .err-msg { flex: 1; } .err-row.old .err-msg { color: rgba(255,136,136,0.6); } .err-row.new .err-msg { color: rgba(136,255,136,0.85); } /\* NAMING \*/ .name-decode { display: flex; flex-wrap: wrap; gap: 8px; margin: 16px 0; } .name-part { border: 1px solid var(--border-bright); border-radius: 6px; padding: 12px 16px; text-align: center; min-width: 80px; } .name-part-val { font-family: var(--font-display); font-size: 1.3em; font-weight: 700; margin-bottom: 6px; } .name-part-desc { font-size: 0.6em; color: var(--text-dim); letter-spacing: 1px; } .np-brand .name-part-val { color: var(--accent); } .np-philosophy .name-part-val { color: var(--accent2); } .np-reliability .name-part-val { color: var(--warn); } .np-revision .name-part-val { color: rgba(200,200,255,0.8); } .np-mode .name-part-val { color: rgba(255,200,100,0.8); } /\* NOTE \*/ .note { color: var(--text-dim); font-size: 0.65em; margin-top: 12px; padding: 10px 14px; border-left: 2px solid var(--border-bright); line-height: 1.8; } /\* QUOTE \*/ .quote { font-family: var(--font-display); font-size: 1.05em; font-weight: 700; color: rgba(255,255,255,0.5); border-left: 3px solid var(--accent); padding: 12px 20px; margin: 24px 0; font-style: italic; } /\* DIVIDER \*/ .divider { height: 1px; background: linear-gradient(90deg, transparent, var(--border-bright), transparent); margin: 56px 0; } /\* GLOW DOT \*/ .glow-dot { display: inline-block; width: 6px; height: 6px; border-radius: 50%; background: var(--accent); box-shadow: 0 0 8px var(--accent); animation: pulse 2s ease-in-out infinite; } @keyframes pulse { 0%,100%{opacity:1;} 50%{opacity:0.3;} } /\* FOOTER \*/ .footer { text-align: center; padding: 48px 0 0; border-top: 1px solid var(--border); } .footer-main { font-family: var(--font-display); font-size: 1.2em; font-weight: 700; color: rgba(255,255,255,0.1); margin-bottom: 8px; } .footer-main strong { color: var(--accent); } .footer-sub { font-size: 0.6em; color: var(--text-muted); letter-spacing: 3px; } .footer-quote { font-size: 0.68em; color: var(--text-dim); margin-top: 20px; font-style: italic; }

PELTGC

Foundation

[Philosophy](#philosophy) [Main Pool](#pool) [Deduplication](#dedup) [Digit Trimming](#threshold) [Merged Pointers](#pointers)

The Pool Learns

[Physics Tiers](#tiers) [Cold Start](#coldstart) [Pool Hierarchy](#hierarchy)

Execution

[Script Queue](#queue) [Thread Model](#threads) [Parallel Splitting](#parallel) [Fractional Routing](#fractional)

Rendering

[NDF](#ndf) [Hexagon Pixels](#hexels) [GPU Architecture](#gpu)

Systems

[Video Decoding](#video) [Audio Pooling](#audio) [Networking](#network) [Security](#security) [Storage Compression](#storage)

Language

[Compiler](#compiler) [Syntax](#syntax) [Error System](#errors) [NMJH](#nmjh) [RHS](#rhs) [Naming Standard](#naming)

Architecture Defended

[The Interrogation](#qa) [Ten More Questions](#solved) [Hard Engineering Critique](#hardcritique)

Complete Documentation — Runtime Philosophy

PELTGC
======

Pool Everything · Leave The Garbage Collector

**Think once.** Remember forever. **Reference when needed.** Never think twice.

01

Foundation

The Philosophy
--------------

PELTGC began with a single question: **why does a garbage collector exist?** The answer — because programs create and destroy the same things repeatedly — reveals the real problem. The GC is not the solution. It is a janitor cleaning up a mess that should never have been made.

The alternative is simple: **stop throwing things away.** Pool everything. Assign every calculation, instruction, result, and state an index. When the same thing is needed again — return the index. Never recompute. Never reallocate. Never collect.

PELTGC is not a memory optimization. It is a runtime philosophy that applies uniformly to computation, rendering, networking, threading, physics, video decoding, and execution itself. The pool is not a feature. It is the foundation.

Pooling is the GC. PELT-GC. A garbage collection technique where the technique is — never garbage collect.

02

Foundation

The Main Pool
-------------

One contiguous block of memory. All calculations from all domains live here, indexed by number. Math, physics, video, encoding, pointers, vertices — all share the same pool. The index is the identity.

GLOBAL POOL — one contiguous block

MATH

\[1\] ADDJIT

\[2\] MULJIT

\[3\] SUBlazy

PHYSICS

\[4\] BOUNCEJIT

\[5\] GRAVJIT

\[6\] COLLIDElazy

VIDEO

\[7\] DCT\_AJIT

\[8\] IDCT\_BJIT

\[9\] INTRAlazy

ENCODING

\[10\] MOVJIT

\[11\] PUSHJIT

\[12\] POPlazy

POINTERS

\[13\] 0x3F00merged

\[14\] 0x4A10merged

\[15\] 0x5C20lazy

VERTICES

\[16\] tree\_AJIT

\[17\] brick\_BJIT

\[18\] grass\_Clazy

### What JIT and Lazy Mean

**JIT** (Just In Time) means the entry was computed the moment it was first needed and immediately stored. The first time BOUNCE was required, it ran, got its index, and will never run again. Every future call routes to \[4\] instantly.

**Lazy** means the entry exists in the pool structure but has not been computed yet — it is reserved and indexed, but its value is still pending. The Script Queue has already seen it coming and assigned it a slot. When the calculation actually arrives, the slot is already waiting. No allocation needed. Just fill and go.

**Merged** means multiple pointers were collapsed into one entry. See Chapter 05.

### How Indices Get Assigned

Indices are assigned in order of first encounter — sequential, per session. The first calculation the pool sees becomes \[1\]. The second becomes \[2\]. The Script Queue pre-reserves indices for calculations it has seen coming before they arrive, so by the time a lazy entry is computed, its index was already decided. The pool never renumbers. An index is permanent for the lifetime of the session.

### Memory Regions and Deactivation

The pool does not grow forever. Under memory pressure, cold regions **deactivate** — they stop consuming active memory but retain their index. When referenced again they reactivate instantly. The work is never lost. It rests.

This is not eviction. Eviction destroys and requires recomputation. Deactivation preserves and requires only a wake signal. The distinction matters: **the pool never forgets, it only sleeps.**

03

Foundation

Deduplication
-------------

The same calculation performed twice is waste. PELTGC makes the second occurrence **structurally impossible** — not caught after the fact, but prevented at the architecture level. Once pooled, a calculation becomes a free index lookup forever.

Normal — recalculates every frame

ADD r0 r1   frame 1

ADD r0 r1   frame 2

ADD r0 r1   frame 3

ADD r0 r1   frame 4

4 calculations. always. no exceptions.

PELTGC — pool it once

\[1\]     JIT compiled — first time

\[1\]     free

\[1\]     free

\[1\]     free

1 calculation. forever free after.

### Adaptive Precision for Floating Point

Floating point values are almost never exactly equal twice — 2.3471 and 2.3472 look different to a strict comparator but are identical to human perception. PELTGC solves this by performing the full accurate calculation first, then **truncating only the search key** used to find a pool match.

The result stored in the pool is always precise. The key used to find it is as coarse as needed. If no match at 4 decimal places — drop to 3. Still no match — drop to 2. The pool always finds a home. The physics is never compromised.

The pool stores **perceived reality**, not raw reality. Differences below the threshold of human perception are noise, not information. The pool ignores noise by design.

04

Foundation

Digit Trimming — The Self-Calibrating Threshold
-----------------------------------------------

The pool stores perceived reality, not raw reality. But how does it decide when two values are close enough to match? Not through a manually configured threshold. Through **digit trimming** — the pool keeps removing trailing digits from both values until they converge on a match that already exists.

If someone asks what 2.0000001 and 2.0000002 are, they are both just 2. The pool figures that out by itself.

Traditional — manual threshold

define threshold = 0.001

if abs(a - b) < threshold: match

Wrong context = wrong threshold

Requires developer configuration

PELTGC — digit trimming

25626221590 vs 25626222590

trim → 256262215 | 256262225 — no match

trim → 25626221 | 25626222 — no match

trim → 2562622 | 2562622 — MATCH

The algorithm needs no context, no configuration, no domain knowledge. It trims until the pool itself confirms a match. The pool defines the threshold **by what it already contains**. Self-calibrating. Zero developer input required.

This also means the threshold is different per domain automatically. Physics positions, audio frequencies, pixel coordinates — each finds its own natural precision level through the same algorithm. One mechanism. Universal application.

05

Foundation

Merged Pointers — Chain Compression
-----------------------------------

Pointer merging is not just collapsing duplicates. It is **compressing entire instruction chains** down to only the parts the pool does not already know.

A disassembly sequence has addresses: 1, 2, 3, 4, 5. If address 3's result is already in the pool, addresses 1 and 2 are merged away entirely. Execution jumps straight to address 3's pooled result and continues from there. The chain is not deduplicated — it is **shortened.**

Normal — full chain always executes

addr 1 → compute (~300 cycles)

addr 2 → compute (~300 cycles)

addr 3 → compute (~300 cycles, already known)

addr 4 → compute (~300 cycles)

addr 5 → result — total: ~1500 cycles

PELTGC — chain compressed at known point

addr 1 → pool hit \[route, ~4 cycles\]

addr 2 → pool hit \[route, ~4 cycles\]

addr 3 → pool hit \[route, ~4 cycles\] ← merge point

addr 4 → compute (only genuinely new part)

addr 5 → result — total: ~312 cycles

### Full or Partial

If the entire chain's final result is already pooled — **full merge.** The whole sequence collapses to a single index lookup. If only a sub-result partway through is known — **partial merge.** The chain is cut at the known point, the known result is routed instantly, and only the remaining unknown steps execute.

Every step in the chain still executes — but at cache speed instead of compute speed. A 10-step chain where steps 1-4 are pooled completes those four steps in ~16 cycles instead of ~1200. Only step 5 onwards costs full compute. The chain is not shortened by skipping — it is compressed by making known steps instant. **The pool does not erase the questions. It answers them so fast they feel like they never happened.**

Normal — 4 duplicate pointers

ptr\_A→0x3F00

ptr\_B→0x3F00

ptr\_C→0x3F00

ptr\_D→0x3F00

PELTGC — 1 entry, chain compressed

A, B, C, D→\[13\]

Pointer table stays tiny. Fits in cache. All 4 cost same as 1. Everything before the known result is gone.

06

The Pool Learns

Physics Tiers — Self Optimizing
-------------------------------

Not all calculations are equally likely. PELTGC organizes physics into tiers based on frequency of use. The system does not require manual configuration — it learns its own tier structure through observation and promotes calculations automatically.

COMMON

Pre-baked at startup. Bounce, gravity, standard collisions. Always ready. Zero compute. Ever. These are known before the first frame runs.

instant

RARE

Speculatively precalculated within a limited lookahead range. Computed once when first encountered. Stored immediately after.

once

PROMOTED

A rare outcome that gets reused mid-execution. The system notices. It promotes the entry into the permanent pool automatically. No developer intervention. The runtime learns itself.

forever

### Promotion Threshold

A RARE entry is promoted to PROMOTED when it crosses a **hit threshold** — the number of times it has been routed from the pool rather than computed fresh. The threshold is not a fixed number. It is relative to session length. A short session promotes entries faster. A long session waits for more evidence before committing an entry to permanent status. The system calibrates what "frequently used" means based on how long the game has been running.

### Demotion

Promotion is not permanent. A PROMOTED entry that stops being used — because the player moved to a different area, or a game phase ended — will accumulate cold time. If it goes unrouted long enough relative to its original hit rate, it demotes back to RARE. If it continues to go unused, it eventually goes dormant. The tier system is always live. It never freezes into a configuration that no longer reflects reality.

The tier system means the pool is not just a flat list of equal entries. It is a living priority structure that reflects exactly what this game, on this machine, for this player, needs most right now. It is different for every session. It is always correct.

07

The Pool Learns

Cold Start — The Feature
------------------------

First run, the pool is empty. Every calculation is computed normally. Nothing is cached. Some would call this a weakness. It is not — and it is warmer than it sounds.

Cold start is like entering the classroom and seeing what's going on. You don't need a briefing. You walk in, observe, understand — and from that point you know everything.

Even on first run, the Script Queue is active. It is reading scripts, seeing certain outcomes, and pre-loading results **within the same session** as they become known. The pool fills itself as the game runs. By the middle of the first session it is already routing. By the end it is deeply warm.

The cold start is not a blank slate. It is a **live calibration.** The queue watches every script execute, every thread run, every outcome resolve — and the pool absorbs all of it in real time. First session the pool learns. Every session after that it already knows.

Traditional engine — pre-optimized

Optimized for average hardware

Optimized for average player behavior

Fits nobody perfectly

Same performance on session 1 and session 100

PELTGC — self-calibrating

Session 1: queue active, pool filling live

Session 2: warm — most things route

Session 10: tuned to this machine, this game, this player

Gets faster the longer you play. Always.

Other engines pre-optimize for an average case that fits nobody perfectly. PELTGC optimizes for the exact case in front of it. The cold start is not a cost. It is the calibration that makes all subsequent runs faster than any pre-configured alternative could ever be.

08

The Pool Learns

Pool Hierarchy
--------------

PELTGC pools are not isolated. They form a hierarchy. Before checking its own pool, a game checks the OS-level pool. Common calculations — gravity, standard math, universal physics — are computed once across the entire machine, not once per game.

OS POOL

Universal calculations. Gravity, basic math, standard physics. Shared across all running applications. Read-only to games — nothing can corrupt it. More PELTGC applications running = everyone benefits.

read-only

GAME POOL

Game-specific calculations. Physics unique to this title, asset-specific vertices, game logic. Writable by the game, invisible to other games. Falls back to OS pool before computing anything new.

isolated write

SESSION POOL

Player-specific patterns from this run. Learned automatically. Cleared between sessions or persisted to disk. The most personal layer — tuned to exactly how this player plays on this machine.

personal

### Machine Uniqueness

Every pool is a fingerprint of the machine that built it. Floating point behavior, hardware timing, and truncation characteristics differ at the silicon level. A pool that is optimal on one CPU is meaningless on another. **The machine is the pool.** They are inseparable. Pool transfer is not a security hole — it is physically nonsensical.

### Session Persistence

The session pool can be persisted to disk between runs. On next launch, the player's personal pool loads before the first frame — the system already knows how this player plays before they press a button. The cold start effectively disappears after the first session. Everything the pool learned is waiting.

Persistence is opt-in per game. Some games benefit from a fresh session pool every run — competitive games where player behavior is intentionally unpredictable. Others benefit enormously from persistence — open world games where the same areas and physics patterns repeat across hundreds of hours.

### Fallback Behavior

On a machine without OS pool support — older hardware, different OS — the game pool simply takes over the OS pool's responsibilities for universal constants. Gravity gets pooled in the game pool instead. Nothing breaks. The hierarchy collapses gracefully to a flat game pool. Performance is slightly lower than on full PELTGC hardware, but still dramatically better than a traditional engine because the game pool is still active.

09

Execution

The Script Queue — The Pool's Eyes
----------------------------------

The Script Queue is not a task scheduler. It is the pool's ability to **read the future with certainty** — not by guessing, but by reading the scripts that have already decided what will happen.

It is like reading a book and knowing what comes next. Not predicting. Reading. The logic is already written. The queue just sees it first.

### Script Level — Certain Outcomes

When a script executes, the queue reads its logic in full. If the script says:

SCRIPT LOGIC

if enemy.attacking AND player.shield == null:  
  player.die()

The queue sees `enemy.attacking = true` and `player.shield = null`. It does not predict the player will die. It **knows with 100% certainty** because the code already decided it. Before the player hits the ground, the pool has already loaded the death animation, respawn logic, checkpoint data, and score update.

Prediction — sometimes wrong

Player health is low...

Maybe they'll use a potion?

Pre-load potion effect... maybe.

Wrong 30% of the time. Wasted compute.

Script Queue — always certain

Queue reads: shield == null, enemy attacking

Script says: player.die() — certain.

Pool pre-loads death outcome now.

100% accurate. Zero wasted compute.

### Thread Level — Below the Scripts

The queue operates below scripts too. Every thread's job is queued before it starts. The pool reads what each thread is about to do and pre-loads everything it will need. The thread shows up to work and **everything is already waiting.**

The thread never asks for a calculation. The pool already knew the thread was coming.

SCRIPT

Queue reads running scripts and sees guaranteed outcomes from logic conditions. Enemy attacking + no shield = certain death. Pool pre-loads all death-related calculations instantly.

certain

THREAD

Every thread's job enters the queue before execution begins. Pool pre-loads everything that thread will need. Thread arrives and finds its work already done. Zero waiting.

pre-loaded

UPDATES

When a game patches, old pool entries never appear in the new queue. They go cold and deactivate through disuse. No active invalidation sweep needed. The update orphans stale entries organically.

self-cleaning

### Two Layers. One Pool.

Script level reads the plot. Thread level reads the author's notes before the book is printed. Both feed the same pool. Both give certainty, not guesses. The queue runs constantly ahead of reality — and reality just catches up to what the pool already prepared.

**The queue is the pool's eyes. The pool is the queue's hands.** Together they eliminate the concept of being unprepared. The pool is never caught off guard — either it already has the result, or the queue already saw it coming.

10

Execution

Thread Model — The 12 Nerds
---------------------------

Twelve students. One whiteboard. No one solves what's already been solved. No one asks a question that's already been answered. Everyone sees what everyone else has written. The pool is the whiteboard. Threads are the students.

Because the pool is **read-only for shared state**, there are no race conditions. Reads never conflict. The synchronization overhead that kills most parallel systems — locks, mutexes, semaphores, wait states — simply does not exist.

### Collisions Don't Happen

The old framing was: thread collision becomes a pipeline. The correct framing is: **thread collisions never happen in the first place.** Because every thread's job enters the Script Queue before execution begins, the queue sees what every thread is about to do and separates their work before they start. By the time a thread begins executing, its entire job has already been pre-loaded into the pool. There is nothing to collide over.

Thread behavior — with Script Queue

Normal T1

CALC\_A — executing

result ready

Normal T2

CALC\_A — waiting (duplicate)

wasted cycles

PELTGC T1

CALC\_A — executing

result ready

PELTGC T2

CALC\_B — already pre-loaded by queue

instant route

T2 was never going to collide. The queue read T2's job description before T2 started and pre-loaded everything it needed. T2 arrives and finds its work already done.

### The Whiteboard Principle

All threads share one pool. They broadcast their results and read each other's results in real time. No thread ever solves something another thread already solved. No thread ever waits for information that's already in the pool.

Communication overhead disappears because the pool is always current. You do not ask your teammate what they computed. You look at the whiteboard. And by the time you look — it was already written there before you arrived.

11

Execution

Parallel Splitting
------------------

One 32GB pool is a bottleneck. Sixteen 2GB pools are sixteen independent domains. Each core owns its slice. No locks. No contention. The same solution that handles pool size also handles parallelism — they are the same problem.

2GBPool 0

Core 0

2GBPool 1

Core 1

2GBPool 2

Core 2

2GBPool 3

Core 3

2GBPool 4

Core 4

2GBPool 5

Core 5

2GBPool 6

Core 6

2GBPool 7

Core 7

### Cross-Pool Lookup

Each core owns its slice — but what if Core 3 needs a result that Core 0 already computed? It does not recompute. It queries Core 0's pool directly via a **shared index table** — a lightweight read-only map that tells every core where every index lives. The result lives in Core 0's memory. Core 3 reads it. No duplication. No transfer. Just a pointer across the boundary.

This is read-only by design. No core ever writes to another core's pool. The shared index table is append-only — cores add entries to it as they compute new results, but never modify or delete existing ones. Reads are free. Contention is impossible.

Traditional multi-core

Core 3 needs result from Core 0

Core 3 either recomputes it

or waits for Core 0 to finish and copy

cache coherency overhead — always present

PELTGC parallel pools

Core 3 checks shared index table

Index says: result lives in Core 0 Pool, slot 42

Core 3 reads slot 42 directly — free

No copy. No wait. No recompute.

More cores = more pools. The architecture scales horizontally with no redesign. Adding cores adds capacity without adding complexity. The shared index table grows with the system automatically.

12

Execution

Fractional Routing — Half-Pooled Solutions
------------------------------------------

Legacy systems suffer from the "All or Nothing" caching problem. If a CPU is asked to calculate a massive, complex equation and it doesn't have the _exact_ final answer stored, it throws its hands up and recalculates the entire thing from scratch. It treats the equation like a locked black box.

PELTGC does not see a black box. It sees **Lego blocks**.

When you solve a math problem, you don't always start from zero. You recognize the tricks. You look at the intermediate steps, realize you've done half of it before, and jump to the end. The hardware should do the exact same thing.

### Compound Intent Resolution

If the engine encounters a completely novel calculation—for example, a player jumping out of a moving vehicle into a windstorm—it breaks the calculation into sub-intents. The final combination may be brand new, but the individual forces are not.

Legacy CPU — All or Nothing

1\. Calculate Gravity: 9.81 \* Mass

2\. Calculate Wind: 1.2 \* Velocity

3\. Add them together for Total Force

3 heavy ALU operations. Complete waste of time.

PELTGC — Fractional Routing

1\. Gravity = \[Index 14\] (Routed instantly)

2\. Wind = \[Index 42\] (Routed instantly)

3\. Add \[14\] + \[42\] -> Pool as \[Index 43\]

1 light addition. Cold Starts are almost never 100% cold.

With Fractional Routing, a "new" calculation is rarely new. It is simply a novel arrangement of already-pooled steps. The compiler recognizes the "half-pooled solutions" and dynamically jumps over the math it already knows. The execution pipeline never starts from zero.

**This flattens the Cold Start curve.** The more you play, the more "puzzle pieces" the pool collects. Even if the game generates a procedural, never-before-seen event, PELTGC solves it almost instantly by snapping together the pooled fragments of past events.

13

Rendering

NDF — No Duplicate Frames
-------------------------

If the pool state did not change between frames, the rendered output would be identical. Rendering it again is pure waste. But NDF does not just check pool state after the fact — the Script Queue tells it what is coming **before the frame is even due.**

If no scripts touching the scene state are in the queue, NDF knows with certainty the next frame will be identical. The GPU is told to skip before the frame cycle even begins. Not reactive — **preventive.**

frame 1

→

queue has scene-changing scripts — render

frame 2

→

queue empty of scene scripts — skip before GPU is asked

frame 3

→

queue still empty — skip

frame 4

→

queue sees camera movement script — render only changed

frame 5

→

queue empty again — skip

**Static scene = infinite FPS.** Not because the GPU is running faster — because it is not running at all. GPU load becomes proportional to actual scene complexity, not to frame rate. A menu screen, a cutscene, a slow moment in gameplay — effectively zero GPU cost.

NDF was not a design target. It emerged naturally from the pool architecture. Once pool state is the source of truth for all rendering, and the queue sees what is coming before it arrives, skipping identical frames becomes the automatic default — not an optimization pass.

### Partial Frame Updates

NDF does not only skip entire frames. When something changes, it skips everything that **did not** change. The pool knows exactly which indices changed between frames — only those entries trigger a redraw. A player moving in a static environment re-renders only the player and their shadow. The background, the sky, the static geometry — untouched. The GPU renders only what reality changed, nothing more.

Traditional — full frame always

Player moved 2 pixels

Re-render entire 4K frame

Sky, ground, buildings — all redrawn

GPU at 100% for 2 pixels of change

PELTGC NDF — only what changed

Player moved 2 pixels

Pool shows: 3 indices changed

Re-render: player sprite + shadow + footstep

GPU at ~1% for exactly what changed

14

Rendering

Hexagon Pixels — The Perfect Grid
---------------------------------

Square pixels are a legacy artifact from the 1950s. They are physically flawed: the distance to a square's corner is longer than the distance to its side. This geometric failure creates jagged edges. To hide this, modern hardware burns massive amounts of compute power on Anti-Aliasing (blurring edges to fake a smooth line).

Hexagons are equidistant. Every neighbor is exactly the same distance from the center. They form natural curves. The human retina is made of hexagonal photoreceptors, not a Cartesian grid of squares. So why do we use squares?

The industry uses squares because the math for hexagons is too heavy to calculate 60 times a second. PELTGC only calculates it once.

Legacy GPU + Square Pixels

Draw square grid.

Detect jagged diagonal line.

Compute sub-pixel blending (MSAA/TAA).

Recalculate blur every single frame.

Heavy constant load. Blurry motion.

PELTGC + Hexagon Pixels

Map 3D edge to hex grid (Frame 1).

Pool the complex coordinate math.

Frame 2+: Route instantly. Zero math.

Natural curves. No Anti-Aliasing needed.

Perfect clarity. Zero ongoing compute.

### NDF Synergy

Modern Anti-Aliasing techniques (like TAA) ruin static frames. They jitter the camera microscopically every frame to gather sub-pixel data, meaning the frame is _always_ changing, even when nothing is moving. This breaks traditional caching.

Because Hexagon Pixels eliminate the need for Anti-Aliasing entirely, the image doesn't need to jitter. The frame remains mathematically identical. This allows PELTGC's **NDF (No Duplicate Frames)** to step in flawlessly. A static hex-rendered scene consumes exactly 0.0% GPU power.

Hexagonal displays have always been the dream of display engineers, bottlenecked by the processor's inability to do the complex math fast enough. PELTGC breaks the bottleneck. The math is routed, not computed. The perfect display finally has the perfect architecture to drive it.

15

Rendering

GPU Architecture — The Real Target
----------------------------------

The GPU arms race is an expensive patch on a philosophy problem. Every generation adds more cores to process the same duplicate calculations faster. More VRAM to hold the same redundant data in more places. More power to push through unchanged frames at higher resolution.

The bottleneck was never hardware. It was always: **why are we doing this work twice.**

PELTGC applied at the GPU architecture level means the silicon itself has the pool baked in. Not software instructing the GPU to cache things — the hardware natively understands the concept of a pooled index. A shader that ran last frame with identical inputs does not execute. It returns the pooled result. Instantly.

### What Changes at Silicon Level

A traditional GPU core has: fetch unit, decode unit, ALU, write-back. Every operation goes through all four stages every time.

A PELTGC GPU core adds a **pool lookup stage before fetch**. Before an instruction is even fetched, the hardware checks the pool index table. Hit — skip fetch, decode, ALU entirely. Return the stored result directly. The ALU sits idle. Power drops to near zero for that core on that cycle. Miss — proceed through normal pipeline and pool the result on the way out.

Traditional GPU core — always executes

Fetch → Decode → ALU → Write

Same shader inputs as last frame?

Doesn't matter. Runs anyway.

Full power every cycle regardless

PELTGC GPU core — pool first

Pool check → hit → return result

Fetch, Decode, ALU never wake up

Core draws near-zero power

Miss → normal pipeline + pool on exit

Duplicate draw calls — hardware-level deduplication. Identical vertices — one calculation shared across every core that needs it. Unchanged pixels — the silicon skips them without NDF telling it to. The GPU stops being a calculator that forgets everything between frames.

The result: less power, less heat, less silicon, more performance. PELTGC GPU does not make expensive hardware faster. It makes cheap hardware capable. A kid who is lagging — stops lagging. The efficiency gain serves everyone at every price point, not just the top of the market.

16

Systems

Video Decoding — Lookahead and Pool
-----------------------------------

H.264 pools pixel data — blocks of image that appear multiple times across frames. PELTGC goes two layers deeper: it pools the **decode instructions themselves**, and the Script Queue reads the video stream **ahead of playback** to pre-load them before the decoder ever asks.

This means even the **first occurrence** of a block can arrive already decoded — because the queue saw it coming in the stream and loaded it in advance. Pooling handles repeats. The queue handles first encounters. Together they eliminate almost all decoding work.

Traditional — reactive

Frame arrives → decode DCT\_A → store result

Frame arrives → decode DCT\_A again (repeat)

First occurrence always costs full decode

Repeats caught after the fact

PELTGC — active anticipation

Queue reads stream → sees DCT\_A coming at f3, f7, f47

Pool pre-loads DCT\_A decode before f3 arrives

f3 arrives → already decoded. Free.

f7, f47 → pool hit. Free.

f1

DCT\_A  
pre-loaded

f2

DCT\_B  
pre-loaded

f3

DCT\_A  
\[7\] free

f4

DCT\_A  
\[7\] free

f5

DCT\_C  
pre-loaded

f6

DCT\_B  
\[8\] free

f7

DCT\_A  
\[7\] free

f8

DCT\_C  
\[9\] free

f9

DCT\_A  
\[7\] free

f10

DCT\_B  
\[8\] free

Every frame is free. Not because the decoder got faster — because the queue read the script of the entire video ahead of time and the pool absorbed it before playback reached it. The decoder arrives to find its work already done.

17

Systems

Audio Pooling — Frequencies Are Just Numbers
--------------------------------------------

Sound is frequency. Frequency is a number. Numbers go in the pool. The entire audio engine follows naturally from the same philosophy as everything else — **pool everything, reference when needed, never reproduce.**

If the same audio frequency appears twice anywhere in the game — same note in a song, same tone in a sound effect, same harmonic in an ambient track — it is one pool entry referenced twice. Not two sounds. One sound, two references.

### Music is Repetition by Design

A single note played 50 times in a song is one pool entry referenced 50 times. A chorus that repeats 8 times — same pool entries, 8 references. The harmonic structure of music is massively repetitive by nature. The pool exposes that and eliminates all of the redundancy automatically.

Traditional audio — stored in full

C4 note × 50 occurrences = 50 stored samples

Chorus × 8 repetitions = 8 stored blocks

Same frequency in SFX = separate file entirely

20-30GB of audio per modern game

PELTGC — pooled frequencies

C4 note = 1 pool entry, 50 references

Chorus = same entries, 8 references

Same frequency in SFX = same pool entry

Fraction of the original audio footprint

### Cross-Context Frequency Sharing

The pool does not care where a frequency was first encountered. A 440Hz tone in the menu music and a 440Hz component in a sword swing are the **same pool entry.** Background music, sound effects, UI sounds, ambient audio, voice lines — they all share one frequency pool. The context is irrelevant. The number is the identity.

### Instruments Share Frequencies

A C4 on a piano and a C4 on a violin have the same base frequency — 261.63Hz. Only the harmonic overtones differ. The pool stores the base frequency once. The overtone pattern is a separate entry. Two completely different instruments — mostly shared pool data, with only the instrument-specific character stored separately.

### Digit Trimming on Audio

440.001Hz and 440.002Hz are indistinguishable to the human ear. Digit trimming collapses them to the same pool entry automatically. The pool stores what can actually be perceived. Everything below the threshold of human hearing is noise — and noise is never stored twice.

A modern game's audio — often 20-30GB — compresses down to a pool of unique frequencies, unique overtone combinations, and unique timing patterns. Most of which repeat constantly. The pool does not store a game's music. It stores the **alphabet the music is written in.**

18

Systems

Networking — Packets Are Just Numbers
-------------------------------------

If both client and server share a deterministic pool, there is no need to transmit state. Transmit the **index**. One byte instead of 120. The pool is the protocol.

Normal packet — 120 bytes

pos\_x: 342.571  
pos\_y: 128.334  
vel\_x: 2.341  
vel\_y: -1.205  
rot: 0.443  
state: jumping

Full state every tick. Bandwidth scales with complexity.

PELTGC packet — 1 byte

4

Both sides share pool. Deterministic. Index is the state.

### Queue Synchronization

The server runs its own Script Queue. The client runs its own Script Queue. They are **partially synced** — not identical, but coordinated.

Player input is queued on the client and transmitted to the server. The server's queue receives the input, reads the scripts it will trigger, and pre-loads outcomes on both sides simultaneously. By the time the input resolves, both client and server already have the result pooled. The server is the canonical truth. The client is always ready to match it.

INPUT

Player input enters the client queue. Transmitted to server. Server queue reads the scripts it triggers. Both sides pre-load the outcome. Synchronized certainty — not synchronized guessing.

synced

WORLD

World state — physics, enemies, environment — is driven by the server queue. Client receives the pool index, not the state. Client already has the state because the pool is shared and deterministic.

server-owned

RENDER

The server never renders. It holds pool state, validates indices, and serves canonical truth. Rendering is entirely the client's concern. An entire class of server-side overhead simply does not exist.

client-only

### Subpool Cloning for Verification

To verify a result across client and server, PELTGC clones the relevant subpool to both sides, runs the calculation independently, and compares outputs. Agreement = valid. Disagreement = desync or tampering detected immediately.

The clone itself is a calculation — so it gets pooled. The first clone of a given subpool is computed once. Every subsequent identical clone is free. The anti-cheat system costs nothing at scale.

### Anti-Cheat by Architecture

Pool indices are randomized per session per machine. No consistent addresses. The pool map lives in the compiler and ships without labels. A disassembler sees only: 1 2 3 4 5 6 7 8. There is nothing to target because the target changes every run.

19

Systems

Pool Integrity Protection
-------------------------

The pool is the entire game's source of truth. Corrupting it would corrupt everything — physics, rendering, networking, logic. It is the highest-value target imaginable. PELTGC protects it at the architecture level, not the software level.

### Why Traditional Anti-Cheat Fails

Traditional anti-cheat scans for known signatures — specific memory addresses, known injection patterns, recognized cheat executables. Cheaters update. Signatures become stale. It is a perpetual arms race that the defender always loses eventually.

PELTGC has no signatures to hunt. The pool indices are randomized per session per machine at compile time. A disassembler sees only: 1 2 3 4 5 6. The labels that would tell an attacker what each index means ship **only in the compiler**, which is never distributed. There is nothing to reverse engineer because the meaningful part was never sent.

attempt 1

pool touch detected — reads outside normal execution pattern

logged silently. attacker does not know they were seen.

attempt 2

pattern confirmed — same touch signature repeated

hey lil script kiddie. ToS Protocol in 3...2...1...

attempt 3

reinstalled and tried again — machine fingerprint still matches

BSOD — WRONG\_POOL\_ADDRESS. Hardware-level rejection.

attempt 4

still trying on same hardware

D... E... A... T... H... (permanent hardware ban)

attempt 5

presumably

fertilizer farm

### The Mechanism

Attempt 1 is silent because the system wants the attacker to keep going. Confidence makes attackers careless. Attempt 2 is the confirmation — the system now has a behavioral fingerprint, not just a single event. Attempt 3 escalates to hardware level because reinstalling changes nothing — the machine is the pool, and the machine is known. Attempt 4 is permanent because at this point the hardware itself is considered compromised.

Pool indices randomized per session per machine. No consistent addresses. Pool map stays in compiler. Ships without labels. Disassembler sees: 1 2 3 4 5 6 7 8. Even if an attacker perfectly reads the pool, they read meaningless numbers with no way to know what any of them represent.

20

Systems

Storage Compression — What 100GB Actually Is
--------------------------------------------

A 100GB game is not 100GB of unique information. It is a small amount of unique information repeated, tiled, referenced, and duplicated until it fills 100GB. PELTGC stores only what is genuinely unique. Everything else becomes an index.

The actual unique information in a 100GB game is a fraction of that. The rest is repetition dressed up as size.

### Where the Redundancy Lives

TEXTURES

Open world games tile terrain textures across massive areas. The same grass, rock, and dirt texture referenced thousands of times. One pool entry per unique texture. Every tile is a free reference.

highest savings

AUDIO

Frequencies shared across music, SFX, ambient, and UI. Instruments sharing base frequencies. Notes repeating throughout an entire soundtrack. 20-30GB collapses to a frequency pool.

highest savings

PHYSICS

Gravity runs every frame. Collision physics repeats constantly. Standard forces pre-baked into the OS pool at boot and shared across every game running on the machine simultaneously.

near-zero cost

GEOMETRY

Repeated enemy types, shared building components, duplicate props. Merged pointer chains compress instruction sequences down to their genuinely unique parts. Similar objects share most of their pool data.

high savings

ANIMATION

Animations share sub-movements. A walk cycle uses the same joint rotations as a run cycle in part. Fractional routing pools the shared sub-components. Only the genuinely different motion is ever stored uniquely.

moderate savings

### The Result

A 100GB game on a traditional engine becomes approximately **5GB or less** under PELTGC. Open world games with tiling terrain and repeated content compress the hardest. Heavily hand-crafted games with fully unique assets compress the least — but even those see massive savings on physics, audio frequencies, and animation sub-components.

Traditional install

Textures: ~40GB (tiled, repeated)

Audio: ~25GB (same frequencies, many files)

Geometry: ~20GB (duplicate objects)

Other: ~15GB

Total: 100GB on disk

PELTGC install

Unique textures: ~2GB

Frequency pool: ~1GB

Unique geometry: ~1.5GB

Other unique data: ~0.5GB

Total: ~5GB on disk

This is not compression in the traditional sense — zipping a file and unzipping it later. The pool **never had the redundancy to begin with.** The game never stored what it didn't need. The 95GB that disappears was never real information — it was the same information repeated 20 times, finally counted once.

21

Language

The PELTGC Compiler
-------------------

PELTGC is not just a runtime philosophy. It is a compiler. The compiler controls bytecode directly, sitting below whatever language the game is written in. It intercepts compiled output and applies the pool logic at the instruction level. The source language is irrelevant.

The architecture: game written in anything → compiles to bytecode → PELTGC intercepts → pools, queues, redirects, deduplicates → hardware receives clean optimized instructions. The developer touches nothing. PELTGC handles everything underneath, invisibly.

### How Interception Works

Every compiler — GCC, LLVM, whatever the game uses — produces an intermediate output before generating final machine code. PELTGC inserts itself at that stage. It receives the intermediate representation, applies pool logic to every instruction, replaces duplicate operations with index lookups, inserts queue pre-load calls, and then passes the result forward to final compilation. The game's compiler never knows PELTGC was there. The hardware never sees the unoptimized version.

### Human-Readable Bytecode

Most bytecode is unreadable by design — it is for machines, not humans. PELTGC bytecode is different. Every operation is annotated with what the pool did. A developer reading it can see exactly what was routed, what was computed fresh, what the queue pre-loaded, and what was merged.

PELTGC BYTECODE — human readable

LOAD gravity       // \[5\] pool hit — routed, zero compute  
LOAD player\_mass   // \[22\] pool hit — routed  
MUL \[5\] \[22\]       // \[47\] new — computed, pooled  
LOAD jump\_height   // \[8\] pool hit — routed  
ADD \[47\] \[8\]       // \[48\] new — computed, pooled  
RENDER player     // queue: pre-loaded by script queue 2ms ago

Traditional bytecode

0x8B 0x45 0xF8

0x89 0x45 0xFC

0x8B 0x4D 0xF8

Requires debugger, symbols, and patience

PELTGC bytecode

LOAD gravity // \[5\] pool hit

MUL \[5\]\[22\] // \[47\] new, pooled

RENDER // pre-loaded by queue

Readable without tools. Always.

Debugging stops being a deep technical skill. A developer looks at the bytecode and immediately sees: this was a pool hit, this was new, this was pre-loaded. The cause of any performance issue is visible directly in the output.

22

Language

Syntax — Human First
--------------------

Most programming languages started close to machine code and slowly drifted toward humans. PELTGC starts at humans and builds down toward the machine. Opposite direction. Completely different result.

The syntax reads like intent. No symbols, no rituals, no arbitrary rules accumulated over decades. Three patterns cover everything: **action: target**, **modifier: condition**, **scope: block**. Learn three patterns. Read any PELTGC code ever written.

C++ — speak the machine's language

void Jump() {'{'}

  if (isGrounded) {'{'}

    velocity.y = jumpHeight;

    isGrounded = false;

    while (pos.y > 0) {'{'}

      vel.y -= grav \* dt;

    {'}'}

  {'}'}

{'}'}

PELTGC — tell it what you want

new jump function:

  check: is\_grounded

  apply: jump\_height upward

  use: gravity downward timebetween

  repeat until: ground

### Defines — No Magic Values

Every word that appears in a script has a definition. The compiler never guesses. If it is used, it is defined. This is the rule.

DEFINES

define: jump\_height = 15  
define: gravity = 9.8  
define: ground = 0  
define: still = 0  
define: nothing = null  
define: timebetween = delta  
define: jump\_key = space  
define: is\_grounded = 1  
define: not\_grounded = 0  
define: quit = 0

### Imports — Concepts, Not Modules

`use: coordinates` unpacks x and y. `use: coordinates3D` unpacks x, y, z. `use: color` unpacks r, g, b. `use: time` unpacks timebetween, total, elapsed. The developer thinks in concepts. The compiler resolves to components. Neither pretends to be the other.

### Pool Declarations — What the Compiler Should Remember

`new sys pool:` declares a block of values that should be immediately and permanently pooled at the OS level — values the developer knows will be needed constantly throughout the entire game. `sys` means system-level, permanent, shared. The compiler pre-bakes these into the COMMON tier before the first frame runs.

`remember:` is the instruction that adds a value to the declared pool block. `remember: gravity` tells the compiler — this value will be needed constantly, pool it immediately, never compute it again. It is the developer making an explicit promise to the system: this is not a one-off calculation. This is a permanent fixture.

POOL DECLARATION

new sys pool:             // declare a permanent system pool block  
  remember: gravity        // pool gravity at COMMON tier — instant forever  
  remember: jump\_height    // pool jump\_height — never compute again  
  remember: ground         // pool ground reference — always available

`use: thread2` in a script is an explicit declaration that this script runs on Thread 2. It does not mean the developer is managing threads manually — it means they are telling the Script Queue which thread's job list this script belongs to. The queue uses this to pre-load correctly: it knows Thread 2 will need this script's results, so it pre-loads specifically for Thread 2's pool slice.

If no thread is specified, the compiler assigns one automatically based on what the script needs and which threads are least loaded. Manual thread assignment is an optimization hint, not a requirement.

FULL JUMP SCRIPT

use: coordinates  
use: gravity  
use: thread2  
  
define: jump\_height = 15  
define: gravity = 9.8  
define: ground = 0  
define: still = 0  
define: nothing = null  
define: quit = 0  
define: jump\_key = space  
define: is\_grounded = 1  
define: not\_grounded = 0  
  
new sys pool:  
  remember: gravity  
  remember: jump\_height  
  remember: ground  
  
new jump function:  
  check: is\_grounded  
  stop at: not\_grounded  
  apply: jump\_height upward  
  set: is\_grounded = not\_grounded  
  use: gravity downward timebetween  
  repeat until: ground  
  set: is\_grounded = 1  
  
new input function:  
  listen: jump\_key  
  stop at: nothing  
  trigger: jump  
  repeat until: quit  
  
new game function:  
  start: input  
  start: jump  
  repeat until: quit  
  
run: game

### Visual Slot Input

In the IDE, colons become paste slots. The keyword is fixed. The intent is fixed. You fill in what belongs. No syntax errors — the slot validates its own type before the compiler sees it. Errors become impossible at the input level, not caught after.

SLOT SYNTAX

ask \[what is your name\]  
remember: \[name\]  
write \[hello\] \[name\]  
repeat \[5\] times  
stop at \[wall\]

23

Language

Error System — Conversation, Not Punishment
-------------------------------------------

Most compilers treat errors as failures. PELTGC treats them as missing information. The compiler is not blocking you. It genuinely does not know — and it asks, politely, with personality.

C++ error

NullReferenceException: Object reference not set to an instance of an object at PlayerController.Jump() line 47

PELTGC

what is character? Can you tell?

C++ error

redefinition of 'gravity' — previous definition at line 3

PELTGC

hey sorry, but why did you just tried to define gravity twice?

PELTGC

Mistake!! You made a typo at function 2, where your define: gravity is located. Please fix it. I sadly don't understand what you mean

The compiler knows where you are, what you wrote before, and what you likely meant. Errors become a conversation. Debugging stops being a skill requiring years of experience. It is just a question-and-answer between you and a compiler that is genuinely trying to help.

Beginner developers spend enormous time decoding error messages that describe the symptom, not the cause, in language designed for the machine. PELTGC describes the cause, in language designed for the human, in the tone of a collaborator not a judge.

24

Language

NMJH — No Mistakes, Just Helping
--------------------------------

PELTGC makes engines faster. NMJH makes **developers better** — silently, without judgment. It watches the bytecode in real time, detects inefficient patterns, and acts. Small inefficiencies are fixed automatically. Larger structural problems are flagged with a conversation, not an error.

Same philosophy as the error system. The system is not blocking you. It is not judging you. It genuinely wants to help — and it only asks when it needs your input to do so.

### Two Tiers of Intervention

SILENT

Identical loop results, redundant function calls, dead code, duplicate calculations already in the pool. Fixed automatically. Developer never sees it. It just runs better.

automatic

FLAGGED

Structural issues — bad game loop design, inefficient asset loading, poor physics setup. Anything where the fix requires a design decision. NMJH asks. It never overrides intent.

collaborative

### Zero Cost

NMJH costs almost nothing to run. Because PELTGC already tracks every calculation's efficiency, hit rate, and usage pattern, NMJH does not need to do extra work to find inefficiencies — **the pool already knows**. NMJH simply acts on data that already exists. The optimizer is essentially free.

NMJH is not a separate system. It is PELTGC's pool data with a decision layer on top. Two systems. One feeds the other. No redundancy.

25

Language

RHS — Readable Hex System
-------------------------

Traditional hex addresses are opaque by design. `0x3F4A2B10` tells you nothing — it is a location with no meaning. RHS replaces this with addresses that describe **state, operation, and location** in a single human-readable token.

A debugger reading RHS understands what is happening at a glance. A debugger reading traditional hex needs a symbol table, documentation, and patience.

### Syntax

RHS FORMAT

y = yes — execute this instruction  
n = no — skip this instruction  
+ = add  
\- = remove  
A = address marker  
1..N = address index (sequential, order of creation)  
  
example: y+1n-2y+8A1  
→ yes add 1 | no remove 2 | yes add 8 | at address 1

Each `y` or `n` is a decision on its own instruction. The `n` entries are not wasted — they remain in the bytecode so a human reading it sees the full decision, not just the outcome. PELTGC pools the patterns regardless.

### Sequential Addressing

Addresses are assigned in order of creation. No reserved zones, no manual categorization. The first thing written is A1. The second is A2. The order is the organization. This maps directly onto the pool index — RHS addresses and pool indices are the same thing, just made readable.

Traditional Hex

0x3F4A2B10 — position

0x000064 — health

0x00000003 — inventory

Requires symbol table to decode

RHS

y+342n+0y+891A1 — position

y+100A2 — health

y+1n+0y+1n+0A3 — inventory

Readable without any documentation

RHS is not a separate system bolted onto PELTGC. It is PELTGC's pool indices made human readable. They were always there. RHS just gives them a format a human can understand without a manual.

26

Language

Hardware Naming Standard
------------------------

Current hardware naming tells you nothing. RTX 4090. RX 7900 XTX. Core i9-14900KS. You need a review site, a spec sheet, and a community wiki to understand what you are buying.

PELTGC hardware names are self-describing. Every character earns its place. Nothing is marketing noise.

### CPU Standard — RisingNc.5ninesNR1S

Rising

product line

Nc

No Calculations  
PELTGC inside

5nines

99.999%  
reliability

NR1

New Revision  
Generation 1

S

Safe  
no overclock

### GPU Standard — PEcct Pool5x.nines

PE

PELTGC

cct

circuit  
hardware

Pool

pool  
philosophy

5x

5× efficiency  
vs standard

.nines

reliability  
tier count

**The more nines, the better the hardware.** Manufacturers compete for nines — not benchmark scores nobody understands. A universal, human-readable reliability standard replaces opaque model numbers. The product roadmap becomes legible in the name.

The naming standard also embeds the technology claim. A CPU called RisingNc is announcing what it runs on. A GPU called PEcct is declaring its architecture. The name is the spec sheet summary.

27

Architecture Defended

The Interrogation — Addressing the Skeptics
-------------------------------------------

When you propose a system that eliminates the garbage collector and bypasses traditional CPU logic, computer science veterans will ask the same four questions. Here are the answers.

### Q: Searching RAM takes 100+ cycles. Basic math takes 1 cycle. If you search a pool instead of calculating, aren't you making it slower?

**A: It doesn't search. It routes.**

Traditional memoization creates a hash, searches a massive dictionary, and asks, _"Have I done this?"_ That is slow. PELTGC uses a **Pre-Compiled Ledger**. The compiler already knows the intent before the instruction fires. It acts as a hardware-level switch.

If someone asks you what 1+1 is, you don't hold up your fingers and count. You just say 2.

When the system sees a calculation it knows, it does not wake up the ALU. It does not open or close logic gates. It simply follows a hardcoded redirect pointer to the answer. **O(1) execution.** Zero search time. Zero compute time.

**The Restaurant Analogy:** A normal CPU is a chef who cooks every burger from scratch, even if 10 are ordered. A memoized CPU searches the massive kitchen to see if a burger is already made (which takes too long). PELTGC is just a numbered menu. The waiter asks for #42, and #42 is handed over instantly.

### Q: If Thread 2 needs the result of Thread 1, Thread 2 has to stop and wait. How does PELTGC avoid thread lock?

**A: Threads don't have egos. They serve the queue.**

In a legacy system, threads are rigidly assigned to tasks. If Thread B needs Task A to finish, it goes to sleep and burns cycles waiting (Thread Lock). In PELTGC, the Script Queue knows the entire dependency graph.

Legacy CPUs

Thread 1: Cutting Brick A

Thread 2: Needs Brick A. Waiting... (wasted cycles)

PELTGC Threads

Thread 1: Cutting Brick A

Thread 2: Becomes Calc\_A. Helps cut Brick A.

The moment a thread hits a dependency wall, it seamlessly shifts roles and helps process the exact bottleneck it was waiting on. No mutexes. No wait states. Just continuous forward momentum.

### Q: RAM is physical. If you never delete anything, won't the 32GB pool eventually hit 100% and crash?

**A: Resident Dormancy and Zero-Cost Overwriting.**

Other engines move "cold" memory to a slow SSD (Pagefile), causing massive lag. Or they freeze the game to sweep and delete it (Garbage Collection). PELTGC does neither.

When data gets cold, it goes **dormant**. It stays in physical RAM but draws zero active processing overhead. If the physical RAM actually hits 99.9% capacity, the hardware natively tracks cache hits. It silently allows the newest calculations to overwrite the absolute coldest, most forgotten indices. The pool doesn't crash; it organically replaces its oldest memories without ever stopping the execution pipeline.

### Q: How does NDF (No Duplicate Frames) know a frame is identical without asking the GPU to render it first?

**A: The frame is just an equation.**

PELTGC treats the entire scene state as a mathematical formula of pool indices. If the inputs have not changed, it is a mathematical certainty that the output will not change.

FRAME HASH

Frame 1: \[Cam\_Pos\_7\] + \[Light\_State\_12\] + \[Player\_Anim\_4\] = Output\_A  
Frame 2: \[Cam\_Pos\_7\] + \[Light\_State\_12\] + \[Player\_Anim\_4\] = Output\_A (Skip GPU)

The hardware checks the ledger. Camera moved? No. Lighting changed? No. Player moved? No. The GPU is completely bypassed. The display controller simply holds the previous buffer. The GPU drops to 0% utilization while delivering perfect visual continuity.

28

Architecture Defended

Ten More Questions — All Solved
-------------------------------

These are the questions that come after the first four. The ones that only appear once someone has understood the system well enough to push deeper. Every single one has an answer built into the architecture.

### Q: Floating point values have billions of possible states. How can the pool ever match them?

**A: Digit trimming. The pool matches itself.**

The pool does not need a manually configured threshold. It keeps removing trailing digits from both values until they converge on a key that already exists. 2.0000001 and 2.0000002 both trim to 2. The pool defines the precision level by what it already contains. No configuration. No context needed. Self-calibrating by design.

### Q: What if two scripts produce contradicting certain outcomes simultaneously? Player dies AND player heals at the same moment?

**A: The queue reads both scripts and compares values.**

If the heal value is lower than the damage value — death is certain. Pre-load death. If the heal value is higher — survival is certain. Pre-load survival. The queue does not guess between them. It reads both scripts, compares the numbers, and the math decides. One outcome. Always certain.

CONFLICT RESOLUTION

damage: 80 heal: 30 → net: \-50 → pre-load death  
damage: 80 heal: 120 → net: +40 → pre-load survival

### Q: If a script reads pool state to determine its outcome, and the pool pre-loads based on that script — isn't that circular?

**A: The queue reads the script. That's all it needs.**

If the result is already in the pool, the script doesn't need to run at all — the pool already has the answer. The queue only reads scripts for outcomes that aren't pooled yet. Once something is pooled, the script is bypassed entirely. There is no loop because the pool eliminates the condition that would create one.

### Q: The intentional delay sounds bad. Won't players feel it?

**A: The delay adapts based on cache hits.**

The queue monitors cache hit rate in real time. High cache hits means the pool is warm and pre-loading fast — delay shrinks. Low cache hits means the pool needs more time to prepare — delay grows slightly. The system calibrates its own breathing room based on how much it actually needs. In a warm session the delay is effectively zero. The player never feels what they never notice.

### Q: In multiplayer, two machines have different pools and different queue timings. How does this not desync?

**A: Partial sync. Input is queued. Everything else follows the server.**

Player input enters the client queue and is transmitted to the server. The server's queue reads the scripts that input triggers and pre-loads outcomes. Both sides resolve to the same result because the server is canonical truth and the pool is deterministic. The client queue handles input. The server queue handles world state. They coordinate without being identical.

### Q: What about completely procedurally generated games? The pool has never seen any of it.

**A: Fractional routing. Cold starts are almost never 100% cold.**

A procedurally generated event is novel as a combination — but its sub-pieces are not. Gravity is gravity. Wind is wind. Collision physics is collision physics. PELTGC routes every sub-component it already knows and only computes the genuinely new combination at the top. The more the pool has seen, the smaller the cold piece becomes. Even in a fully procedural game, the pool is solving most of the work from day one.

### Q: Thread collisions seem inevitable at scale. Twelve threads will eventually want the same thing.

**A: They never reach that point. The queue separates them before they start.**

Every thread's job is queued before execution begins. The queue sees what every thread is about to do and distributes work so no two threads are ever reaching for the same calculation. A collision requires two threads to want the same thing at the same time. The queue makes that structurally impossible by the time threads are running.

### Q: How does the pool decide what to keep vs what to let go dormant under memory pressure?

**A: Efficiency tracking. The pool knows exactly what is worth keeping.**

Every entry tracks cache hits and compute matches — how many times it was used and how much compute it saved. Low efficiency entries merge with similar ones or lose their detail and keep only the useful core. The pool curates itself continuously. It never bloats blindly. It gets leaner and smarter over time, not just larger.

### Q: Cold start sounds rough for the first session. How warm is it really on first run?

**A: Warmer than it sounds. The queue is active from frame one.**

Even on first run the Script Queue is reading scripts and pre-loading certain outcomes within the same session as they become known. The pool fills live as the game runs. By the middle of the first session it is already routing large portions of work. Cold start is not a blank session — it is a live calibration that gets warmer every minute.

### Q: NDF seems reactive — it checks after the fact whether a frame changed. Can it do better?

**A: It already does. The queue tells it before the frame is due.**

If no scripts touching scene state are in the queue, NDF knows with certainty the next frame will be identical — before the frame cycle even begins. The GPU skip is preventive, not reactive. NDF does not check after the fact. It reads what is coming and acts before it arrives.

Every question above has an answer that was already inside the system. The architecture is not defended by adding exceptions. It is defended by showing the design already thought further ahead than the question did.

29

Architecture Defended

The Hard Engineering Critique — Four Attacks, Four Answers
----------------------------------------------------------

A serious systems architect reading this document raised four attacks. They are the best four attacks possible. Every one of them has an answer already built into the architecture — but the document did not make those answers visible enough. This chapter fixes that.

### Attack 1: The Memory Wall. An ALU adds two numbers in 1 cycle. A RAM lookup takes 100-300 cycles. Routing is slower than computing. You can't fit a 2GB pool in cache.

**The pool is not flat RAM. It mirrors the cache hierarchy exactly.**

The pool has tiers — and those tiers map directly to hardware memory layers:

COMMON

Pre-baked universal constants. Gravity, standard math, base physics. These live in L1/L2 cache directly on the die. Always sub-nanosecond. Never touch RAM. The silicon already knows them.

L1 / L2 cache

PROMOTED

Hot entries that the system learned are used constantly. Promoted specifically because their hit rate justifies permanent cache residency. They live in L3 cache — still orders of magnitude faster than RAM.

L3 cache

RARE

Cold and dormant entries. These live in RAM. They are not routed frequently — if they were, they would be promoted. The 100-300 cycle cost applies here, but these entries are cold by definition. They are rarely touched.

RAM — rarely hit

The critique assumes every pool lookup goes to RAM. That is only true for entries the system has correctly identified as rarely used. Everything hot is in cache. Everything truly constant is on-die. The architecture self-organizes exactly the way the critique demands — it just does it automatically through the tier system rather than manually.

A 1-cycle ALU operation beats a 300-cycle RAM lookup. A 1-cycle ALU operation does not beat a 4-cycle L1 cache lookup. PELTGC does not compete with the ALU on RAM lookups. It competes with the ALU on cache lookups — and it wins on every calculation it has seen before.

### Attack 2: The Causality Paradox. You cannot skip addresses 1 and 2 to reach address 3 without knowing what 1 and 2 produce as inputs first. You need the past to find the future.

**The merge happens at known outputs, not by skipping unknown inputs.**

The critique reads chain compression as: skip addresses 1 and 2, jump to 3. That is not what happens. What actually happens:

What the critique thinks happens

addr 1: player velocity — SKIPPED???

addr 2: wind force — SKIPPED???

addr 3: combined force — pool hit

Problem: how do you get addr 3's key without 1 and 2?

What actually happens

addr 1: player velocity — pool hit \[route, ~4 cycles\]

addr 2: wind force — pool hit \[route, ~4 cycles\]

addr 3: combined force — pool hit \[route, ~4 cycles\]

All three routed. Total: ~12 cycles. Not skipped — fast.

Addresses 1 and 2 are not skipped. They are routed — meaning they execute at cache speed instead of compute speed. Their outputs are known immediately. Those outputs form the key for address 3. Address 3 is then also routed. The chain is not shortcut by skipping steps — it is compressed by making every step instant. The causality is preserved. The compute is eliminated.

The merge in Chapter 4 refers to **pointer deduplication** — collapsing multiple pointers that reference the same already-computed result into one. Not to skipping prerequisite steps.

### Attack 3: State Space Explosion. Even trimmed to 2 decimal places, an open world game produces trillions of unique states. The index map alone fills 32GB.

**The pool is not an exhaustive state map. It is a curated efficiency structure.**

The critique imagines the pool stores every unique combination of X, Y, Z, rotation, velocity, and animation frame ever encountered. That would indeed be trillions of entries. That is not what the pool stores.

The pool stores **individual calculation results** — not combined world states. Gravity at 9.81 is one entry. A velocity of 5.2 m/s is one entry. The result of multiplying them is one entry. It does not store "player at position 342.5, 128.3, 0, rotation 45°, velocity 5.2, frame 12" as a single entry. It stores each of those values and operations individually.

And critically — the pool curates itself. Entries that are never hit again go dormant and eventually compress. The pool is not a ledger that grows with every unique moment. It is a living structure that grows toward the calculations that matter and shrinks away from ones that don't.

What the critique assumes

Store: {x:342.5, y:128.3, rot:45, vel:5.2, frame:12}

Store: {x:342.6, y:128.3, rot:45, vel:5.2, frame:12}

Store: {x:342.7, y:128.3, rot:45, vel:5.2, frame:12}

Trillions of combined states → 32GB instantly

What actually happens

Store: gravity = 9.81 \[1 entry\]

Store: velocity = 5.2 \[1 entry\]

Store: 9.81 × 5.2 = 50.412 \[1 entry\]

Position routes via digit trimming. Unique ops only.

### Attack 4: The Halting Problem. Human input is unpredictable. The queue cannot know the future if the player presses the shield button 1ms before the hit.

**The queue never predicts human input. It waits for it, then reads what follows with certainty.**

This is the most important distinction in the entire system. The queue does not guess what the player will do. It does not predict button presses. Human input is genuinely unpredictable and the system makes no attempt to predict it.

What the queue does: the moment input arrives — the moment the player's button press enters the queue — the queue immediately reads the scripts that input will trigger and pre-loads their certain outcomes. The certainty begins **after** the input, never before.

What the critique thinks the queue does

Predict: player will not press shield

Pre-load: death animation

Player presses shield — WRONG

Pipeline flush — wasted work

What the queue actually does

Wait. Human input is unknown. Do not predict.

Player presses shield — input enters queue

Queue reads: shield equipped script triggers

Pre-load: block animation, parry window — certain.

The intentional delay exists precisely for this. When input arrives, the system has a brief window — microseconds — to read the triggered scripts and pre-load before execution catches up. The delay is not wasted time. It is the reaction window that makes post-input certainty possible.

If the player had NOT pressed shield: the enemy hit script triggers, queue reads it, death is certain, death is pre-loaded. If the player presses shield at the last millisecond: new input enters queue, queue discards the death pre-load, reads the shield script, pre-loads survival instead. The queue is fast enough that this switch costs almost nothing. Microseconds of re-routing versus milliseconds of execution time.

The queue does not predict humans. It reads code. Humans are unpredictable. Code, once triggered by human input, is not. That is the boundary. Everything before the button press is unknown. Everything after it is certain. The queue lives on the certain side of that line.

PELTGC — **Pooling is the GC.**

Think once · Remember forever · Reference when needed · Never think twice

"bright minds always glow like the smallest firefly around ones that don't matter"
