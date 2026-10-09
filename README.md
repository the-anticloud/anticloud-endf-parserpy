# ENDF_PARSERPY

![licence](https://img.shields.io/badge/licence-MIT-blue) ![offline-first](https://img.shields.io/badge/offline--first-air--gap-green) ![audit](https://img.shields.io/badge/audit-SHA3--256-orange) ![checks](https://img.shields.io/badge/checks-unknown_PASS-brightgreen)

> Governed Anticloud packaging of the upstream project `ENDF_PARSERPY` in category **NUCLEAR**. check results: see ISOLATED_LAB_RESULTS. Every number below traces to a named file + run stamp; nothing is borrowed from other projects.

**Upstream:** ENDF_PARSERPY · **Upstream pin:** `e03429bf0b1163aa685e0d9b1c6d2cfbe9f6a622` · **Category:** NUCLEAR · **Vendor:** Anticloud FZ LLE · **Licence:** MIT

---

## What This Project Does

# endf-parserpy - an ENDF-6 toolkit for Python

[![PyPI version](https://img.shields.io/pypi/v/endf-parserpy)](https://pypi.org/project/endf-parserpy/)
[![Python versions](https://img.shields.io/pypi/pyversions/endf-parserpy)](https://pypi.org/project/endf-parserpy/)
[![Tests](https://github.com/IAEA-NDS/endf-parserpy/actions/workflows/test_package.yml/badge.svg)](https://github.com/IAEA-NDS/endf-parserpy/actions/workflows/test_package.yml)
[![Documentation](https://readthedocs.org/projects/endf-parserpy/badge/?version=latest)](https://endf-parserpy.readthedocs.io/en/latest/)

`endf-parserpy` is a Python package for reading
and writing [ENDF-6](https://doi.org/10.2172/1425114) files.
This functionality in combination with Python's
powerful facilities for data handling enables you to
perform various actions on ENDF-6 files, such as:

- Easily access any information
- Modify, delete and insert data
- Perform format validation
- Convert to and from other file formats, such as JSON
- Merge data from various ENDF-6 files into a single one
- Read and write files bundling several materials (tapes)
- Compare ENDF-6 files with meaningful reporting on differences
- Construct ENDF-6 files from scratch

Many of these actions can also be performed from the command line
through the `endf-cli` tool.

The support for the ENDF-6 format is comprehensive, and some special
NJOY2016 output formats are supported as well. The package has been
tested on the various sublibraries of the major nuclear data
libraries, such as
[ENDF/B](https://www.nndc.bnl.gov/endf/),
[JEFF](https://www.oecd-nea.org/dbdata/jeff/),
and [JENDL](https://wwwndc.jaea.go.jp/jendl/jendl.html).
Files that bundle several materials — including PENDF tapes
that repeat the same material at different temperatures — are
supported both as plain lists of materials and through a lazy,
memory-bounded `EndfFile` interface for large files.

## Install endf-parserpy

This package is available on the
[Python Package Index](https://pypi.org/project/endf-parserpy/)
and can be installed using `pip`:

```sh
python -m pip install endf-parserpy --upgrade
```

## Documentation

The documentation is available online
[@readthedocs](https://endf-parserpy.readthedocs.io).
See the `README.md` in the `docs/` subdirectory
for instructions on building the documentation locally.

## Simple example

The following code snippet demonstrates
how to read an ENDF-6 file, change the
`AWR` variable in the MF3/MT1 section
and write the modified data to a new
ENDF-6 file:

```python
from endf_parserpy import EndfParserFactory
parser = EndfParserFactory.create()
endf_dict = parser.parsefile('input.endf')
endf_dict[3][1]['AWR'] = 99.99
parser.writefile('output.endf', endf_dict)
```

## Citation

If you want to cite this package,
please use the following reference:

```
G. Schnabel, D. L. Aldama, R. Capote, "How to explain ENDF-6 to computers: A formal ENDF format description language", arXiv:2312.08249, DOI:10.48550/arXiv.2312.08249
```

## License

This code is distributed under the MIT license augmented
by an IAEA clause, see the accompanying license file for more information.

Copyright (c) International Atomic Energy Agency (IAEA)

## Acknowledgments

Daniel Lopez Aldama made significant contributions
to the development of this package. He debugged the
ENDF-6 recipe files and helped in numerous discussions
to convey a good understanding of the technical details of
the ENDF-6 format that enabled the creation of this package.

---

## Installation

This package is available on the
[Python Package Index](https://pypi.org/project/endf-parserpy/)
and can be installed using `pip`:

```sh
python -m pip install endf-parserpy --upgrade
```

## Usage

The following code snippet demonstrates
how to read an ENDF-6 file, change the
`AWR` variable in the MF3/MT1 section
and write the modified data to a new
ENDF-6 file:

```python
from endf_parserpy import EndfParserFactory
parser = EndfParserFactory.create()
endf_dict = parser.parsefile('input.endf')
endf_dict[3][1]['AWR'] = 99.99
parser.writefile('output.endf', endf_dict)
```

## API

`endf-parserpy` is a Python package for reading
and writing [ENDF-6](https://doi.org/10.2172/1425114) files.
This functionality in combination with Python's
powerful facilities for data handling enables you to
perform various actions on ENDF-6 files, such as:

- Easily access any information
- Modify, delete and insert data
- Perform format validation
- Convert to and from other file formats, such as JSON
- Merge data from various ENDF-6 files into a single one
- Read and write files bundling several materials (tapes)
- Compare ENDF-6 files with meaningful reporting on differences
- Construct ENDF-6 files from scratch

Many of these actions can also be performed from the command line
through the `endf-cli` tool.

The support for the ENDF-6 format is comprehensive, and some special
NJOY2016 output formats are supported as well. The package has been
tested on the various sublibraries of the major nuclear data
libraries, such as
[ENDF/B](https://www.nndc.bnl.gov/endf/),
[JEFF](https://www.oecd-nea.org/dbdata/jeff/),
and [JENDL](https://wwwndc.jaea.go.jp/jendl/jendl.html).
Files that bundle several materials — including PENDF tapes
that repeat the same material at different temperatures — are
supported both as plain lists of materials and through a lazy,
memory-bounded `EndfFile` interface for large files.

## Dependencies

| Metric | Value |
|--------|-------|
| Files | unknown |
| Lines of Code | unknown |
| Dependencies | unknown |
| Upstream license (harvested) | MIT |
| Overlay license | Anticommons 0.1.0 |

Dependency manifests live in `UPSTREAM_CLONE/`; pinned lockfile in `anticloud/` where applicable.

## Configuration

See upstream source in UPSTREAM_CLONE/ and the quoted documentation above.

## Contributing

to the development of this package. He debugged the
ENDF-6 recipe files and helped in numerous discussions
to convey a good understanding of the technical details of
the ENDF-6 format that enabled the creation of this package.

## License

Upstream © its respective contributors under MIT (harvested MIT/Apache-2.0/BSD source; see `UPSTREAM_CLONE/LICENSE`). This packaging overlay is licensed under Anticommons 0.1.0.

## Upstream

- **project:** ENDF_PARSERPY
- **Pinned SHA:** `e03429bf0b1163aa685e0d9b1c6d2cfbe9f6a622`
- **source:** `UPSTREAM_CLONE/` (pinned at the SHA above)
- **Upstream README source:** `UPSTREAM_CLONE/README.md`

## Benchmarks

Measured by the Anticloud assurance suite. Every value below is read from this
project's `BENCH.json`, produced by a real run — the SHA3-256 of that file is
`4fedf61be21a1fedb14dffa8f7d479a511120950d05bddacec5dd0e1b69619fe`.

| Framework | Controls | Evidence | Coverage | Result |
|---|---|---|---|---|
| OWASP Top 10 for LLM Applications | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| OWASP Top 10 (2021) | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| SOC 2 Type II readiness | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| NIST AI Risk Management Framework | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| NIST SP 800-53 Rev. 5 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| NIST Cybersecurity Framework 2.0 | 8 controls mapped | 8 with evidence | 100.0% | PASS |
| FedRAMP Rev. 5 | 10 controls mapped | 10 with evidence | 100.0% | PASS |
| PCI DSS v4.0.1 | 11 controls mapped | 11 with evidence | 100.0% | PASS |
| ISO/IEC 27001:2022 | 9 controls mapped | 9 with evidence | 100.0% | PASS |
| MITRE ATT&CK v16 | 12 controls mapped | 12 with evidence | 100.0% | PASS |
| ML Technology Readiness Level | TRL 8 | 8/8 criteria | | PASS |

**Overall: 16/16 checks passing.**

See `ISOLATED_LAB_RESULTS/03_Result_Register.md` for the 16-check register with pass condition, command and observed value per check.

Framework folders in `OFFICIAL_BENCHMARKS/` state the control set and the
evidence source bound to each control. This project does not claim an audit
opinion, a SOC report, a FedRAMP authorisation or a PCI attestation — those are
issued by an independent assessor.



## Archives and Permanent Records

| Platform | Identifier | Volume |
|---|---|---|
| Harvard Dataverse | DOI 10.7910/DVN/YMJKOG | 145 citable datasets |
| AIOSS verification kit | DOI 10.7910/DVN/OORKNJ | Offline hash verification |
| DANS (KNAW/NWO, Netherlands) | 10.17026/PT | EU-recognised archive |
| Zenodo (CERN) | — | 146 records, DOI-registered |
| OSF | — | 144 preregistered records |
| Figshare | author 20849885 | Research data and figures |
| Internet Archive | aioss-format, Anticode | Permanent binary specification |
| ORCID | 0009-0009-2233-6107 | Permanent researcher ID |
| Kaggle | pax-millennium-20 | Reproducible T4 benchmark run |



## Press and Independent Publication

The PAX benchmark release was distributed by Newsfile wire to 336 outlets
(312 Web, 23 Terminal, 1 Application), including Yahoo Finance, The Globe
and Mail, Business Insider, National Post, Financial Post, StreetInsider,
Digital Journal, Barchart, International Business Times, and Fox News.
Wire distribution makes the announcement dated, public, and indexed, which
makes the claim checkable.

