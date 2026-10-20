# Tracker Wave Check

Is a move between two brand-tracker waves real, or noise? Enter last wave's score and sample size, this wave's, and get a verdict.

Open `index.html` in any browser. No build step and no dependencies.

- **Inputs:** two percentages and two sample sizes, plus confidence (90/95/99%), the smallest change you would act on, how many metrics you are scanning, and a design effect for weighted samples.
- **Test:** Wilson interval per wave, combined into a range for the change with Newcombe's hybrid score method. The p-value is a pooled two-proportion z-test.
- **Many metrics:** the Sidak correction raises the bar when you scan more than one metric per wave.
- **Verdicts:** `moved`, `real, but small`, `no meaningful move`, `not proven`. "No meaningful move" is only said when the whole range sits inside what you would ignore.
- **Also shows:** the smallest move your sample could detect (80% power), the respondents per wave needed to prove the observed move, and a table of detectable moves at common sample sizes.
- **Share:** downloads a paper-ground PNG card, and the URL hash holds your numbers.

Assumes a simple random sample and covers sampling noise only. A changed panel, question wording or fieldwork window can move a score by more than this.

Checked by hand: 31% to 34% on 500 per wave gives z of about 1.01, p of about 0.31, range -2.8 to +8.8pp.

Styled to the ben.j.ads brand: paper ground, Bricolage Grotesque Condensed and Archivo (bundled in `fonts/`, SIL OFL), lime as a mark only. No external requests.

## License

Code is MIT licensed ([LICENSE](LICENSE)). The bundled fonts (Bricolage Grotesque, Archivo) are SIL OFL 1.1, with licenses in `fonts/`. The ben.j.ads wordmark and footnote mark in `logo/` are Ben Johnston's brand assets and are not covered by the MIT license.
