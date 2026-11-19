# Python Collections Practice Questions

Despite its repository name, `String Based PracticeQuestions.ipynb` covers strings, lists, tuples and sets. The notebook has eleven code cells: three section-label strings, six syntactically valid exercise blocks, one invalid set-exercise block and a final empty cell.

## Contents

String helpers cover case conversion, slicing, word operations, character counts, regular-expression sketches, a Caesar cipher and CSV parsing. Other blocks contain list and tuple operations, followed by set exercises. Many questions share a single large cell rather than a separate cell per exercise.

## Read locally

Open in Jupyter or a notebook-capable editor using Python 3. Shown imports are standard-library modules: `re`, `collections`, `string`, `csv` and `random`. Some collection exercises are interactive. Run sections selectively and inspect state changes: examples mutate and clear collections, reuse names and depend on earlier values.

## Confirmed limits

- Cell 10 (one-based) has a mismatched closing bracket in its nested-set example. The entire cell fails Python parsing before any of its set examples run. It also contains assumptions about helper functions and collection state that need review before use.
- `find_longest_word("")` raises `ValueError`; `most_frequent_word("")` raises `IndexError`.
- `extract_domain_name` raises `IndexError` when its input has no `@` character.
- `count_syllables` actually counts whitespace-separated words, not syllables.
- `convert_csv_to_list` strips newlines and returns one flat parsed row, not the list-of-lists promised by its exercise comment.
- `remove_whitespaces` removes ordinary spaces only; word helpers often use substring operations rather than token boundaries. Email/URL regular expressions and the Caesar cipher are learning sketches, not production validation or security tools.

These are static and targeted review findings, not exhaustive validation. Original exercise code, saved outputs, names and history remain unchanged in this README-only update.
