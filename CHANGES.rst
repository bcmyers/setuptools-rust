CHANGES
^^^^^^^

0.10.0 (2018-05-06)
------------------

- This release significantly improves performance


0.9.2 (2018-05-11)
------------------

- Fix `build_rust` crashing on `Cargo.toml` manifests without a `name` key in the `[lib]` section
- Fix single quotes not being handled when parsing `Cargo.toml`


0.9.1 (2018-03-22)
------------------

- Remove unicode_literals import as Python 2 ``distutils`` does not support Unicode


0.9.0 (2018-03-07)
------------------

- Find inplace extensions and automatically generate ``Cargo.toml`` manifests #29


0.8.4 (2018-02-27)
------------------

- Improve compatibility of `build_rust` with `build_ext` #28


0.8.3 (2017-12-05)
------------------

- Ignore strip option when platform is win32 #26


0.8.2 (2017-09-08)
------------------

- Fix script generation for bdist_wheel


0.8.1 (2017-09-08)
------------------

- Added `native` parameter

- Fix script generation for executables


0.8.0 (2017-09-05)
------------------

- Support multiple rust binaries #24


0.7.2 (2017-09-01)
------------------

- Generate console-script for Binding.Exec #22

- Do not run `cargo check` for `sdist` command #18

- Remove extra python3 file extension for executables.


0.7.1 (2017-08-18)
------------------

- Allow to strip symbols from executable or dynamic library.

- Use PyO3 0.2 for example.


0.7.0 (2017-08-11)
------------------

- Allow to build executable and pack with python package.

- Use PyO3 0.1 for example.


0.6.4 (2017-07-31)
------------------

- `check` command respects `optional` option
- Don't fail when Rust isn't installed while all extensions are optional

0.6.3 (2017-07-31)
------------------

- Fix pypi source distribution

0.6.2 (2017-07-31)
------------------

- Add `optional` option to `RustExtension` #16

0.6.1 (2017-06-30)
------------------

- Support `CARGO_TARGET_DIR` variable #14


0.6.0 (2017-06-20)
------------------

- Add support for PyO3 project https://github.com/PyO3/PyO3

- Add support for no-binding mode


0.5.1 (2017-05-03)
------------------

- Added support for "cargo test"

- Fixed unbound method type error #4


0.5.0 (2017-03-26)
------------------

- Added support for "cargo check"


0.4.2 (2017-03-15)
------------------

- Added "--qbuild" option for "build_rust" command.
  Set "quiet" mode for all extensions.

- Added "--debug" and "--release" options for "build_rust" command.


0.4.1 (2017-03-10)
------------------

- Fixed cargo manifest absolute path detection


0.4 (2017-03-10)
----------------

- Fixed bdist_egg and bdist_wheel support

- setuptool's clean command cleans rust project as well

- Use absolute path to cargo manifest

- Enable debug builds for inplace builds, otherwise build release

- Simplify monkey patches


0.3.1 (2017-03-09)
------------------

- Fix compatibility with some old versions of setuptools


0.3 (2017-03-09)
----------------

- Fixed OSX extension compilation

- Use distutils exceptions for errors

- Add rust version check for extension

- Cleanup example project


0.2 (2017-03-08)
----------------

- Fix bdist_egg and bdist_wheel commands


0.1 (2017-03-08)
----------------

- Initial release
