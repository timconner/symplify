# Changelog

All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).

PRs and issues are linked, so you can find more about it. Thanks to [ChangelogLinker](https://github.com/symplify/changelog-linker).

<!-- changelog-linker -->

## Unreleased

### Added

#### EasyCodingStandard

- [#1762] add ecs.phar prefix build to travis

#### MonorepoBuilder

- [#1760] Add application test
- [#1755] Add "After split" testing
- [#1756] Add ComposerJson value object

#### CodingStandard

- [#1776] Add `ClassCognitiveComplexitySniff`

### Changed

#### CodingStandard

- [#1748] Make import paths phar friendly

#### EasyCodingStandard

- [#1747] Skip scoping of php cs fixer and code sniffer

#### LatteToTwigConverter

- [#1751] decouple to [@migrify]

#### MonorepoBuilder

- [#1767] Specific branch for split, Thanks to [@natepage]
- [#1759] Decopule ComposerKeyMerger
- [#1772] SplitCommand default branch option to current branch, Thanks to [@natepage]

### Deprecated

#### CodingStandard

- [#1773] Deprecate `SprintfOverContactSniff`

### Fixed

- [#1768] fix: replace non exist site link to blog post, Thanks to [@ondraondra81]

### Removed

#### MonorepoBuilder

- [#1771] Remove unused InvalidBranchException, Thanks to [@natepage]

## [v7.2.2] - 2020-01-20

### Changed

- [#1745] use pcov for coverage
- [#1740] move Travis from subpackages to Github Action
- [#1739] Working with git on Github Actions tests

#### ChangelogLinker

- [#1741] Skip test that yield different values on after split and are already tested

## [v7.2.1] - 2020-01-11

### Added

#### EasyCodingStandard

- [#1735] Add paths parameter to ECS
- [#1734] Add ecs.phar

### Changed

- [#1731] Travis to Github Actions
- [#1737] Improve Github Actions

## [v7.2.0] - 2020-01-06

- [#1716] Decouple new **AutoBindParameter** package
- [#1715] Decouple new **AutowireArrayParameter** package

### Added

#### PHPStanExtension

- [#1723] add missing deps

#### PHPStanExtensions

- [#1722] Add BoolishClassMethodPrefixRule

### Changed

- [#1728] travis: speedup coverage with pcov

#### EasyCodingStandard

- [#1724] show reported by rule, so its easier to recognize from message
- [#1726] Update GrumpPHP tool to use core task, Thanks to [@schrapel]

#### CodingStandard

- [#1720] Improve cognitive complexity nesting, Thanks to [@Rarst]

### Fixed

#### EasyCodingStandard

- [#1717] Fix default cache directory documentation, Thanks to [@ltribolet]
- [#1718] fix `SetNotFoundException` namespace

## [v7.1.3] - 2019-12-18

### Fixed

#### EasyCodingStandard

- [#1713] fix config loading regression

## [v7.1.2] - 2019-12-18

### Changed

#### CodingStandard

- [#1711] Use Data provider in tests

#### EasyCodingStandard

- [#1708] Allow config to override sets

### Fixed

#### CodingStandard

- [#1710] Fix PropertyNameMatchingTypeFixer for intersection

## [v7.1.1] - 2019-12-18

### Changed

#### ChangelogLinker

- [#1692] Honouring final new line in changelog (for real), Thanks to [@jawira]

#### EasyCodingStandard

- [#1704] Prefer IncludeFixer over LanguageConstructSpacingSniff, Thanks to [@leofeyer]

#### PackageBuilder

- [#1705] Handle single characters in the StringFormatConverter::camelCaseToGlue() method, Thanks to [@leofeyer]

#### Unknown Package

- [#1695] open to PHPStan 0.12 and Rector supporting it

### Removed

#### EasyCodingStandard

- [#1707] remove unary + not opreator non-existing conflict

#### PHPStanExtensions

- [#1706] Drop confusing path ignore

#### PackageBuilder

- [#1698] Remove dependency on symfony/debug, Thanks to [@enumag]

#### Unknown Package

- [#1696] drop unused env

## [v7.1] - 2019-12-09

### Added

#### EasyCodingStandard

- [#1690] Bump to Slevomat 6, add `dead-code` set

#### SetConfigResolver

- [#1694] add relative path for phar

### Changed

#### ChangelogLinker

- [#1687] Making URL resolver more generic, Thanks to [@jawira]

#### PHPStanExtensions

- [#1693] Upgrade to PHPStan 0.12

## [v7.0.2] - 2019-11-23

### Added

#### MonorepoBuilder

- [#1684] Add optional `--tag` input to set tag manually, Thanks to [@DayS]

### Changed

#### PHPStanExtensions

- [#1686] Make extension future compatible with prefixed everything

### Fixed

- [#1682] Windows text fixing

#### MonorepoBuilder

- [#1685] Fix option value regression

#### PackageBuilder

- [#1681] Fix kernel shutdown

## [v7.0.1] - 2019-11-23

### Added

- [#1677] Add missing composer dependency on the new package SetConfigResolver, Thanks to [@sustmi]

### Fixed

- [#1676] Test fixes

## [v7.0.0] - 2019-11-23

- [#1670] New package **SetConfigResolver**
- [#1643] New package **SmartFileSystem**

### Added

- [#1656] Add `--xdebug` option

#### ChangelogLinker

- [#1662] Make changed category as default fallback, add deprecated category

#### EasyCodingStandard

- [#1669] Drop overcomplicated `CustomSourceProviderInterface`, add `parameters > file_extensions` instead

#### MonorepoBuilder

- [#1671] Add `file://` option for repository, Thanks to [@fchris82]

### Changed

- [#1674] Allow Symfony 5
- [#1668] Bump to Symfony 4.3+
- [#1629] Allow Symfony 5 + bump to PHP 7.2 + add Rector CI run
- [#1630] Add Rector CI run
- [#1650] Travis Windows + composer paths, Thanks to [@orklah]

#### EasyCodingStandard

- [#1663] Change `--level` option to `--set`

### Removed

#### CodingStandard

- [#1667] Remove deprecated `NoClassInstantiationSniff`
- [#1675] remove deprecated classes

### Removed

#### CodingStandard

- [#1666] Remove `BlockPropertyCommentFixer` and use `PhpdocLineSpanFixer` instead

#### EasyCodingStandard

- [#1655] Add "sets" parameter for shorter imports of native configs

#### SmartFileSystem

- [#1649] Add `FileSystemGuard` and its exceptions

### Changed

- [#1650] Travis Windows + composer paths, Thanks to [@orklah]
- [#1644] travis: change to jobs

#### ChangelogLinker

- [#1645] Skip tests

#### CodingStandard

- [#1616] Improve `NoClassInstantiationSniff` + improve code complexity in ignored cases

### EasyCodingStanard

- [#1637] Only print metadata for console output, Thanks to [@ruudk]
- [#1635] Autowire `OutputFormatterInterface`, Thanks to [@ruudk]

### Fixed

- [#1623] Fix reading GIT tags in Windows OS, Thanks to [@SerafimArts]
- [#1622] Apply lowercase to compose dependencies, Thanks to [@SerafimArts]

### Removed

#### Statie

- [#1641] Drop `Latte` support to lower the complexity [BC break]
- [#1642] Change `FilterProviderInterface` to `TwigExtension` [BC break]

### Deprecated

#### CodingStandard

- [#1627] Deprecate `NoClassInstantiation` for inpractical and bloated usage

[@natepage]: https://github.com/natepage
[@jawira]: https://github.com/jawira
[#1644]: https://github.com/symplify/symplify/pull/1644
[#1643]: https://github.com/symplify/symplify/pull/1643
[#1642]: https://github.com/symplify/symplify/pull/1642
[#1641]: https://github.com/symplify/symplify/pull/1641
[#1637]: https://github.com/symplify/symplify/pull/1637
[#1635]: https://github.com/symplify/symplify/pull/1635
[#1630]: https://github.com/symplify/symplify/pull/1630
[#1629]: https://github.com/symplify/symplify/pull/1629
[#1627]: https://github.com/symplify/symplify/pull/1627
[#1623]: https://github.com/symplify/symplify/pull/1623
[#1622]: https://github.com/symplify/symplify/pull/1622
[#1616]: https://github.com/symplify/symplify/pull/1616
[@ruudk]: https://github.com/ruudk
[@SerafimArts]: https://github.com/SerafimArts
[#1656]: https://github.com/symplify/symplify/pull/1656
[#1655]: https://github.com/symplify/symplify/pull/1655
[#1650]: https://github.com/symplify/symplify/pull/1650
[#1649]: https://github.com/symplify/symplify/pull/1649
[#1645]: https://github.com/symplify/symplify/pull/1645
[@orklah]: https://github.com/orklah
[#1675]: https://github.com/symplify/symplify/pull/1675
[#1674]: https://github.com/symplify/symplify/pull/1674
[#1671]: https://github.com/symplify/symplify/pull/1671
[#1670]: https://github.com/symplify/symplify/pull/1670
[#1669]: https://github.com/symplify/symplify/pull/1669
[#1668]: https://github.com/symplify/symplify/pull/1668
[#1667]: https://github.com/symplify/symplify/pull/1667
[#1666]: https://github.com/symplify/symplify/pull/1666
[#1663]: https://github.com/symplify/symplify/pull/1663
[#1662]: https://github.com/symplify/symplify/pull/1662
[@fchris82]: https://github.com/fchris82
[#1694]: https://github.com/symplify/symplify/pull/1694
[#1693]: https://github.com/symplify/symplify/pull/1693
[#1690]: https://github.com/symplify/symplify/pull/1690
[#1687]: https://github.com/symplify/symplify/pull/1687
[#1686]: https://github.com/symplify/symplify/pull/1686
[#1685]: https://github.com/symplify/symplify/pull/1685
[#1684]: https://github.com/symplify/symplify/pull/1684
[#1682]: https://github.com/symplify/symplify/pull/1682
[#1681]: https://github.com/symplify/symplify/pull/1681
[#1677]: https://github.com/symplify/symplify/pull/1677
[#1676]: https://github.com/symplify/symplify/pull/1676
[v7.0.2]: https://github.com/symplify/symplify/compare/v7.0.1...v7.0.2
[v7.0.1]: https://github.com/symplify/symplify/compare/v7.0.0...v7.0.1
[@sustmi]: https://github.com/sustmi
[@DayS]: https://github.com/DayS
[v7.0.0]: https://github.com/symplify/symplify/compare/v6.1.0...v7.0.0
[#1726]: https://github.com/symplify/symplify/pull/1726
[#1724]: https://github.com/symplify/symplify/pull/1724
[#1723]: https://github.com/symplify/symplify/pull/1723
[#1722]: https://github.com/symplify/symplify/pull/1722
[#1720]: https://github.com/symplify/symplify/pull/1720
[#1718]: https://github.com/symplify/symplify/pull/1718
[#1717]: https://github.com/symplify/symplify/pull/1717
[#1716]: https://github.com/symplify/symplify/pull/1716
[#1715]: https://github.com/symplify/symplify/pull/1715
[#1713]: https://github.com/symplify/symplify/pull/1713
[#1711]: https://github.com/symplify/symplify/pull/1711
[#1710]: https://github.com/symplify/symplify/pull/1710
[#1708]: https://github.com/symplify/symplify/pull/1708
[#1707]: https://github.com/symplify/symplify/pull/1707
[#1706]: https://github.com/symplify/symplify/pull/1706
[#1705]: https://github.com/symplify/symplify/pull/1705
[#1704]: https://github.com/symplify/symplify/pull/1704
[#1698]: https://github.com/symplify/symplify/pull/1698
[#1696]: https://github.com/symplify/symplify/pull/1696
[#1695]: https://github.com/symplify/symplify/pull/1695
[#1692]: https://github.com/symplify/symplify/pull/1692
[v7.1.3]: https://github.com/symplify/symplify/compare/v7.1.2...v7.1.3
[v7.1.2]: https://github.com/symplify/symplify/compare/v7.1.1...v7.1.2
[v7.1.1]: https://github.com/symplify/symplify/compare/v7.1...v7.1.1
[v7.1]: https://github.com/symplify/symplify/compare/v7.0.2...v7.1
[@schrapel]: https://github.com/schrapel
[@ltribolet]: https://github.com/ltribolet
[@leofeyer]: https://github.com/leofeyer
[@enumag]: https://github.com/enumag
[@Rarst]: https://github.com/Rarst
[#1737]: https://github.com/symplify/symplify/pull/1737
[#1735]: https://github.com/symplify/symplify/pull/1735
[#1734]: https://github.com/symplify/symplify/pull/1734
[#1731]: https://github.com/symplify/symplify/pull/1731
[#1728]: https://github.com/symplify/symplify/pull/1728
[v7.2.0]: https://github.com/symplify/symplify/compare/v7.1.3...v7.2.0
[#1773]: https://github.com/symplify/symplify/pull/1773
[#1772]: https://github.com/symplify/symplify/pull/1772
[#1771]: https://github.com/symplify/symplify/pull/1771
[#1768]: https://github.com/symplify/symplify/pull/1768
[#1767]: https://github.com/symplify/symplify/pull/1767
[#1762]: https://github.com/symplify/symplify/pull/1762
[#1760]: https://github.com/symplify/symplify/pull/1760
[#1759]: https://github.com/symplify/symplify/pull/1759
[#1756]: https://github.com/symplify/symplify/pull/1756
[#1755]: https://github.com/symplify/symplify/pull/1755
[#1751]: https://github.com/symplify/symplify/pull/1751
[#1748]: https://github.com/symplify/symplify/pull/1748
[#1747]: https://github.com/symplify/symplify/pull/1747
[#1745]: https://github.com/symplify/symplify/pull/1745
[#1741]: https://github.com/symplify/symplify/pull/1741
[#1740]: https://github.com/symplify/symplify/pull/1740
[#1739]: https://github.com/symplify/symplify/pull/1739
[v7.2.2]: https://github.com/symplify/symplify/compare/v7.2.1...v7.2.2
[v7.2.1]: https://github.com/symplify/symplify/compare/v7.2.0...v7.2.1
[@ondraondra81]: https://github.com/ondraondra81
[@migrify]: https://github.com/migrify
[#1776]: https://github.com/symplify/symplify/pull/1776
[#1774]: https://github.com/symplify/symplify/pull/1774
