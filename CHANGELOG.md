# Changelog

## 2.9.0
- Add Anchor client
## 2.8.0
- Added `onPriceChangeVerbose` callback to `PythConnection` to support getting account keys and slots on each price update.

## 2.7.2
### Changed
- Added pythtest program key and cluster url
- Updated examples to work with pythtest

## 2.7.1
  Moved solana/web3 to peerDependencies 

## 2.7.0
  Added timestamp fields (overwriting existing reserved space)

## 2.6.3

### Changed
- Renamed websocket usage example to `example_ws_usage.ts`
- Updated documentation to describe usage for `PythHttpClient`

### Added
- Example code for using the http client in `example_http_usage.ts`

## 2.6.1

### Changed
- Changed TWAP to EMAP and TWAC to EMAC

## 2.6.0

### Added
- Checks current slot when parsing a Price account and set status to unknown if price is stale. Being stale means it is not updated in `MAX_SLOT_DIFFERENCE` slots (currently 25).
- Adds status field in PriceData to access the current status (considering price getting stale) easier.

### Changed
- Converts Some type/status structs to enums to be able to use them in a cleaner way. It's backward compatible.


## 2.5.3

### Fixed
Updated tests for Pyth symbology change

## 2.5.1

### Changed

Improved error message when passing an invalid cluster name to `pythProgramKeyForCluster`

## 2.5.0

### Changed

Restructure `drv2` field in `PriceData` to `minPublishers` and other future drv values

## 2.4.0

### Changed

Product only define `price` and `confidence` fields if it currently has a valid price

### Fixed

Memory leak in an underlying library

## 2.3.2

### Added

PythConnection 

## 2.2.0

### Added

numQuoters

## 2.1.0

### Added

Support new twap and twac

## 2.0.1

### Added

Types

## 2.0.0

### Added

Support for v2 account structure

### Removed

Support for v1 account structure

## 1.0.7

### Changed

allow nextPriceAccountKey to be null

## 1.0.6

### Changed

Updated README.md

## 1.0.5

### Fixed

Respect size when parsing product metadata

## 1.0.4

### Fixed

Gatsby support

## 1.0.3

### Fixed

Do not rely on Buffer's readBig(U)Int64LE

## 1.0.2

### Changed

Repository url

## 1.0.1

### Fixed

Parse price as Big*Int*64

## 1.0.0

Initial release
