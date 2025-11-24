Project Statement: Command-Line Currency Converter

Problem Statement

Many users occasionally need a quick, distraction-free way to perform simple currency conversions without the overhead of web browsers, advertisements, or complex user interfaces. The goal is to provide a fast, accessible, and self-contained command-line utility for instantaneous currency conversion that can be executed in any terminal environment with Python installed.

Scope of the Project

The project is scoped to a minimal, client-side Python script with no external dependencies (beyond standard Python libraries). It focuses solely on the core conversion calculation functionality.

In Scope:

Interactive command-line interface (CLI) for user input.

Validation of numerical amounts and currency codes.

Mathematical calculation of conversions between supported mock currencies.

Clear display of the exchange rate and final converted amount.

Out of Scope (Future Enhancements):

Fetching real-time rates from an external API (requires the requests library).

Saving or loading conversion history.

Graphical User Interface (GUI).

Support for cryptocurrencies.

Target Users

Developers/System Administrators: Users who primarily work in terminal environments and need a quick utility.

Students: Learning basic programming concepts and mathematical logic applications in Python.

Anyone requiring a simple, immediate conversion tool without internet connectivity (assuming the rates are acceptable for the task).

High-Level Features

Core Conversion: Convert Amount A (Currency 1) to Amount B (Currency 2) using fixed, mock rates.

Rate Display: Explicitly show the calculated exchange rate for the pair.

Support: List all supported currency codes upon startup.
