Change Log
----------

**2.1.1**

- Added ``dmyformat()`` to return dates in DD/MM/YYYY format.
- Deprecated ``slashformat()`` method to be replaced by ``dmyformat()`` method.
- Fixed PyPI package not including a required file. Issue `#3 <https://github.com/dralshehri/hijri-converter/issues/3>`__ by `@PureTryOut <https://github.com/PureTryOut>`__.
- Fixed some typos.
- Updated tests.

**2.1.0**

This version has more accurate conversion and better internal code.
Details are as follows:

- Dropped support for the years before 1343 AH because the Umm al-Qura calendar
  was not established then.
- Added ``validate`` parameter to Hijri object for optional disabling of
  Hijri date validation and improving performance.
- Verified conversion against original references and updated the
  ``month_starts`` tuple for more accurate conversion.
- Improved ``Hijri`` object rich comparison methods.
- Improved date validation methods for better performance and readability.
- Made the ``Hijri`` object hashable by adding a custom ``__hash__`` method.
- Refactored many internal methods (not affecting the API).
- Other minor fixes, enhancements and performance boost.

**2.0.0**

In short, this version supports only lunar Hijri calendar on Python 3.6+, and
the conversion is in complete agreement with the official Umm al-Qura calendar.
Details are as follows:

- Renamed the package to ``hijri-converter``.
- Dropped support for the solar Hijri calendar.
- Dropped support for Python 3.5.
- Refactored localization and ``ummalqura.py`` module.
- Updated ``month_starts`` tuple in alignment with the Umm al-Qura calendar.
- Added ``fromdate()`` classmethod to ``Gregorian`` object.
- Added ``notation()`` method to ``Hijri`` and ``Gregorian`` objects.
- Added more methods to ``Gregorian`` object including ``slashformat()``,
  ``month_name()``, ``day_name()`` and ``to_julian()``.
- Renamed ``month_days()`` method of ``Hijri`` object to ``month_length()``.
- Changed formatted string to use f-strings.
- Improved documentation and examples.
- Updated unit tests.
- Fixed other minor issues and typos.

**1.5.0**

- Added ``fromisoformat()`` classmethod to ``Hijri`` object.
- Added support for rich comparison between Hijri dates.
- Updated documentation and testing code.
- Other minor fixes and enhancements.

**1.4.0**

- Refactored conversion methods to improve performance.
- Changed date validation back to be the default and removed optional parameter.
- Added ``to_julian()`` method to ``Hijri`` object.
- Updated documentation and testing code.
- Other minor fixes and enhancements.

**1.3.3**

- Fixed a bug in range validation for the Gregorian date.
- Changed generic typing to built-in types.
- Added more tests to cover the solar calendar.
- Improved code structure and documentation.

**1.3.2**

- Improved documentation and changelog.

**1.3.1**

- Fixed README file.

**1.3.0**

- Added documentation directory with an online version.
- Changed date input validation to be optional and disabled by default.
- Improved code readability and performance.
- Other minor fixes and enhancements.

**1.2.0**

- Added ``slashformat()`` method to ``Hijri`` object.
- Improved date validation code.
- Fixed some typos in documentation and docstrings.

**1.0.1**

- Improved examples and documentation.

**1.0.0**

- First release.
