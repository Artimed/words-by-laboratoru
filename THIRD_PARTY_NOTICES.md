# Third-party materials

This inventory accompanies the public preview. Each third-party component retains
its own terms; this file does not license the original Words code as open source.

| Material | Use and notice |
| --- | --- |
| open-dict-data/ipa-dict | Shared English IPA; revision 972cd67dd5f96bc5660e28070cde26e3928abcd7. MIT notice: docs/licenses/ipa-dict.txt. Learner-notation adaptations are documented in docs/VOCABULARY.md. |
| CMU Pronouncing Dictionary | Pronunciation provenance recorded by block-two source metadata, revision 74790861f652b15e4ac49015a90074ad62a27690. Preserve docs/licenses/CMUdict.txt. This notice is retained even though the visible IPA map has a separate source. |
| Sparkle 2.10.0 | In-app update framework. Its upstream LICENSE contains the MIT terms and additional bundled-component notices; preserve the complete file, not only its first section. Bundled license: LICENSES/Sparkle.txt. |
| CPython | Embedded CPython 3.11.17; its upstream license text is docs/licenses/python.txt and inside the runtime. |
| python-build-standalone | Pinned Astral release 20261013, Apple Silicon install_only archive. Upstream release: https://github.com/astral-sh/python-build-standalone/releases/tag/20261013. Preserve installed notices for pip, setuptools and their vendors. Additional native-library notices are in docs/licenses/python-runtime; their audit provenance is recorded in docs/qa/python-native-license-inventory.json. |
| macOS frameworks and voices | System services used by Words; no Apple voice recordings or system framework binaries are copied into the repository. |

The original starter list, editorial translations and Russian pronunciation hints
have separate provenance and licensing decisions from the code. English labels are
not a license to copy a proprietary dictionary's complete database or examples.
Dictionary websites used for spot checks are references, not permission to repackage
their contents. The project is not affiliated with Cambridge, Apple, OpenAI or
Anthropic; compatibility descriptions do not imply endorsement.

The builder copies the license texts into app resources, including the native
runtime notice subdirectory. The supplemental set covers bzip2, libffi, ncurses,
mpdecimal, Expat, OpenSSL, liblzma, SQLite, Tcl/Tk, libuuid, libedit and zlib;
additional upstream notices are retained conservatively and do not establish that
every named library is linked. The metadata also names zlib-ng: its matching
upstream notice is retained separately because it was absent from the full archive.

The supplemental notices were prepared after public build 12 and require a new
signed release to reach installed users. Existing runtime notice files were checked
against that build; this inventory is not a jurisdiction-specific legal opinion or
a completed audit of dictionary provenance. Original-app terms remain a separate,
unadopted draft and must not override third-party rights.
