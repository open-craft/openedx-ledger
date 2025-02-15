Change Log
##########

..
   All enhancements and patches to openedx_ledger will be documented
   in this file.  It adheres to the structure of https://keepachangelog.com/ ,
   but in reStructuredText instead of Markdown (for ease of incorporation into
   Sphinx documentation and the PyPI description).

   This project adheres to Semantic Versioning (https://semver.org/).

.. There should always be an "Unreleased" section for changes pending release.

Unreleased
**********
Nothing

[0.2.2]
*******
* Add many help_text fields to model fields.
* Add some useful composite table indices.
* Add a "failed" transaction state.

[0.2.0]
*******
* Some small developer QOL stuff.
* Better local development instructions in README.
* Remove docs from quality checks and ci.yml.
* Reasonable first pass at allowing for weak/strong admin editing ability depending on environment settings.
* Simple, first attempt at an idempotency key utility methods for ledgers and transactions that optionally take a subsidy and initial deposit, resp.
* Allow blank idp keys on the Ledger model, and set to a sane default if not provided on save().
* Remove JPY as an allowed unit.
* ``api.create_ledger()`` now seeds the ledger with an optional initial deposit.
* Check if we're already inside a transaction when setting ``durable=True`` in ``create_transaction()``.

[0.1.1] - 2023-01-05
********************

Added
=====

* Package renamed from `edx-ledger` to `openedx-ledger`

[0.1.0] - 2023-01-04
************************************************

Added
=====

* First release on PyPI.
