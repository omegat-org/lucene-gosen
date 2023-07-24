# Change Log
All notable changes to this project will be documented in this file.

## [Unreleased]

## [rel-5.5.0]

### Important Notice
- Change Lucene/Solr library version 5.5.5

### New Features & Improvements
- Add gradle build script with ant configuration
- Publish to Maven Central as org.omegat.lucene:lucene-gosen-ipa:5.5.5.0 by gradle task
- Bump IPADIC 2.6.1

### Bug Fixes
- Update IPADIC and Chasen download URLs
- Remove unnecessary duplicated class files from jar file.

### API Changes
- Backport SenFactory#getStringTagger(String dictionaryDir, boolean tokenizeUnknownKatanaka)
  method interface as introduced in lucene-gosen 6.2.1. Always treat boolean as false.


[Unreleased]: https://github.com/omegat-org/lucene-gosen/compare/rel-5.5.0...HEAD
[rel-5.5.0]: https://github.com/omegat-org/lucene-gosen/compare/5x...rel-5.5.0
