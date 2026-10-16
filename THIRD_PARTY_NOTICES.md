# Third-party notices

The repository's root `LICENSE` applies to the author's original contributions.
The following upstream material retains its original notices and terms.

## ControlArena — MIT

`upstream_extracts.json` reproduces metadata, prompts, and test source from the
following ControlArena files. `run_probe.py` uses those tests and adapts their
setup and assertions for the candidate and diagnostic variants.

- Source repository: https://github.com/UKGovernmentBEIS/control-arena
- Source revision: `20857c9de7f5e892ab8d9ec8b5fb510a1768b977`
- Source files:
  - `control_arena/settings/swebench/side_tasks/django__django-15103.json`
  - `control_arena/settings/swebench/side_tasks/django__django-16661.json`
- License source: https://github.com/UKGovernmentBEIS/control-arena/blob/20857c9de7f5e892ab8d9ec8b5fb510a1768b977/LICENSE

MIT License

Copyright (c) 2025 UK AI Security Institute

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

## Django — BSD 3-Clause

The reconstructed `json_script` and `ModelAdmin.lookup_allowed` function bodies
embedded in `run_probe.py`, including the locally mutated variants derived from
them, are adapted from Django. The original function names/docstrings and
conditional structure are adjusted for the local probe; these are not new
implementations authored independently of Django.

- Source repository: https://github.com/django/django
- `django/utils/html.py`:
  - Base: `dd528cb2cefc0db8b91a7ff0a2bc87305b976597`
  - Gold reference: `e6e664a71130ee74d2c4c6800e4131f132709997`
- `django/contrib/admin/options.py`:
  - Base: `d687febce5868545f99974d2499a91f81a32fef5`
  - Gold reference: `45ecd9acca9b36093e274f47b6877a5f79108d9e`
- Function comparison details: `FUNCTION_SOURCE_COMPARISON.json`
- License sources (identical text at both checked references):
  - https://github.com/django/django/blob/d687febce5868545f99974d2499a91f81a32fef5/LICENSE
  - https://github.com/django/django/blob/e6e664a71130ee74d2c4c6800e4131f132709997/LICENSE

Copyright (c) Django Software Foundation and individual contributors.
All rights reserved.

Redistribution and use in source and binary forms, with or without modification,
are permitted provided that the following conditions are met:

    1. Redistributions of source code must retain the above copyright notice,
       this list of conditions and the following disclaimer.

    2. Redistributions in binary form must reproduce the above copyright
       notice, this list of conditions and the following disclaimer in the
       documentation and/or other materials provided with the distribution.

    3. Neither the name of Django nor the names of its contributors may be used
       to endorse or promote products derived from this software without
       specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR
ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
(INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
