# Third-party materials

This inventory accompanies the private preview. It does not apply a blanket license
to the entire repository or finish the public redistribution review.

| Material | Use and notice |
| --- | --- |
| open-dict-data/ipa-dict | Shared English IPA; revision 972cd67dd5f96bc5660e28070cde26e3928abcd7. MIT notice: docs/licenses/ipa-dict.txt. Learner-notation adaptations are documented in docs/VOCABULARY.md. |
| CMU Pronouncing Dictionary | Pronunciation provenance recorded by block-two source metadata, revision 74790861f652b15e4ac49015a90074ad62a27690. Preserve docs/licenses/CMUdict.txt. This notice is retained even though the visible IPA map has a separate source. |
| CPython | Embedded CPython 3.11.17; its upstream license text is docs/licenses/python.txt and inside the runtime. |
| python-build-standalone | Pinned Astral release 20261013, Apple Silicon install_only archive. See docs/PYTHON_RUNTIME.md for provenance and checksum. Preserve the upstream installed notices, including notices for bundled packages and libraries. Complete their component inventory before public redistribution. |
| macOS frameworks and voices | System services used by Words; no Apple voice recordings or system framework binaries are copied into the repository. |

The original starter list, editorial translations and Russian pronunciation hints
have separate provenance and licensing decisions from the code. English labels are
not a license to copy a proprietary dictionary's complete database or examples.
Dictionary websites used for spot checks are references, not permission to repackage
their contents. The project is not affiliated with Cambridge, Apple, OpenAI or
Anthropic; compatibility descriptions do not imply endorsement.

The builder currently copies the license texts in docs/licenses into app resources.
A public release must additionally verify that all shipped runtime notices remain
present, that data redistribution rights are documented, and that approved project
license/attribution files accompany both source and binary distributions.
