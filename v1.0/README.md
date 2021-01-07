## Data Description

## Notes
- All flux densities are given in units of ``mJy`` (AB zeropoint = 16.4).
- Missing data/parameter are indicated with ``-99``.

## Columns


|                   *Column*     | *Unit* |                                                                                       *Description* |
|     :--------------------:     | :--------------------:    |                                                       :------------------------------------------- |
|                                |  |                                                                                                     |
|                         ``ID`` | |ID of the object from the parent catalogue                                             |
|                          ``RA`` | deg | The Right Ascension coordinate as given in the parent catalogue                                      |
|                          ``DEC`` | deg |  The declination, in equatorial coordinate epoch J2000                                             |
|                          ``Area`` | bool |   Same as **goodArea** flag in the parent catalogues. Denotes region with reliable photometry.    |
|                          ``z`` |   |  Redshift used for fitting                                                                          |
|                          ``ztype`` |  |   Redshift type flag. Spectroscopic=1, photometric=0                                               |
|                          ``LIR_total`` | Lsol  |  Total FIR luminosity, obtained as the sum between AGN and DL07 components                |
|                          ``eLIR_total`` | Lsol |   Uncertainty on the total FIR luminosity                                                 |
|                          ``Lagn`` | Lsol  |  AGN luminosity                |
|                          ``eLagn`` | Lsol |   Uncertainty on the AGN luminosity                                                 |
|                          ``Lir_draine`` | Lsol  |  Luminosity given by the DL07 template                |
|                          ``eLir_draine`` | Lsol |   Uncertainty on the luminosity given by the DL07 template                                                 |
|                          ``MD`` | Msol |   Dust mass as predicted by the best-fit DL07 template |
|                          ``eMD`` | Msol |   Uncertainty on the dust mass                                              |
|                          ``deltaGDR`` |  |   Gas-to-dust ratio                                              |
|                          ``MG`` | Msol |   Gas mass computed from deltaGDR and MD                                              |
|                          ``eMG`` | Msol |   Uncertainty on the gas mass                                             |
|                          ``Mstar`` | Msol |   Stellar mass, equal to the one in the parent catalogue                                             |
|                          ``lastdet`` | micron  |   Last band that has a S/N>3 detection.  Given in rest frame                                               |
|                          ``chi2`` |  |   Goodness of fit per degree of freedom.                                               |
|                          ``f_agn`` |  |   AGN fraction                                               |
|                          ``efagn`` |  |   Uncertainty on the AGN fraction                                               |
