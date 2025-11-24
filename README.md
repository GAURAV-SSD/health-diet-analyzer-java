# Health & Diet Analyzer — Java (Humanized)

A small console Java app that helps hostel students (or anyone) get a quick sense of their daily diet quality and simple suggestions to improve it. I started this as a course project and kept the code intentionally simple so it's easy to read and extend.

Why I made this
- I wanted a local, no-friction tool to experiment with diet scoring rules without relying on external services.
- Built this during college to help friends in hostels understand nutrient gaps easily.

Quick summary
- Input: simple CSV or sample JSON data describing meals and food items.
- Output: daily nutrient totals, a simple score, and plain-language suggestions.
- Not medical advice — meant for prototyping and learning.

What’s new in this “humanized” version
- Friendlier README and usage examples.
- Short explanations of the scoring rationale instead of dry statements.
- Comments in code focus on why decisions were made, not just what the code does.
- Small TODOs and realistic limitations listed.

Quick start (Maven)
1. Requirements: Java 17+ and Maven.
2. Build:
   mvn clean package
3. Run (example):
   mvn exec:java -Dexec.mainClass=com.healthdiet.Main
   or
   java -cp target/classes com.healthdiet.Main

Simple run example (what you’ll see)
- "Welcome — enter today's meals or load sample_data/meals.csv"
- "Today's score: 68/100 — good job! Try adding more vegetables for fiber."

Project layout (where to look)
- src/main/java/com/healthdiet — core code (Main, Analyzer, models)
- data/ — sample inputs
- tests/ — unit checks (small set)

Design notes and limitations
- Scoring is intentionally simple and rule-based so you can change it quickly.
- Edge cases (allergic info, portion-size normalization) are out of scope for now.
- If you want clinical-grade advice, integrate a nutrition database and consult experts.

How to help / Contributing
- Report issues describing a use case or sample input.
- PRs welcome — small, focused changes with a note about why the change helps.
- When adding rules, include example input and expected output.

Author / Contact
- Gaurav Bhardwaj (GAURAV-SSD) — a college project owner. If you want me to keep developing this for a specific use (e.g., vegetarian hostel meal plans), say so and I’ll add a small config and examples.

Changelog (short)
- 0.1.0 — initial prototype (CSV input, scoring, console output)
- 0.1.1 — README and code comments rewritten to be more human, added CONTRIBUTING and CHANGELOG outlines

License
- Add your preferred license file (e.g., MIT) in the repo root to clarify reuse.