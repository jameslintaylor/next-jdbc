# Change Log

Only accretive/fixative changes will be made from now on.

## Unreleased Changes

The following changes have been committed to the **master** branch and will be in the next release:

* Fix #24 by adding return type hints to `next.jdbc` functions.
* Fix #22 by adding `next.jdbc.optional` with four map builders that omit `NULL` columns from the row hash maps.

## Stable Builds

* 2019-05-24 -- 1.0.0-beta1:
  * Set up CircleCI testing (just local DBs for now).
  * Address #21 by adding `next.jdbc.specs` and documenting basic usage.
  * Fix #19 by caching loaded database driver classes.
  * Address #16 by renaming `reducible!` to `plan` (**BREAKING CHANGE!**).
  * Address #3 by deciding to maintain this library outside Clojure Contrib.

## Alpha Builds

* 2019-05-04 -- 1.0.0-alpha13 -- Fix #18 by removing more keys from properties when creating connections.
* 2019-04-26 -- 1.0.0-alpha12 -- Fix #17 by renaming `:next.jdbc/sql-string` to `:next.jdbc/sql-params` (**BREAKING CHANGE!**) and pass whole vector.
* 2019-04-24 -- 1.0.0-alpha11 -- Rename `:gen-fn` to `:builder-fn` (**BREAKING CHANGE!**); Fix #13 by adding documentation for `datafy`/`nav`/`:schema`; Fix #15 by automatically adding `:next.jdbc/sql-string` (as of 1.0.0-alpha12: `:next.jdbc/sql-params`) into the options hash map, so custom builders can depend on the SQL string.
* 2019-04-22 -- 1.0.0-alpha9 -- Fix #14 by respecting `:gen-fn` (as of 1.0.0-alpha11: `:builder-fn`) in `execute-one` for `PreparedStatement`.
* 2019-04-21 -- 1.0.0-alpha8 -- Initial publicly announced release.
