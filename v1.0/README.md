## Data Description

## Notes
- All flux densities are given in units of ``mJy`` (AB zeropoint = 16.4).
- Missing data/parameter are indicated with ``-99``.

## Columns


|                   *Column*     | *Unit* |                                                                                       *Description* |
|     :--------------------:     | :--------------------:    |                                                       :------------------------------------------- |
|                                |  |                                                                                                     |
|                         ``ID`` | -|ID of the object from the parent catalogue                                             |
|                          ``RA`` | deg | The Right Ascension coordinate as given in the parent catalogue                                      |
|                          ``DEC`` | deg |  The declination, in equatorial coordinate epoch J2000                                             |
|                          ``Area`` | bool |   Same as **goodArea** flag in the parent catalogues. Denotes region with reliable photometry    |
|                          ``z`` | -  |  Redshift used for fitting                                                                          |
|                          ``ztype`` | bool  |   Redshift type flag. Spectroscopic=1, photometric=0                                               |
|                          ``LIR_total`` | Lsol  |  Total FIR luminosity, obtained as the sum between AGN and DL07 components                |
|                          ``eLIR_total`` | Lsol |   Uncertainty on the total FIR luminosity                                                 |
|                          ``Lagn`` | Lsol  |  AGN luminosity                |
|                          ``eLagn`` | Lsol |   Uncertainty on the AGN luminosity                                                 |
|                          ``Lir_draine`` | Lsol  |  Luminosity given by the DL07 template                |
|                          ``eLir_draine`` | Lsol |   Uncertainty on the luminosity given by the DL07 template                                                 |
|                          ``MD`` | Msol |   Dust mass as predicted by the best-fit DL07 template |
|                          ``eMD`` | Msol |   Uncertainty on the dust mass                                              |
|                          ``deltaGDR`` | - |   Gas-to-dust ratio                                              |
|                          ``MG`` | Msol |   Gas mass computed from deltaGDR and MD                                              |
|                          ``eMG`` | Msol |   Uncertainty on the gas mass                                             |
|                          ``Mstar`` | Msol |   Stellar mass, equal to the one in the parent catalogue                                             |
|                          ``lastdet`` | micron  |   Last band that has a S/N>3 detection.  Given in rest frame                                               |
|                          ``chi2`` |-  |   Goodness of fit per degree of freedom.                                               |
|                          ``f_agn`` |-  |   AGN fraction                                               |
|                          ``efagn`` |-  |   Uncertainty on the AGN fraction                                               |
|                          ``fgas`` |-  |   Gas fraction computed as MG/MD                                              |
|                          ``fgas_FMR`` |-  |   Gas fraction computed assuming that MG=100xMD                                              |
|                          ``Lir_med`` |Lsol | Total FIR luminosity, computed from the chi2 distribution                                               |
|                          ``eLir68`` |Lsol |     Uncertainty on the total FIR luminosity, computed as the 68 % confidence interval                    |
|                          ``Mdust_med`` |Msol |  Dust mass, computed from the chi2 distribution                                              |
|                          ``eMdust68`` |Msol |   Uncertainty on the dust mass, computed as the 68 % confidence interval                      |
|                          ``Umin`` | |  Best fit Umin                                               |
|                          ``qpah`` |index |  Index of the best fit qpah value                                               |
|                          ``gamma`` | |    Best fit gamma                                             |
|                          ``U`` |Lsol/Msol |  Average radiation field intensity, computed as LIR_total/(125xMD)                                               |
|                          ``sU`` |Lsol/Msol |   Uncertainty on the average radiation field intensity                                              |
|                          ``deltaMS`` | |   SFR/SFR_ms where SFR=LIR_draine*10^-10 and SFR_ms is given by [Schreiber+15](https://ui.adsabs.harvard.edu/abs/2015A%26A...575A..74S/abstract)                                             |
|                          ``e_deltaMS`` | |    Uncertainty on deltaMS                                             |
|                             **IR PHOTOMETRY** | mJy|   IR bands from [Liu+18](https://ui.adsabs.harvard.edu/abs/2018ApJ...853..172L/abstract) and [Jin+18](https://ui.adsabs.harvard.edu/abs/2018ApJ...864...56J/abstract)                                          |
| **Opcially derived parameters** | | Quantities contained in these columns are not yet well tested, use at your own risk                   | 
|''mass''|Msol| Stellar mass computed by Stardust|
|''e_mass''|Msol| Uncertainty on the stellar mass computed by Stardust|
|''mass_K''|Msol| Stellar mass computed via the rest-frame K-band luminosity with M/L=0.6|
|''nfilt''| - | Number of bands used in fitting, this includes upper limits too|
|''sfr_opt''| Msol/year | Unobscured star-formation rate, derived via optical photometry|
|''Av''| - | V-band attenuation|
