---
title: Release Notes
nav_order: 2
---

# Version 3.6.7

🔗 [Download](https://www.psr-inc.com/app/link/?t=d&f=nwsddp-3.6.7-setup.exe)

## Corrections

* Warns when there is modification of non-existing plant instead of showing error and interrupting the conversion.

# Version 3.6.6

## Corrections

* Registers components required during installation in order to run the program.

# Version 3.6.5

## New features

* Support for the hydrological trend file by stations (vazpast). It should be enabled through the new option “Convert hydrological trend data by station, if available”.
* Hydrological bias by REE is not supported (eafpast).

## Corrections

* Correction in the format of the interconnection registration data.

# Version 3.6.4

## New features

* Adds to the registration modification file format (MDC) a field for the cost of curtailment of renewables. Standard value of R$ 100.00.
* Option enabled by default: Use Newave penalty data.

## Corrections

* Minimum thermal generation no longer modeled as a generation constraint. Reverts what's new in version 3.5.30.
* Adds interconnection and interconnection sum modification for the first month of the study.

# Version 3.6.3

## Corrections

* Corrects sense of capabilities in interconnect modification data.

# Version 3.6.2

## Corrections

* Fixes rounding error to prevent the historical unavailability factor from being greater than the forced one.
* Updates name of minimum generation constraints of plants with the name of the plant.

# Version 3.6.1

## Corrections

* Correction in additional data from hydroelectric plants that prevented running the simulation in SDDP 17.
* Updated default run options to SDDP 17.

# Version 3.6.0

## New features

* Data format update to SDDP 17.

# Version 3.5.30

## New features

* Minimum thermal generation represented as generation constraint (SDDP 17).

## Corrections

* Correction in the registration data and modification of thermal plants.

# Version 3.5.29

## Corrections

* Correction in writing generation restrictions for more than one system.
* Adds negative estimated reservoir area warning (PMO 08/2021).

# Version 3.5.28

## Corrections

* Fixed REE conversion in SDDP Reservoir Sets.
* Correction in the minimum generation data to consider programmed unavailability modification.

# Version 3.5.27

## New features

* Converts REE to SDDP Reservoir Pools.
* Adds new SDDP 17 compliant option to convert REE risk aversion curve data into Reservoir Set Alert Energy Constraint with % data.
  * Enable “Convert CAR to Reservoir Set Constraints” to use the feature.

# Version 3.5.26

## Corrections

* Correction in the reading of the initial volume by subsystems.
* Correction in handling penalties when REE does not exist.

# Version 3.5.25

## Corrections

* Ignores non-existent interchanges in interchange grouping data.
* Enlarges dimensions of the options screen.

# Version 3.5.24

## New features

* Option to consider Newave's minimum generation constraint penalty.

## Corrections

* Correction in reading Newave's penalty data.


# Version 3.5.23

## New features

* Option to use the maximum flow from the history in the definition of the table height x defluence of the tailrace channel (enabled by default).

## Corrections

* Improvement in the calculation of the table x elevation deflects the tailrace, avoiding decreasing elevation values.
* Correction in the handling of the minimum generation constraint.

# Version 3.5.22

## New features

* Block `VERTMN` of the MDC to define minimum spillage for hydroelectric plants (SDDP 16).
* MDC for PMO 2021-02 without using dummy plants to model spillage.

## Corrections

* Correction in the treatment of Angra's minimum generation constraint (PMO 2021-01).

# Version 3.5.21

## Corrections

* Correction in reading Newave thermal class modification data (PMO 2021-01).

# Version 3.5.20

## Corrections

* Correction of the calculation of the minimum generation of thermal plants, where negative values close to zero could appear due to truncation errors.

# Version 3.5.19

## Corrections

* Correction of the maximum value of the elevation x tailrace table for plants with influence of spillage on the tailrace.

# Version 3.5.18

## New features

* Printing, in log, of the list of plants classified as run-of-river.

## Corrections

* Correction in the elevation x tailrace table when a plant is influenced by spillage in the tailrace. In this version, the historical maximum flow is also considered for the calculation of the points in the table when the plant has spillage influence in the tailrace channel.
* Reduction of the tolerance between minimum/maximum dimension to consider valid a table dimension x volume.


# Version 3.5.17

## Corrections

* Correction in the classification of run-of-river plants with the Newave criteria.


# Version 3.5.16

## Corrections

* Bug fix when reading the coordinates x tailrace polynomials of hydroelectric plants introduced in version 3.5.15.
* Bug fix that always enabled Newave criteria for run-of-river hydropower plants classification.


# Version 3.5.15

## New features

* Option (default) to classify hydropower plants as run-of-river using the Newave criteria.
* MDC `CONFIG` block to redefine parameters used in the conversion process. In this version, `TOL_FIO_DAGUA` is available to configure the difference between maximum and minimum volume to classify a plant as a run-of-river (alternative to the previous option).


# Version 3.5.14

## New features

* Renewable technology type field in the `USINA_NAO_SIMULADA` block of the MDC.

# Version 3.5.13

## Corrections

* Compatibility of renewable data for SDDP 16.
* Correction in the action of the buttons “Search” of data folder and MDC file.

# Version 3.5.12

## New features

* New modification files with the conversion of non-simulated plants into renewable sources for the PMO as of May/20 and PDE 29.

## Corrections

* Correction in the handling of systems in the application of the `USINA_NAO_SIMULADA` block in PDE 29.


# Version 3.5.11

## New features

* Possibility of representing non-simulated Newave plants as Renewable Sources in SDDP using the `USINA_NAO_SIMULADA` block in the modification file. See manual.

## Corrections

* Treatment of the initial and final stages of the structural CVUs of thermoelectric plants.
* Update of the correction in the rounding of the Minimum Generation value of Thermal Power Plants: using double precision for the verification and truncation of the minimum generation value.


# Version 3.5.10

## Corrections

* Correction in the conversion of the data of modifications of the sum of interconnection: it considers information of the final month to open the limits of the steps not informed.
* Corrects the reading of data from small plants and the application of the depth of the landings.


# Version 3.5.9

## New features

* GUI update, adds buttons like “Show in Explorer” and “Browse...” to show Newave/SDDP data folder in Windows Explorer and to select/create a different folder with the system screen respectively. Minor UI fixes.
* Possibility of renaming plants and systems through the code “NAME” in the registration modification files. See manual.

## Corrections

* Correction in the rounding of the value of Minimum Generation of Thermal Plants, leading to exceed the installed power of the plant in a certain stage/block.


# Version 3.5.8

## Corrections

* Correction in the conversion of interconnection modifications data: reduces the tolerance of the difference between two consecutive months to consider the modification.


# Version 3.5.7

## Corrections

* Corrects handling of the additional load in the total demand of a system.


# Version 3.5.6

## Corrections

* Reading the configuration of the number of years of scheduled maintenance to be considered when reading the thermal plant maintenance file (0, 1 or 2).


# Version 3.5.5

## New features

* Option to consider zero scheduled downtime in the first calendar year for maintenance-free plants (disabled by default).
* Editing the outputs selected by default of a converted case through the index.dat file (folders in the program's installation directory).

## Corrections

* Adjusts an inflexible portion of the thermal generation when it exceeds the remaining installed power during maintenance.


# Version 3.5.4

## Corrections

* Bug fix in the option to automatically rename elements with duplicate names when the name has 12 characters filled.
* Bug fix when the option “Controllable spillage in all plants” is disabled.


# Version 3.5.3

## Corrections

* Fixed average block duration rounding that occasionally resulted in simulation error messages.
* Remove unused parameters from sddp.dat.
* Correction in the maximum power of non-simulated plants, starting to consider the highest power between the defined in the system and level data files.
* Default option for compatibility with OptGen: “Update registration in addition to modification files”.


# Version 3.5.2

## Corrections

* Generation of names for small plants.
* Removes persistence from the vazoesC.dat read configuration.
* Removes a factor of 0.995 from the converted GTMIN/minimum thermal generation value.


# Version 3.5.1

## New features

* Treatment of non-controllable and partially controllable spill options.
* Minimum thermal generation GTMIN.DAT file reading.
* Reading the GHMIN.DAT file of minimum hydroelectric generation.
* Reading the RE.DAT file of electrical restrictions of equivalent energy reservoir.
* Representation of more than one small plant per subsystem.
* Reading the VMINP and CMONT mnemonics from MODIF.DAT.
* Reading of scenario resampling options and monthly or annual correlation matrix.

## Corrections

* Ignores preventive rationing option.
* Default acronym for North (NO) and Northeast (NE) systems.
* Correction in the automatic acronym for abbreviated names (eg: T. PIRES = TP).
* Improved filling of standby volume data (VMAXT).


# Version 3.5

## New features

* Added option to correct negative incrementals in history.

## Corrections

* Correction in reading interchange grouping data for more than 3 levels.
* Changing the number of interchange sum modifications.
* Reading of thermal expansion data for dates prior to the start of the study.


# Version 3.4.4

## New features

* Reading the REE.DAT file to consider equivalent energy reservoirs. With this, the converter starts to correctly interpret the CONFHD.DAT file.
* Inclusion of a new MDC file for PMO cases as of April/2016.


# Version 3.4.3

## New features

* Change to inform the nominal project values in the registration data for hydroelectric and thermoelectric plants in expansion. This change has no impact on the results and aims to facilitate the integration of cases from the Brazilian system with the OptGen expansion planning model, developed by PSR.
* Extension in the reading of the MDC file to allow resetting the defluence penalty keeping the limits informed in Newave.
* Inclusion of a new MDC file for PMO cases from October/2015.
* New option for selecting the number of forward scenarios in SDDP: 200 (default) or 1200 scenarios.

## Corrections

* Correction of error when reading the ARQUIVOS.DAT file due to the inclusion of new equivalent reservoir files and electrical restrictions.


# Version 3.4.2

## New features

* Flexibility in reading data for modifying the registration of hydroelectric plants to accept the definition of chronological minimum flow data for the “PRE” and “POS” years of the study.


# Version 3.4.1

## New features

* The maximum number of interchange aggregation modifications has been increased.
* New registry modification file (MDC) for the 2023 Decennial Expansion Plan (PDE 2023).


# Version 3.4

## New features

* Flexibility in reading the generation data of small plants to allow interpretation of misaligned codes.
* The conversion of the time-variable Forced Outage Equivalent Rate (TEIF) data, defined in the EXPT.DAT file through the TEIFT parameter, was included.


# Version 3.3

## New features

* Fixed an error in converting fuel data to zero defined cost fuels for the entire study horizon. These fuels were not converted to SDDP and the database was inconsistent.


# Version 3.2

## New features

* The conversion of the time-varying minimum flow (minimum flow) data, associated with the VAZMINT parameter of the MODIF.DAT file, was included.


# Version 3.1

## New features

* The conversion of parameters associated with the CVaR risk aversion methodology was included.
* The following default parameters for SDDP execution were changed:
  * Number of series changed from 80 to 200
  * Maximum number of iterations changed from 7 to 8
  * Minimum number of iterations equal to maximum number of iterations for rounds with CVaR
  * Penalty for violation of minimum flow changed from 0.1 BRL/hm3 to 40,000 BRL/hm3.
  * New option to use absolute seed set as default.
  * Option for seed 33013 (SEED 33013) disabled.


# Version 3.0

## New features

* Changes related to the details of waterfalls through the external file for modification of the NEWAVE register (file NWSDDP.MDC):
  * A new functionality was added to the interface that allows the management of different NWSDDP.MDC files (which may contain differences to adapt to different NEWAVE cases). These files will be part of the NwSddp converter installation and the file to be used can be selected at the time of data conversion. In addition, a functionality was also created to download MDC files that will be published in the future by PSR.
  * Some additional loads defined in the Newave data should not be added to the demand as they are, for example, submotors already considered in the individualized SDDP model and, if they were considered, there would be a double counting in the demand of the corresponding systems. A new field has been included that, if informed, obligatorily defines for all additional loads whether or not it should be considered in the conversion process.
  * A field was included to define chronological minimum runoff data, which allows for detailed modeling of the Belo Monte and Belo Monte Complementar plants.
  * Extension of the reading of the modification data of the hydroelectric plants register to consider the field “Average leakage channel”.
* New option that indicates that the file VAZOESC.DAT (flows from the DECOMP model) should be considered instead of the file VAZOES.DAT (flows from the NEWAVE model).
* The writing of fuel data considering the most current SDDP format was implemented. The initial step of converting these data indicated by the SDDP graphical interface will no longer be necessary when opening a case newly created by the converter.
* Verification of duplicate small power plant data has been included.
* Check was included to define penalty for minimum operating volume restrictions as default SDDP in cases where the accumulated production factor of downstream plants is less than zero (pumps).
* Changed formats of generated files and order of elements in order to ensure compatibility with the format used by the SDDP graphical interface when saving data.


# Version 2.8

## New features

* Reading and conversion of additional load data was implemented. The demand of the additional loads is incorporated into the demand of the corresponding system.
* The need for a hydrological station file (POSTOS.DAT) was removed. If there is any inconsistency in the file or it does not exist, the converter will use the name of the associated hydroelectric plant as the name of the station.
* Added an option to automatically correct duplicate names for systems, hydroelectric plants, thermal plants and hydrological stations. If this option is disabled (default option) the program displays a message that allows the user to enter new names for the elements.
* The converter identifies pairs of hydroelectric plants located in different systems and associated with the same hydrological station. For each pair, the unpowered plant is automatically considered as dummy and is removed from the configuration. In addition, the real power plant is connected to the dummy power plant's system cascade. If both plants do not have motorization, the converter will try to identify the fictitious plant through the presence of the FIC marker in its name. If this marker is found, the converter will ask the user to confirm that the plant is, in fact, fictitious.
* Added protection for reading total energy market data in inconsistent format.


# Version 2.7

## New features

* The extension of the Risk Aversion Curve reading was implemented with the option “Penalty in the minimum volume”. When this option is selected, the CAR is not represented by system and the minimum operative volume data are penalized based on the CAR cost indicated for each system and the plant's average accumulated production factor.
* There is a limitation of Newave, which requires that real systems must have at least one hydroelectric plant in operation at all stages of the study. Due to this, EPE made, in the 2019 Decennial Plan, a special model for the Belo Monte, Tapajós and others plants, which includes a fictitious machine with a power equal to 1 MW and maximum turbine power equal to 1 m3/s entering the setup start. An option was created that aims to try to identify these plants and correct the configuration in the creation of the SDDP database. This option can be selected by the user in the “Options” screen in the interface.
* Added a check on the consistency between the power of machines added in the hydroelectric expansion file (EXPH.DAT) and the hydroelectric plant registration file (HIDR.DAT).
* The maximum turbocharging of hydroelectric plants considered for the calculation of the table of “outflow  tailrace level” is now based on the highest turbine value over the entire study horizon.

## Corrections

* The printing format of the interconnection coefficients in the interchange sum restrictions has been corrected.
* Fixed an error in the initialization of the number of machines of existing hydroelectric plants with expansion, which caused, in some cases, the number of machines, the total power and the maximum tur-bination of the plant to be above the correct value.
* An error in printing the flow history file has been fixed.


# Version 2.6

## New features

* As of this version, the NwSddp converter considers the conversion of Newave version 14 data as the default option. An option has been included for converting data in the format of previous versions, which can be selected in the “Options > Execution Options” screen in the interface from NwSddp. The difference between the versions consists in the fact that the data from versions prior to 14 admit data of “time-variable deficit cost”, whose file name is indicated in record 31 of the “arquivos.dat” file. In turn, data from versions after 14 indicate in the same record the data file of "grouping of interchanges".
* Conversion of exchange aggregation data has been included. These data, present in Newave from version 14 onwards, are converted to SDDP and represented as sum restrictions of exchange flows.
* The maximum flow point for creating the table "exhaust channel height x flow" is now obtained as a function of the maximum flow in the history.
* The “Area” (constant) field, used by SDDP to calculate the evaporation of run-of-river plants, is now also calculated for the other plants.

## Corrections

* Treatment for reading hydroelectric expansion data was introduced because an error occurred in the NwSddp if the hydroelectric expansion data had an inconsistent format. As of this version, a message is informed indicating the inconsistent record in case of error.
