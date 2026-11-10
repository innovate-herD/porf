Exploring a Lightweight AI Assistant for PLC Logic & Symbol Cross-Referencing
Something for control systems engineers, to trace variable dependencies across multiple data blocks, reviewing tag tables, and double-checking safety interlocks and scan-cycle execution order to ensure code runs safely and deterministically.

While full enterprise toolchains have their place, I wanted to experiment with something leaner: a standalone, browser based Proof of Concept acting as a slimmed down AI agent for PLC logic inspection and tag cross-referencing.

I put together a lightweight, zero-install HTML package that runs right in the browser, giving engineers a quick way to:

Audit Routine Logic: Scan Structured Text (IEC 61131-3), Siemens SCL, and Rockwell L5X code blocks for safety interlock bypasses, timer reset traps, and double-coil scan race conditions.

Symbol Table Cross-Referencing: Cross-reference routine logic against variable symbol tables to flag address memory overlaps, implicit type mismatches, and undeclared tags.

Instant Refactoring: Receive clean, normalized code suggestions with scan conflicts resolved.

Want to test it out? Grab the package directly from GitHub, extract it, and open index.html  

If you want to update the Gemini 3.8 fetch to the latest use the following below: 
const res = await fetch(`https://generativelanguage.googleapis.com/v1beta/models/gemini-3.8-flash:generateContent?key=${apiKey}`, {
You can edit the index.html file source code, and find FETCH. Then copy provided 3.8. 
