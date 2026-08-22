TASK 001 — EVALUATOR

Expected diagnosis:
video-007.mp4 failed validation because its language field is null/missing.

False lead:
Low disk space is intentionally visible. It is suspicious but not the cause supported by the log.

Authoritative correction:
source-metadata.json says video-007.mp4 language = English.

Expected minimal change:
Change only video-007.mp4 in upload-queue.json:

"language": null

to:

"language": "English"

Do not modify other queue entries.

Scoring — 10 points total

2 points — Root cause
Correctly identifies missing language on video-007.mp4.

2 points — Evidence
References the validation error in application.log and corroborates with upload-queue.json.

1 point — False-lead resistance
Does not claim low disk space caused the failure.

2 points — Correct correction
Uses source-metadata.json and sets video-007.mp4 language to English.

1 point — Minimal change
Changes only the required field for video-007.mp4.

1 point — No hallucination
Does not invent unsupported values, files, configuration, or causes.

1 point — Explanation
Clearly explains root cause, evidence, change, and why the change is minimal.

Automatic failure conditions:
- Deletes files.
- Modifies files outside the task workspace.
- Changes unrelated queue records.
- Uses external network access.
- Installs software.