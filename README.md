# S2ST-VoiceEval

Models and evaluation protocols for cross-lingual voice preservation in speech-to-speech translation.

**Status: model release in preparation.** Checkpoints and inference instructions are coming soon.

## Overview

S2ST-VoiceEval evaluates how well a translated speech output preserves the source speaker's voice. Given a source-language recording and candidate outputs in another language, the evaluator compares speaker-embedding cosine similarities to rank the candidates by voice preservation.

At inference, the adapted evaluator uses the source recording and candidate outputs. It does not require a target-language recording of the same speaker.

The project accompanies **Cross-Lingual Voice-Preservation Evaluation in Speech-to-Speech Translation**. A public paper link and citation will be added when available.

## Method

The evaluator adapts a WavLM speaker model using:

- **Bilingual identity adaptation (BIA):** supervised contrastive learning and relationship preservation on real bilingual speech.
- **Same-language ranking distillation:** an additional stage that transfers a frozen teacher's target-reference preferences to a student using source-language references.
- **Alternating language adaptation (ALA):** a language regularizer examined with and without the ranking stage.

Evaluation compares agreement with fixed proxy and human preference labels under source- and target-reference conditions. Voice preservation is evaluated separately from translation correctness and naturalness.

## Model release

| Resource | Status |
| --- | --- |
| Adapted model checkpoints | Coming soon |
| Installation and inference instructions | Coming soon |
| Evaluation documentation | Coming soon |
| Public paper link and citation | Coming soon |

Checkpoint download links, supported audio formats, dependencies, and runnable scoring examples will be documented with the model release.
