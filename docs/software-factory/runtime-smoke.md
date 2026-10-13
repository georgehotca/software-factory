# Local runtime smoke diagnostic

This file records a local Software Factory runtime diagnostic. It confirms the expected marker file exists with exact contents; it does not establish that a change was merged, deployed, or verified in a remote environment.

Validate the marker from the repository root with:

```sh
python3 -c "from pathlib import Path; assert Path('docs/software-factory/runtime-smoke.txt').read_text() == 'software factory local runtime verification' + chr(10)"
```

A successful command exit confirms the marker text and its trailing newline match the diagnostic expectation.
