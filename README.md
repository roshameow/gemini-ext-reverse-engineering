# Gemini CLI Extension: Formula Reverse Engineering

A specialized extension for [Gemini CLI](https://github.com/google/gemini-cli) that transforms your AI Agent into a senior data scientist capable of reverse-engineering complex, black-box scoring algorithms and mathematical models.

Instead of letting AI blindly overfit data with random polynomials or neural networks, this extension enforces a rigorous, **7-step iterative methodology**:

1. **Exploratory Fitting:** Fast correlation testing across dimensions.
2. **Isolate & Control Components:** Locking down perfectly linear/known variables to reduce dimensionality.
3. **Outlier Analysis:** Targeting max-residual data points to discover hidden logic flaws.
4. **Slicing & Segmentation:** Reconstructing true thresholds and controlling unknown variables via narrow-band slices (or zero-value slices).
5. **Polynomial Probing & Shape Guessing:** Using geometric shapes to deduce the true analytical expression (e.g., Log, Exp, Arcsinh).
6. **Fusion:** Merging segmented behaviors into unified laws.
7. **Physical Elegance:** Forcing "ugly" machine-generated decimals to snap back to the elegant integers and fractions intended by human designers.

## Installation

Install directly via Gemini CLI:

```bash
gemini ext install https://github.com/roshameow/gemini-ext-reverse-engineering
```

Then reload your skills in interactive mode:
```text
/skills reload
```

## Usage

Simply ask Gemini CLI to analyze your dataset and find the underlying formula. The Agent will automatically trigger the skill and strictly follow the 7-step expert workflow.

*Example prompts:*
- "Here is a dataset with Sharpe, Turnover, Returns, and Drawdowns, mapped to an IS Score. Reverse-engineer the scoring formula for me."
- "I have this black-box physics data. Find the elegant mathematical equation behind it using the formula-reverse-engineering skill."

## License

MIT