# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.6.0] - 2021-06-22
### Added
- Allow query service to query indexer metadata though add `--indexer <indexer-meta-api>` (#327)
- Add `_Metadata` in the query schema (#327)
### Changed
- change `lastProcessedHeight` and `targetHeight` type to `Int`. (#347)


## [0.5.0] - 2021-04-20
### Added
- Remove `condition` in query schema, please use `filter` instead (#260)
- `@jsonField` annotation is now supported in `graphql.schema` which allows you to store structured data JSON data in a single database field
  - We'll automatically generate coresponding JSON interfaces when querying this data (#275)
  - Read more about how you can use this in our [updated docs](https://doc.subquery.network/create/graphql.html#json-type)

## [0.4.0] - 2021-03-25
### Added
- support filter for condition search (#240)

## [0.3.2] - 2021-03-11
### Fixed
- add dependency of @subql/common for @subql/query (#233)

## [0.3.1] - 2021-03-11
### Fixed
- fix wrong cross package imports (#231)

## [0.3.0] - 2021-03-11
### Added
- refactor logger: support --output-fmt and --log-level (#220)
- use read db host (DB_HOST_READ from env) as priority (#221)

## 0.2.0 - 2021-02-05
### Added
- init query service project
- customise first/last plugin to give max record to query (#114)
- disable debug mode in production (#115)
- overwrite plugin to fix one to one unique key check
- update query publish and docker build process

[Unreleased]: https://github.com/subquery/subql/compare/v0.5.0...HEAD
[0.5.0]: https://github.com/subquery/subql/compare/v0.4.0...v0.5.0
[0.4.0]: https://github.com/subquery/subql/compare/v0.3.2...v0.4.0
[0.3.2]: https://github.com/subquery/subql/compare/v0.3.1...v0.3.2
[0.3.1]: https://github.com/subquery/subql/compare/v0.3.0...v0.3.1
[0.3.0]: https://github.com/subquery/subql/compare/v0.2.0...v0.3.0
