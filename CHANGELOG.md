## Changelog

#### 0.19.2 (2014-07-29)

* Remove the `Base.Ord` constraint from `Ord` so new Ord instances can be added. Note that you cannot use a custom implementation of the methods, JavaScript's native operators are used for comparisons.

#### 0.19.1.2 (2014-04-29)

* Allow `fay 0.20`

#### 0.19.1.1 (2014-04-07)

* Fix compilation on GHC 7.8

### 0.19.1 (2014-03-13)

* Add Data.Char

## 0.19 (2014-01-14)

* Ord instance for Integer
* Export base versions of Maybe, Ordering, and Either instead of redefining when compiling with GHC. This helps when writing libraries targeting both Fay and GHC
* `Prelude`: Add `void`, `>=>` and `<=<`, `unless`, `forM`, `mapM`
* Add `Debug.Trace` module exporting `trace` and `traceShow`

Minor:
* Upper bound to the latest major Fay version

## 0.18.0.0 (2013-09-24)

* Fixed implementation of `>>` and `>>=` (this bug didn't affect normal usage)
* Add `fail`
* Generalize type signatures for `fromIntegral` and `fromInteger`


## 0.17.0.0 (2013-08-27)

* The type signature of `FFI.ffi` has been generalized to `IsString s => s -> a` to support `RebindableSyntax`.
* Prelude now exports `ifThenElse` as a default for `RebindableSyntax`


## 0.16.0.0 (2013-08-05)

* Added more Ratio functions and move them all into Data.Ratio
