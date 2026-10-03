# DM42 Numerical Integration Handbook

A practical, evidence-based guide to numerical integration on the SwissMicros DM42, covering `∫f(x)`, `ACC`, accuracy checks, failure modes, and scientific and engineering applications.

[Download the handbook (PDF)](./DM42_Numerical_Integration_Handbook.pdf)

## About the handbook

The **DM42 Numerical Integration Handbook** explains how to formulate, evaluate, test, and defend numerical integrals on the DM42. It develops the subject from signed area and accumulated quantities through accuracy control, difficult integrands, numerical diagnostics, transformations, and advanced applied models.

This is not a general owner's manual or a general programming manual. It focuses on the reasoning and calculator workflow needed to obtain trustworthy integrals: define the accumulated quantity, choose the variable and limits, establish the integrand and its units, predict the result's sign and scale, select a meaningful `ACC`, inspect both returned registers, and verify the answer independently.

## Contents

- **Part I — What Integration Means**: accumulated quantities, signed area, dimensional sense, and physical interpretation.
- **Part II — How Numerical Integration Works**: quadrature, approximation error, convergence, and the limits of numerical evidence.
- **Part III — The DM42 Integration Application and `ACC`**: integrand programs, limits, accuracy settings, the returned integral in `X`, and the uncertainty estimate in `Y`.
- **Parts IV–VII — First, Applied and Intermediate Integrals**: fully worked examples that build reliable calculator technique.
- **Parts VIII–XII — Numerical Strategy and Failure Modes**: interval splitting, cancellation, discontinuities, singularities, improper integrals, oscillation, narrow peaks, and misleading convergence.
- **Parts XIII–XVI — Advanced and Extreme Applications**: demanding scientific and engineering models, transformations, convergence experiments, and defensible reporting.
- **Appendices A–M**: quick reference material, templates, diagnostics, constants, notation, troubleshooting, glossary, and bibliography.

The examples span mathematics, physics, astrophysics, electronics, chemistry, biology, probability, finance, logistics, and engineering.

## Keystroke notation

The handbook distinguishes between calculator keys, menu choices, typed names, displayed results, and stored program instructions:

| Form | Meaning |
| --- | --- |
| `[KEY]` | Physical key or named shifted function |
| `{SOFT}` | Soft-key label currently shown on the display |
| `⟨TEXT⟩` | Literal alpha text followed by `ENTER` |
| `→` | Continue to the next action; not a calculator instruction |
| `display: …` | Expected text or value on the calculator display |
| `01 instruction` | Stored program line exactly as listed |

In Program mode, ordinary instructions are entered with their physical keys or menu soft keys. Pressing `[XEQ]` creates an actual `XEQ` instruction, so it is used only when a program must call a labelled routine or subroutine.

## The working discipline

1. Name the quantity being accumulated.
2. Choose the integration variable and differential.
3. Write the integrand and state its units.
4. Choose finite limits and inspect the interval for poles, jumps, peaks, oscillation, and cancellation.
5. Estimate the expected sign and order of magnitude.
6. Choose `ACC` to match the quality of the input data and the purpose of the calculation.
7. Run `∫f(x)`, read the integral from `X`, and inspect the uncertainty estimate in `Y`.
8. Repeat with a tighter `ACC` and split the interval where appropriate.
9. Verify independently and report only meaningful digits.

## Using the handbook

1. Download or open [`DM42_Numerical_Integration_Handbook.pdf`](./DM42_Numerical_Integration_Handbook.pdf).
2. Work through Parts I–IV in order if numerical integration or the DM42 integration application is new to you.
3. Enter the early examples exactly as shown, including the integrand program, variable, limits, and `ACC` setting.
4. Compare `X` and `Y` across repeated runs; do not accept a result merely because the calculator returned one.
5. Use interval splitting, transformed variables, convergence tests, and independent high-precision checks for difficult or consequential integrals.
6. Keep the appendices nearby as a quick reference when building your own models.

## Contributing

Corrections and improvements are welcome. When reporting a problem, please include:

- the PDF page and section;
- the integrand, limits, and `ACC` setting;
- the program line or keystroke sequence involved;
- the values returned in `X` and `Y`;
- the expected or independently verified result; and
- the calculator firmware version, when relevant.

Please use an issue for isolated corrections and a pull request for proposed file changes.

## Disclaimer

This is an independent, unofficial educational resource. It is not affiliated with or endorsed by SwissMicros. Product and company names belong to their respective owners. Numerical examples should be independently checked before being used for consequential engineering, financial, scientific, or safety-related work.
