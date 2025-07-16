# RedFlagger
Find Red Flags in a WA conversation

## MVP System Design
🧾 1. Input Module: User uploads .txt export of WhatsApp chat.
Parser splits messages: sender, timestamp, content.

🧮 2. Preprocessing & Chunking: Clean metadata, remove system messages.
Chunk into: Per day / week
Per topic turn (based on shifts in conversation)

🧰 3. Analysis Engines (Chains)
🔴 Red Flag Detector

Prompts LLM to find:
- Gaslighting
- Breadcrumbing
- Guilt-tripping
- Blame-shifting
- Love bombing
- Silent treatment

Output: Flag + explanation + message reference.

😐 Emotional Consistency Analyzer
- Tone analysis over time.
- Detects shifts in sentiment, message volume, use of positive/negative words, emojis.

Outputs: Timeline of mood vs engagement.

💔 Relationship Health Score
Summary chain + scoring rubric.

Factors: balance of effort, tone mismatch, emotional support.

📝 Closure Report Generator
- Final AI-generated letter:
- Summary of dynamics
- What went wrong
- What the user can learn

A fictional “last message” for closure

📊 4. Frontend (optional MVP interface)
- Simple Streamlit UI

Upload chat 
Run analysis
Visual output: flags, charts, downloadable report
