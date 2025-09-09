# CloudCal-XL5

Unofficial fork of CloudCal, adapted for Thermo Scientific Niton XL5 analyzers. Not affiliated with the original maintainers.


>**Repository:** cloudCal-XL5-fork<br>
>**Upstream project:** CloudCal (GPL-3.0)<br>
>**License:** GPL-3.0

---

## How to use

* Website: 
* Containers (Docker Hub): 

> Local install instructions may be added later.

---

## What is this fork?

cloudCal-XL5 is an unofficial fork of the CloudCal app tailored for Thermo Scientific Niton XL5 pXRF workflows. It is designed to interoperate with [TropiCal](https://github.com/dannilocruz/TropiCal):

* TropiCal exports XL5 raw spectra (with metadata),
* cloudCal‑XL5 builds empirical calibrations and produces `.quant` files, and
* TropiCal uses `.quant` to quantify raw XL5 spectra (exporting majors as oxides wt% and traces in ppm).

### Key additions in this fork

* XL5 I/O: readers/writers and handlers for Niton XL5 outputs.
* TropiCal compatibility: accepts TropiCal raw spectra and produces `.quant` files for TropiCal to use.
* Bugfixes & ergonomics specific to XL5 datasets.

> This is not an official release of CloudCal. Please file issues here (not in the upstream repo) for XL5/TropiCal‑specific behavior.

---

## How the calibration works (brief)

Calibrations follow the Lucas–Tooth and Price approach used by CloudCal. You can also choose alternative linear/nonlinear models as supported by CloudCal.

---

## Supported input/output

Everything CloudCal supports plus the XL5/TropiCal pathway:

* Inputs supported by CloudCal (upstream): `.csv` from S1PXRF; PDZ v24/v25; `.spx`; Elio `.spt`; `.mca`; Artax net‑counts `.csv`.
* XL5 / TropiCal workflow:

  * Input: XL5 raw spectra exported by TropiCal (with metadata).
  * Output: `.quant` calibration files produced by cloudCal‑XL5, which TropiCal uses for empirical quantification.

---

## Related repositories

* CloudCal (upstream): [https://github.com/leedrake5/CloudCal](https://github.com/leedrake5/CloudCal)
* CloudCal‑XL5‑fork (this repo for `.quant` creation): [https://github.com/dannilocruz/CloudCal-XL5-fork](https://github.com/dannilocruz/CloudCal-XL5-fork)
* TropiCal (companion app): [https://github.com/dannilocruz/TropiCal](https://github.com/dannilocruz/TropiCal)

---

## Citing

If you use this fork, please cite both the upstream CloudCal and this fork:

* CloudCal: Drake, B.L. 2018. *CloudCal v3.0*. GitHub. doi: 10.5281/zenodo.2596154.
* This fork: cloudCal‑XL5-fork, version/tag, GitHub: 

---

## License

This repository is distributed under GPL‑3.0, the same license as CloudCal.

* Original copyright and license notices are preserved.

See `LICENSE` for details.

---

## Acknowledgments

* CloudCal creators and contributors for the original project.
* Users and collaborators providing XL5 datasets and feedback.

---

## Contributing & Support

This is an unofficial fork. For XL5/TropiCal‑specific issues and enhancements, please use this repository’s Issues. For (non‑XL5) concerns, refer to the original CloudCal project.
