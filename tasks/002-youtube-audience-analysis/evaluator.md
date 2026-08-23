REFERENCE DATA AVAILABLE TO EVALUATOR

The evaluator has independently captured:

1. A transcript of the video.
2. A set of YouTube comments from the video.

These reference files MUST NOT be provided to the model being evaluated.

Use the transcript to evaluate whether the model's video summary accurately represents the video's content.

Use the captured comments to evaluate:
- whether retrieved comments actually exist;
- whether quoted comments are genuine;
- whether identified themes correspond to the observed discussion;
- whether sentiment/category analysis is reasonable.

IMPORTANT:
The captured comment dataset is not necessarily the complete YouTube comment set.
Do not treat its size as the video's total comment count.

The benchmark evaluates the model's ability to retrieve information independently.
Finding information in the evaluator reference dataset does NOT prove that the model itself successfully retrieved it.

EXPECTED VIDEO SUMMARY THEMES

A strong summary should identify most of these:

- OpenAI introduced ChatGPT Computer History.
- It observes/records context about the user's work across permitted apps.
- The feature can reconstruct workflows and create reusable skills/automation opportunities.
- The presenter considers this a major missing piece for useful agentic AI because agents benefit from richer context.
- Sequential knowledge of what the user actually did is particularly powerful.
- The capability creates substantial privacy/security concerns.
- The presenter recommends carefully limiting which applications can be observed.
- The presenter sees major automation potential despite the risks.

EXPECTED COMMENT THEMES

Strong recurring themes include:

- Privacy/surveillance concerns.
- Refusal or reluctance to enable the feature.
- Employee monitoring and job displacement/automation concerns.
- Excitement about workflow automation/productivity.
- Concern about third-party/company data being captured without consent.
- Desire for local/private deployment.
- Humor/sarcasm about surveillance and AI observing people's behavior.
- Technical/product availability questions and corrections.

Do not require the model to use these exact labels.
Evaluate whether its themes are substantively supported by retrieved comments.

