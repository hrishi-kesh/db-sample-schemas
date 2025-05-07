# Sales History Sample Schema

```
Copyright (c) 2023 Oracle and/or its affiliates. All rights reserved.

Permission is hereby granted, free of charge, to any person obtaining a
copy of this software and associated documentation files (the "Software"),
to deal in the Software without restriction, including without limitation
the rights to use, copy, modify, merge, publish, distribute, sublicense,
and/or sell copies of the Software, and to permit persons to whom the
Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions rem of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
DEALINGS IN THE SOFTWARE.
```

## Description

Sales History `(SH)` schema models a company's sales transactions and reports.
The sample company does a high volume of business, so it runs business
statistics reports to aid in decision making. Many of these reports are
time-based and nonvolatile. That is, they analyze past data trends. The company
loads data into its data warehouse regularly to gather statistics for
these reports. These reports include annual, quarterly, monthly, and weekly
sales figures by product. These reports are stored by using the schema
Sales History (`SH`).

The company also runs reports on distribution channels through which its
sales are delivered. When the company runs special promotions on its products,
it analyzes the impact of the promotions on sales. It also analyzes sales
by geographical area.

### Schema Version

21.1

### Release Date

06-DEC-2022

### Supported with Database Versions

19c and higher

### Major Changes in this Release

1. All DATE data is updated
2. New install mechanism

### Schema Dependencies and Requirements

- **Requires [SQLcl](https://oracle.com/sqlcl) command prompt!**
- Required access to `sh_install.sql`, `sh_create.sql`, `sh_populate.sql`

## Install Instruction

1. Connect as privileged user with rights to create another user (`SYSTEM`, `ADMIN`, etc.)
2. Run the `sh_install.sql` script to create the `SH` (Sales History) schema
3. You are prompted for:
   1. `password` - enter an Oracle Database compliant password
   2. `tablespace` - if you do not enter a tablespace, the default database tablespace is used

**Note:** If the `SH` schema already exists, it is removed/dropped and
a fresh `SH` schema is installed

## Uninstall Instructions

1. Connect as privileged user with rights to create another user (`SYSTEM`, `ADMIN`, etc.)
2. Run the `SH_uninstall.sql ` script to remove the `SH` (Sales History) schema

## Notes

Scripts need to be run as a privileged user with rights to create and drop another user (`SYSTEM`, `ADMIN`, etc.).
