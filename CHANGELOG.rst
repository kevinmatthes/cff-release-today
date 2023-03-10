.. --------------------- GNU General Public License 3.0 --------------------- ..
..                                                                            ..
.. Copyright (C) 2022─2023 Kevin Matthes                                      ..
..                                                                            ..
.. This program is free software: you can redistribute it and/or modify       ..
.. it under the terms of the GNU General Public License as published by       ..
.. the Free Software Foundation, either version 3 of the License, or          ..
.. (at your option) any later version.                                        ..
..                                                                            ..
.. This program is distributed in the hope that it will be useful,            ..
.. but WITHOUT ANY WARRANTY; without even the implied warranty of             ..
.. MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the              ..
.. GNU General Public License for more details.                               ..
..                                                                            ..
.. You should have received a copy of the GNU General Public License          ..
.. along with this program.  If not, see <https://www.gnu.org/licenses/>.     ..
..                                                                            ..
.. -------------------------------------------------------------------------- ..

.. -------------------------------------------------------------------------- ..
..
..  AUTHOR      Kevin Matthes
..  BRIEF       The development history of this project.
..  COPYRIGHT   GPL-3.0
..  DATE        2022─2023
..  FILE        CHANGELOG.rst
..  NOTE        See `LICENSE' for full license.
..              See `README.md' for project details.
..
.. -------------------------------------------------------------------------- ..

.. -------------------------------------------------------------------------- ..
..
.. _changelog.d: changelog.d/
.. _Keep a Changelog: https://keepachangelog.com/en/1.0.0/
.. _Scriv: https://github.com/nedbat/scriv
..
.. -------------------------------------------------------------------------- ..

Changelog
=========

All notable changes to this project are documented in this file.  The format is
based on `Keep a Changelog`_ and optimised for maintenance with `Scriv`_.

Unreleased
----------

All pending changelog entries are stored in `changelog.d`_.

.. scriv-insert-here

.. _changelog-0.5.2:

0.5.2 — 2023-03-06
------------------

Fixed
.....

- documentation:  "Git" instead of "git" in README of ``LICENSEs``

.. _changelog-0.5.1:

0.5.1 — 2023-03-01
------------------

Changed
.......

- Dependabot(deps): Bump kevinmatthes/validate-boolean from 0.1.1 to 0.1.2

.. _changelog-0.5.0:

0.5.0 — 2023-03-01
------------------

Added
.....

- Action:  option to commit the changes

- CFF:  cite Git identity setup Action

- CI:  new test cases for self-test (option ``commit``)

- documentation:  software license of ``cut``

- documentation:  software license of ``fregante/setup-git-user``

- documentation:  software license of Git

- documentation:  software license of ``grep``

- README:  document new input value

- Action:  option to push committed changes

- README:  document new input value

Changed
.......

- documentation:  software license of ``date``

- documentation:  software license of ``mv``

.. _changelog-0.4.0:

0.4.0 — 2023-02-28
------------------

Added
.....

- Action:  option to checkout the repository

- CI:  new test cases for self-test (option ``checkout``)

- README:  document new input value

- documentation:  software license of ``actions/checkout``

- documentation:  software license of
  ``citation-file-format/cffconvert-github-action``

- documentation:  software license of ``date``

- documentation:  software license of ``kevinmatthes/validate-boolean``

- documentation:  software license of ``mv``

- documentation:  software license of ``sed``

- README:  document new directory ``LICENSEs``

Changed
.......

- README:  adjust wording of Action application description

.. _changelog-0.3.1:

0.3.1 — 2023-02-26
------------------

Removed
.......

- GitHub Action workflows:  ``ad-m/github-push-action@v0.6.0`` as dependency

.. _changelog-0.3.0:

0.3.0 — 2023-02-26
------------------

Added
.....

- Action:  option to validate the CFF before updating it

- CFF:  cite CFF validation Action

- CI:  new test cases for self-test (option ``validate``)

- README:  document new input value

.. _changelog-0.2.2:

0.2.2 — 2023-02-26
------------------

Added
.....

- README:  Bors badge

Changed
.......

- Action:  unify update steps for main CFF

- README:  adjust branding information description

Fixed
.....

- Bors:  copyright years of configuration file

.. _changelog-0.2.1:

0.2.1 — 2023-02-08
------------------

Added
.....

- Bors:  initial setup

.. _changelog-0.2.0:

0.2.0 — 2023-01-23
------------------

Added
.....

- CODEOWNERS

- CI:  GitHub Action self-test

Changed
.......

- CI:  rename CFF validation workflow to ``ci.yml``

- README:  change CFF validation badge to CI badge

.. _changelog-0.1.3:

0.1.3 — 2023-01-08
------------------

Changed
.......

- use own GitHub Action for Scriv fragment creation

- bump2version:  track moved Scriv settings file

- Scriv:  move settings to fragment storage

- use own GitHub Action for release preparations

Removed
.......

- Dependabot:  Python 3 setup

- placeholder in Scriv fragment storage

- Python 3 software requirements list

.. _changelog-0.1.2:

0.1.2 — 2023-01-06
------------------

Changed
.......

- update copyright years to "2022─2023"

.. _changelog-0.1.1:

0.1.1 — 2023-01-06
------------------

Changed
.......

- update Dependabot milestones

- Dependabot(deps): Bump actions/checkout from 3.2.0 to 3.3.0

.. _changelog-0.1.0:

0.1.0 — 2022-12-25
------------------

Added
.....

- create this repository

- license:  GPL-3.0

- repository README

- CITATION.cff

- GitHub Action workflow:  CFF validation

- bump2version:  track CITATION.cff

- bump2version:  track Scriv settings

- CHANGELOG fragment directory

- Dependabot:  GitHub Action setup

- Dependabot:  Python 3 setup

- GitHub Action workflow:  release

- GitHub Action workflow:  Scriv fragment creation

- list of Python 3 software requirements

- Python 3 software requirement:  bump2version

- Python 3 software requirement:  Scriv

- settings:  bump2version

- settings:  Scriv

- this CHANGELOG

- bump2version:  track README

- create GitHub Action source file

- detailed description to the README

- make release workflow use this repository's Action

- make this Action run in Bash shell environments

.. -------------------------------------------------------------------------- ..
