<!---------------------- GNU General Public License 3.0 ------------------------
--                                                                            --
-- Copyright (C) 2022─2023 Kevin Matthes                                      --
--                                                                            --
-- This program is free software: you can redistribute it and/or modify       --
-- it under the terms of the GNU General Public License as published by       --
-- the Free Software Foundation, either version 3 of the License, or          --
-- (at your option) any later version.                                        --
--                                                                            --
-- This program is distributed in the hope that it will be useful,            --
-- but WITHOUT ANY WARRANTY; without even the implied warranty of             --
-- MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the              --
-- GNU General Public License for more details.                               --
--                                                                            --
-- You should have received a copy of the GNU General Public License          --
-- along with this program.  If not, see <https://www.gnu.org/licenses/>.     --
--                                                                            --
------------------------------------------------------------------------------->

<!------------------------------------------------------------------------------
--
--  AUTHOR      Kevin Matthes
--  BRIEF       Important information regarding this project.
--  COPYRIGHT   GPL-3.0
--  DATE        2022─2023
--  FILE        README.md
--  NOTE        See `LICENSE' for full license.
--
------------------------------------------------------------------------------->

# cff-release-today

## Summary

[![](https://bors.tech/images/badge_small.svg)](https://app.bors.tech/repositories/59793)
[![](https://github.com/kevinmatthes/cff-release-today/workflows/ci/badge.svg)](https://github.com/kevinmatthes/cff-release-today/workflows/ci)
[![](https://img.shields.io/github/license/kevinmatthes/cff-release-today)](https://github.com/kevinmatthes/cff-release-today)

Set the release date of the CITATION.cff to the present day.

1. [License](#license)
1. [Description](#description)
1. [Inputs](#inputs)
   1. [`validate`](#validate)
1. [Branding Information](#branding-information)

## License

[![](https://img.shields.io/github/license/kevinmatthes/cff-release-today)](https://github.com/kevinmatthes/cff-release-today)

This project's license is **GPL-3.0**.  The whole license text can be found in
`LICENSE` in the main directory of this repository.  The brief version is as
follows:

> Copyright (C) 2022─2023 Kevin Matthes
>
> This program is free software: you can redistribute it and/or modify
> it under the terms of the GNU General Public License as published by
> the Free Software Foundation, either version 3 of the License, or
> (at your option) any later version.
>
> This program is distributed in the hope that it will be useful,
> but WITHOUT ANY WARRANTY; without even the implied warranty of
> MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
> GNU General Public License for more details.
>
> You should have received a copy of the GNU General Public License
> along with this program.  If not, see <https://www.gnu.org/licenses/>.

## Description

This GitHub Action will set the entry of the field `date-released` in the
top-level scope of a CITATION.cff to the present day.  The present day is
thereby determined by the locale settings of the runner executing this Action.

The field to be updated needs to match the following regular expression.

```
^date-release: ....-..-..
```

Thus, the date must not be enclosed in neither single nor double quotes and must
be separated from the field's name by exactly one space character.

The update is processed using calls to the following three UNIX applications:

- `sed`
- `date`
- `mv`

It is recommended to execute this Action on a Linux runner as tests have shown
that these applications are available out-of-the-box on GitHub's default Linux
runner.  This Action requires a Bash shell environment.  There are no ouputs.

This Action only operates on the file named CITATION.cff, stored in the
respective repository's root directory.  It will succeed even if there is no
`date-released` field given in the top-level scope of the CITATION.cff to work
on but it will fail if there is no CITATION.cff in the root directory of the
respective repository.

To apply this Action, just add the following line to the step section of a
GitHub Action workflow job.

```yaml
      - uses: kevinmatthes/cff-release-today@v0.3.1
```

## Inputs

### `validate`

This input is **optional**.  When set to `true`, the CITATION.cff will be
[checked for validity](CITATION.cff#L107-L128) before being updated.  This is
set to `true`, by default.

## Branding Information

The branding of this Aciton uses the icon `sunrise` on a green background.  The
sunrise shall symbolise the "dawn" of a new version.  The colour green was
chosen as it is often associated with the season spring which, again, stands for
the beginning of something new.

<!----------------------------------------------------------------------------->
