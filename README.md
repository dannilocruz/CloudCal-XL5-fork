# CloudCal-XL5

Unofficial fork of [CloudCal](https://github.com/leedrake5/CloudCal) tailored for for Thermo Scientific™ Niton™ XL5 Plus handheld analyzers.<br>
Not affiliated with or endorsed by Thermo Fisher Scientific.


>**Repository:** CloudCal-XL5-fork<br>
>**Upstream project:** CloudCal (GPL-3.0)<br>
>**License:** GPL-3.0

---

## How to use

* Website: https://cloudcalxl5.danilocruz.earth
* Containers (Docker Hub): [dannilocruz/cloudcal-xl5-fork](https://hub.docker.com/repository/docker/dannilocruz/cloudcal-xl5-fork/general)

---

## What CloudCal-XL5 does

CloudCal-XL5 is designed to interoperate with [TropiCal](https://github.com/dannilocruz/TropiCal):

* TropiCal exports XL5 raw spectra (with metadata),
* cloudCal‑XL5 builds empirical calibrations and produces `.quant` files, and
* TropiCal uses `.quant` to quantify raw XL5 spectra (exporting majors as oxides wt% and traces in ppm).

## Key additions in this fork

* XL5 I/O: readers/writers and handlers for Niton XL5 outputs.
* TropiCal compatibility: accepts TropiCal raw spectra and produces `.quant` files for TropiCal to use.
* Bugfixes & ergonomics specific to XL5 datasets.

---

## How the calibration works (brief)

Calibrations follow the Lucas–Tooth and Price approach used by CloudCal. You can also choose alternative linear/nonlinear models as supported by CloudCal.

---

## Supported input/output

Everything CloudCal supports plus `.csv` files from TropiCal:

---

## Related repositories

* TropiCal (companion app): [https://github.com/dannilocruz/TropiCal](https://github.com/dannilocruz/TropiCal)

---

## Citing

If you use this fork, please cite both CloudCal and CloudCal-XL5:

* CloudCal: Lee Drake. (2019). leedrake5/CloudCal: Neural Networks (v3.0). Zenodo. https://doi.org/10.5281/zenodo.2596154
* Cruz, D. J. N. (2025). CloudCal-XL5 (v1.0). Zenodo. https://doi.org/10.5281/zenodo.17137170

---

## License

This repository is distributed under GPL‑3.0, the same license as CloudCal.

* Original copyright and license notices are preserved.

See `LICENSE` for details.

---

## Contributing & Support

This is an unofficial fork. For XL5/TropiCal‑specific issues and enhancements, please use this repository’s Issues. For (non‑XL5) concerns, refer to the original CloudCal project.

## Disclaimer

- CloudCal-XL5 is provided “as is” without warranty of any kind, express or implied. It is intended for research and educational use.
- CloudCal-XL5 is not affiliated with or endorsed by Thermo Fisher Scientific. *Thermo Scientific™* and *Niton™* are trademarks of Thermo Fisher Scientific and its affiliates, used here for identification only.
- CloudCal-XL5 is not affiliated with the original CloudCal maintainers.
