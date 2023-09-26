# Space-Detector-Laboratory
## Introduction

Gamma-ray astronomy is the study of astrophysical objects via the detection of their energetic photons,
which can range from 10 keV to hundreds of GeV in energy. Energies below 10 keV are generally described
as being x-rays.
In order to efficiently detect γ-ray emission from these astrophysical sources, the correct scintillator
and/or detector combination needs to be used, as each detector is sensitive over a particular part of the
electromagnetic spectrum, with a quantum efficiency that varies with respect to energy.
The experiment follows the pre-flight tests performed on the detectors for the Fermi Burst Alert Telescope, documented in Bissaldi et al. [2009]. 

## 1] Detectors

The four detectors are:

• a Hyper-Pure Germanium detector (HPGe);

• a Cadmium Telluride detector (CdTe);

• a Thallium-doped Sodium Iodide detector (NaI:Tl);

• a Bismuth Germanate detector (BGO).

Each detector measures the energy deposited by each incident photon. It does this by using the deposited
energy to excite electrons within the crystal structure. The detector converts these excited electrons into
an electrical signal, which is measured and digitised. Since the number of electrons increases with the
amount of energy deposited in the detector, the size of this response measures the energy deposited by
the gamma ray.
For each incoming photon, the output from the detector is digitised. This adds a count into the appro-
priate digital energy channel. Once many gamma-rays have entered the detector and deposited (some or
all of) their energy, the resulting spectrum consists of the number of counts in each channel.
These four represent two types of gamma-ray detector, which are distinguished by how they convert
excited electrons into an electrical output:

• HPGe & CdTe are solid state detectors. These directly detect the energy absorbed from ionising
radiation as an electrical current generated when the high energy photon deposits energy and
excites electrons into the conduction band.

• NaI & BGO are scintillator detectors. These detector crystals absorb high-energy photons and re-
emit low-energy photons at visible wavelengths. A photomultiplier (usually a photomultiplier tube
(PMT)) is used to convert this light into an electrical signal that can be amplified and digitised.


## 2] Radioactive Sources

Pre-calibrated radioactive sources have been used to determine the lab detectors' spectral response.
Two examples are 241Am and 60Co:

• 241Am has a half-life of ∼432 years, and decays to 237Np via emission of an alpha particle (42He).
In doing so, it populates excited levels in 237Np, one of which is the 52
− at an excitation energy of 59.5 keV. After 67 ns, this level then decays to the ground state of 237Np via emission of a 59.5 keV X-ray.


• 60Co has a half-life τ 12 ≃ 5yr, and decays via β−-decay. This results in the population of the 4+ excited state in 60Ni, which promptly undergoes a quick cascade to the ground state in this stable nucleus, via emission of two gamma rays, with energies of 1173.2 keV and 1332.5 keV respectively.


## 3] Calibration & Characterisation of High Energy Detectors

• The spectral data consists of channels and counts. so must calibrate the energy response
of each detector.

• it must be characterised the performance of each detector so you can compare and contrast the 4 detectors, their similarities, differences, and strengths and
weaknesses.

For this purpose, the following are necessary:

– the energy resolution as a function of energy;

– the absolute and intrinsic efficiencies as a function of energy;

– the off-axis performance of the detector (eg., efficiency vs angle).

To do this, it has been necessary to develop an appropriate set of data analysis pipelines. This means a set of scripts that take as inputs the spectral files and appropriate configuration information, and output the appropriately analysed data products, including tables and graphs.



