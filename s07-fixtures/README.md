# M046 S07 designated development source

These are source-authored inputs for fresh development acceptance on this test branch. The application manifests on master remain part of the source oracle. `source-expectations.json` records exact source hashes and contextual expectations before any scan; its relative case expectations come from the frozen, independently authored scanner corpus at the stated revision.

The fixtures include custom pip inputs and two distinct pip 26.0.1 observations, npm and Cargo lock edges, unresolved Go/Python declarations, an empty npm application, ignored prose, unsupported source and execution traps. Do not install dependencies, run package scripts or execute setup.py to inspect these inputs. The complete source remains incompletely inventoried; it must never be presented as a clean dependency result. Four advisory groups are required independently on each pip occurrence, with the actual frozen advisory identity recorded.

This branch is prepared locally before publication or scan submission. It does not establish release, development, human or rollback acceptance.
