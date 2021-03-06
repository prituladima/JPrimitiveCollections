# Change Log
All notable changes to this project will be documented in this file.
This project does its best to adhere to [Semantic Versioning](http://semver.org/).


--------
### [0.3.0](N/A) - 2017-10-22
#### Changed
* `*List` `addAll(Collection)` renamed/changed to `addValues(Iterable)` for ease of use and renamed to avoid ambigious method definition with `addAll(*List)` (i.e. `IntList`)
* `*ArrayList` static methods `of(Collection, int)` and `toArray(Collection, int)` first parameter changed to `Iterable` for ease of use
* `*MapSorted` `putAll(Collection, Collection[, ...])` changed to `putAll(Iterable, Iterable[, ...])` for ease of use
* Some unit test additions


--------
### [0.2.1](https://github.com/TeamworkGuy2/JPrimitiveCollections/commit/24b1c88356f14fc6adf4ca8940c045783da702cd) - 2016-10-03
#### Added
* Added *List.iterator() interface method

#### Changed
* Reordered some methods in various classes/interfaces

#### Fixed
* Fixed *ArrayView.indexOf() bug


--------
### [0.2.0](https://github.com/TeamworkGuy2/JPrimitiveCollections/commit/66f5407b79b7fb4e5bc1d57c0f53dea8c8d8e22f) - 2016-10-02
Should be backward compatible with the 0.1.x, but binary compatibility of the jar may be broken due to interface changes.

#### Changed
* Added methods to *List interfaces:
  * removeRange()
  * addAll(Collection)
  * addToCollection()
  * toList()
* Added methods to *ListReadOnly interfaces:
  * average()
  * max()
  * min()
  * sum()
* Moved methods up from *List -> *ListReadOnly interfaces:
  * toList()
  * toString(Appendable)
* Expanded several generic parameter type signatures with '? extends' and '? super' for easier use
* Improved documentation and added synchronization documentation mentioning whether classes are thread safe or not
* Renamed the internal *ArrayView 'objs' field to 'values'


--------
### [0.1.3](https://github.com/TeamworkGuy2/JPrimitiveCollections/commit/1088cc8308eda64482dc9c3b5f9ece1210aa60f9) - 2016-09-10
#### Added
* Added *SortedList.binarySearch()


--------
### [0.1.2](https://github.com/TeamworkGuy2/JPrimitiveCollections/commit/cdb1aa563223728b4af283417eab8cb8f8f438ac) - 2016-08-27
#### Changed
* Updated jsimple-types dependency to latest 0.5.x version


--------
### [0.1.1](https://github.com/TeamworkGuy2/JPrimitiveCollections/commit/c8c5a0399a378cae62757f80456174c71c88759e) - 2016-06-26
#### Added
* Added lastIndexOf() to \*MapSorted, \*MapReadOnly, \*ListSorted, \*ListReadOnly, and \*Searchable

#### Changed
* Cleaned up some documentation

#### Fixed
* Bug in \*ListSorted.indexOf() not returning lowest index when multiple identical values existed in the sorted list


--------
### [0.1.0](https://github.com/TeamworkGuy2/JFileIo/commit/6c1a6738feea81c5d753ce4fc132610a28aa82fa) - 2016-06-26
#### Added
* Initial versioning of existing code
* Switched versions.md format to CHANGELOG.md, see http://keepachangelog.com/
* Moved test files to separate test/ directory
