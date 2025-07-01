# Description of WHOTS-19 Mooring

The WHOTS-19 mooring was deployed on June 17, 2023, from the NOAA Ship _Oscar
Elton Sette_ and recovered on June 6, 2024. The mooring consisted of a surface
buoy equipped with two complete sets of Air–Sea Interaction Meteorological
(ASIMET) sensors and a suite of subsurface oceanographic instruments mounted
along the bridle and mooring line down to 155 m, with additional sensors near
the bottom. For a detailed technical description of the mooring design, see
{cite}`Santiago-Mandujano2024a, Santiago-Mandujano2024b`.

The WHOTS-19 mooring was designed to collect high-quality time series of
surface meteorology and upper-ocean temperature, salinity, and biogeochemical
variables in support of long-term air-sea flux studies at Station ALOHA.

## Surface Components

The buoy included the following instrumentation mounted on a blue hull with a
white tower and yellow deck ({numref}`table-surface-components`):

```{table} Surface meteorological instrumentation on the WHOTS-19 buoy, organized by system side (port = System 1, starboard = System 2). All sensors were mounted on the buoy tower. Heights are reported relative to the buoy deck.
:name: table-surface-components
:widths: auto
:align: center
| **Instrument Type**                                     | **IDs / Details**                                                                                                    |
| ------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| **Data Loggers**                                        | 9 (System 1, port side); ID 42 (System 2, starboard side)                                                            |
| **Relative Humidity and Air Temperature (HRH) Sensors** | 269 and 247, mounted at 231 cm                                                                                       |
| **Barometric Pressure Recorders (BPR)**                 | 210 and 206, mounted at 242 cm                                                                                       |
| **Wind Sensors (RM Young)**                             | 225 and 701, mounted at 264 cm                                                                                       |
| **Precipitation Sensors (PRC)**                         | 235 (System 1 – top broken before recovery); ID 506, both mounted at 256 cm                                          |
| **Longwave Radiation Sensors (LWR)**                    | 214 and 219, mounted at 281 cm                                                                                       |
| **Shortwave Radiation Sensors (SWR)**                   | 233 and 373, mounted at 281 cm                                                                                       |
| **Sea Surface Temperature (SST)**                       | 1727 and 5996, mounted at –155 cm                                                                                    |
| **Iridium Satellite Systems**                           | IMEIs: 300234063855630, 300234063160290                                                                              |
| **GPS – Melo**                                          | IMEI: 300034013707580                                                                                                |
| **GPS – Rover**                                         | 1034 and 724; IMEIs: 300434064530400, 300434063547190                                                                |
| **Other Sensors**                                       | Vaisala WXT (ID 204, 264 cm); Airmar (ID 6079L253, 273 cm, hanging); HC2A (ID WI9, 232 cm); SBE39AT (ID 719, 228 cm) |
```

## Subsurface Instrumentation

Subsurface instruments were mounted along the bridle and at a fixed depth on
the mooring line, as follows ({numref}`table-subsurface`):

```{table} Additional shared surface instrumentation on the WHOTS-19 buoy, including GPS units, Iridium satellite modems, and auxiliary sensors.
:name: table-subsurface
:widths: auto
:align: center
| **Instrument Type**   | **ID**  | **Depth** | **Notes**               |
| --------------------- | ------- | --------- | ----------------------- |
| MAPCO₂ System         | 26      | 155       | With equilibration tube |
| CTD (SBE16)           | 6832    | 155       |                         |
| Oxygen Sensor         | 1381    | 155       |                         |
| Fluorometer           | 2597    | 155       | Includes bio-wiper      |
| pH Sensor (SAMI)      | P246    | 155       |                         |
| Span Gas Canister     | JB03812 | —         | For sensor calibration  |
| Xeos Kilo Transmitter | 1494    | —         | IMEI: 300234062727610   |
```

Five internally logging Sea-Bird SBE-56 temperature sensors were bolted to the
buoy hull's underside, measuring sea surface temperature and salinity.
The SBE-56s measured SST once every 60 sec between 80-110 cm below the surface.
Two SBE-37 MicroCATs were at 1.55m measuring at every 300s (See
{numref}`table-7`).

```{table} WHOTS-19 MicroCAT and SBE-56 Temperature Sensor Information.
:name: table-7
:widths: auto
:align: center
| **Instrument** | **SN** | **Depth (m)** | **Sample Interval (sec)** |
|:--------------:|:------:|:-------------:|:-------------------------:|
|     SBE-56     |  6410  |     0.8       |            60             |
|     SBE-56     |  6239  |     0.8       |            60             |
|     SBE-56     |  6412  |     1.0       |            60             |
|     SBE-56     |  6983  |     1.1       |            60             |
|     SBE-56     |  7211  |     0.8       |            60             |
|     SBE-37     |  1727  |     1.55      |            300            |
|     SBE-37     |  5996  |     1.55      |            300            |
```

Instrumentation provided by UH for the WHOTS-19 mooring included 18 Sea-Bird
SBE-37 MicroCATs, of which 9 were pressure-equipped, and two newly added
MicroCATs deployed at greater depths (120 m, 135 m). All MicroCATs measured
temperature and conductivity and were deployed with antifoulant capsules to
minimize biofouling. In addition, UH deployed two upward-looking RDI Workhorse
Acoustic Doppler Current Profilers (ADCPs) operating at 300 kHz and 600 kHz,
respectively. WHOI contributed two Vector Measuring Current Meters (VMCMs), an
Acoustic Receiver, and all required deep mooring hardware. The ADCPs were
mounted at nominal depths of 47.5 m and 125 m, and the VMCMs were positioned at
10 m and 30 m. Two additional SBE-37 MicroCATs were installed approximately 39 m
above the anchor.

The {numref}`mooring_subsurface` table provides detailed metadata for the
WHOTS-19 subsurface instrumentation, including nominal depths, serial numbers,
sample intervals, and event times. To verify the performance of internal
clocks, a cold-water spike was applied to all UH MicroCATs before deployment by
placing an ice pack against each temperature sensor
({numref}`mooring_subsurface`) and again after recovery ({numref}`table-8`). For
the ADCPs, a 20-second manual transducer rub was performed to generate a
recognizable signal spike ({numref}`table-9`, {numref}`table-10`).

```{raw} latex
\begin{landscape}
```

```{table} WHOTS-19 mooring subsurface instrument deployment. All times are in UTC (MM/DD/YY hh:mm:ss). Columns: SN = Serial Number, Inst = Instrument, Z (m) = Depth in meters, P SN = Pressure Sensor Serial Number, Δt (s) = Sample Interval in seconds, AR = Acoustic Receiver, MC = MicroCAT, VMCM = Vector Measuring Current Meter, ADCP = Acoustic Doppler Current Profiler.
:name: mooring_subsurface
:widths: auto
:class: longtable
:align: center

|   SN   |    Instrument     |      Z (m)      | Pressure SN | Δt (s) | Start Logging Data |   Cold Spike Begin    |    Cold Spike End     |   Time in Water   |
| :----: | :---------------: | :-------------: | :---------: | :----: | :----------------: | :-------------------: | :-------------------: | :---------------: |
|  3382  |        MC         |        7        |     N/A     |  180   | 06/13/23 23:59:59  |   06/16/23 00:00:00   |   06/16/23 00:30:00   | 06/16/23 21:00:00 |
|  0035  |       VMCM        |       10        |     N/A     |   60   | 06/08/23 00:21:29  |  06/16/23 20:23:00\*  |          N/A          | 06/16/23 20:28:00 |
|  6892  |        MC         |       15        |   2651234   |   75   | 06/13/23 23:59:59  |   06/16/23 00:00:00   |   06/16/23 00:30:00   | 06/16/23 20:25:00 |
|  4663  |        MC         |       25        |     N/A     |  180   | 06/13/23 23:59:59  |   06/16/23 00:00:00   |   06/16/23 00:30:00   | 06/16/23 20:19:00 |
| 112497 | Acoustic Receiver |       25        |     N/A     |  N/A   | 06/12/23 19:00:00  |          N/A          |          N/A          | 06/16/23 20:19:00 |
|  0058  |       VMCM        |       30        |     N/A     |   60   | 06/08/23 00:21:29  |  06/16/23 20:13:00\*  |          N/A          | 06/16/23 20:16:00 |
|  3633  |        MC         |       35        |     N/A     |  180   | 06/13/23 23:59:59  |   06/16/23 00:00:00   |   06/16/23 00:30:00   | 06/16/23 20:12:00 |
|  3381  |        MC         |       40        |     N/A     |  180   | 06/13/23 23:59:59  |   06/16/23 00:00:00   |   06/16/23 00:30:00   | 06/16/23 20:09:00 |
|  3668  |        MC         |       45        |    5579     |  180   | 06/16/23 00:01:30  |   06/16/23 01:40:00   |   06/16/23 02:05:00   | 06/16/23 20:06:00 |
| 13917  |   600 kHz ADCP    |      47.5       |     N/A     |  600   | 06/15/23 23:59:00  | See {numref}`table-9` | See {numref}`table-9` | 06/16/23 21:23:00 |
|  3619  |        MC         |       50        |     N/A     |  180   | 06/13/23 23:59:59  |   06/16/23 00:00:00   |   06/16/23 00:30:00   | 06/16/23 21:24:00 |
|  3620  |        MC         |       55        |     N/A     |  180   | 06/13/23 23:59:59  |   06/16/23 00:00:00   |   06/16/23 00:30:00   | 06/16/23 21:27:00 |
|  3621  |        MC         |       65        |     N/A     |  180   | 06/13/23 23:59:59  |   06/16/23 00:00:00   |   06/16/23 00:30:00   | 06/16/23 21:29:00 |
|  9988  |        MC         |       75        |     N/A     |  180   | 06/13/23 23:59:59  |   06/16/23 00:00:00   |   06/16/23 00:30:00   | 06/16/23 21:31:00 |
|  4699  |        MC         |       85        |    10209    |  240   | 06/13/23 23:59:59  |   06/16/23 00:00:00   |   06/16/23 00:30:00   | 06/16/23 21:32:00 |
|  3791  |        MC         |       95        |     N/A     |  180   | 06/16/23 02:00:00  |   06/16/23 02:06:00   |   06/16/23 02:30:00   | 06/16/23 21:34:00 |
|  2769  |        MC         |       105       |  12364705   |  240   | 06/13/23 23:59:59  |   06/16/23 00:00:00   |   06/16/23 00:30:00   | 06/16/23 21:36:00 |
| 25352  |     MC (New)      |       120       |   5983494   |  240   | 06/13/23 23:59:59  |   06/16/23 00:00:00   |   06/16/23 00:30:00   | 06/16/23 21:47:00 |
|  7637  |   300 kHz ADCP    |       125       |     N/A     |  300   | 06/15/23 23:59:00  | See {numref}`table-9` | See {numref}`table-9` | 06/16/23 21:47:00 |
| 25444  |     MC (New)      |       135       |  12152941   |  240   | 06/13/23 23:59:59  |   06/16/23 00:00:00   |   06/16/23 00:30:00   | 06/16/23 21:49:00 |
|  4701  |        MC         |       155       |    10211    |  240   | 06/13/23 23:59:59  |   06/16/23 00:00:00   |   06/16/23 00:30:00   | 06/16/23 21:51:00 |
| 11381  |        MC         | 39 m off Anchor |   2146836   |  300   | 06/16/23 00:01:00  |   06/16/23 00:00:00   |   06/16/23 00:30:00   | 06/17/23 00:02:41 |
| 11380  |        MC         | 39 m off Anchor |   2146835   |  300   | 06/16/23 00:01:00  |   06/16/23 00:00:00   |   06/16/23 00:30:00   | 06/17/23 00:02:41 |
```

```{raw} latex
\end{landscape}
```

```{table} WHOTS-19 mooring recovery summary for C-T (Conductivity-Temperature) and ADCP (Acoustic Doppler Current Profiler) instruments. All times in UTC (MM/DD/YY hh:mm:ss). SN = Serial Number, Tlg = Logging, Spk = Spike, Q = Quality.
:name: table-8
:widths: auto
:align: center

| **Z (m)** |   **SN**   |     **T out**     |      **Spk**      |    **End Spk**    |   **Tlg Stop**    | **N Samples** |           **Q**           |
| :-------: | :--------: | :---------------: | :---------------: | :---------------: | :---------------: | :-----------: | :-----------------------: |
|     7     |    3382    | 06/07/24 01:46:00 | 06/07/24 05:56:00 | 06/07/24 06:26:00 | 06/11/24 00:13:21 |    174243     |           Good            |
|    15     |    6892    | 06/07/24 01:54:00 | 06/07/24 05:56:00 | 06/07/24 06:26:00 | 06/14/24 14:38:03 |    414947     |           Good            |
|    25     |    4663    | 06/07/24 01:57:00 | 06/07/24 05:56:00 | 06/07/24 06:26:00 | 06/08/24 03:38:40 |    172873     |           Good            |
|    35     |    3633    | 06/07/24 00:41:00 | 06/07/24 05:56:00 | 06/07/24 06:26:00 | 06/07/24 19:31:30 |    172710     |           Good            |
|    40     |    3381    | 06/07/24 00:37:00 | 06/07/24 05:56:00 | 06/07/24 06:26:00 | 06/08/24 03:19:15 |    172866     |           Good            |
|    45     |    3668    | 06/07/24 00:33:00 | 06/07/24 05:56:00 | 06/07/24 06:26:00 | 06/08/24 03:07:45 |    171871     |           Good            |
|   47.5    | ADCP 13917 | 06/07/24 00:29:00 | 06/07/24 05:56:00 | 06/07/24 06:26:00 |        N/A        |     40846     |     Stopped 3/25/24       |
|    50     |    3619    | 06/07/24 00:28:00 | 06/07/24 05:56:00 | 06/07/24 06:26:00 | 06/11/24 00:19:06 |    174245     |           Good            |
|    55     |    3620    | 06/07/24 00:27:00 | 06/07/24 05:56:00 | 06/07/24 06:26:00 | 06/11/24 00:01:23 |    174240     |           Good            |
|    65     |    3621    | 06/07/24 00:25:00 | 06/07/24 05:56:00 | 06/07/24 06:26:00 | 06/10/24 23:56:24 |    174238     |           Good            |
|    75     |    9988    | 06/07/24 00:25:00 | 06/07/24 05:56:00 | 06/07/24 06:26:00 | 06/07/24 20:19:00 |    172725     |           Good            |
|    85     |    4699    | 06/07/24 00:24:00 | 06/07/24 05:56:00 | 06/07/24 06:26:00 | 06/10/24 23:52:11 |    130678     |           Good            |
|    95     |    3791    | 06/07/24 00:24:00 | 06/07/24 05:56:00 | 06/07/24 06:26:00 | 06/07/24 04:30:20 |    171890     |           Good            |
|    105    |    2769    | 06/07/24 00:23:00 | 06/07/24 05:56:00 | 06/07/24 06:26:00 | 06/08/24 03:28:10 |    129653     |    Did not record P/C     |
|    120    |   25352    | 06/07/24 00:21:00 | 06/07/24 05:56:00 | 06/07/24 06:26:00 | 06/08/24 00:27:30 |    129607     |           Good            |
|    125    | ADCP 7637  | 06/07/24 00:17:00 | 06/07/24 05:56:00 | 06/07/24 06:26:00 | 06/07/24 19:07:00 |     51522     |           Good            |
|    135    |   25444    | 06/07/24 00:16:00 | 06/07/24 05:56:00 | 06/07/24 06:26:00 | 06/07/24 22:42:30 |    129581     |           Good            |
|    155    |    4701    | 06/07/24 00:14:00 | 06/07/24 05:56:00 | 06/07/24 06:26:00 | 06/07/24 22:06:10 |    129571     |           Good            |
|  38 mab   |   11380    | 06/06/24 19:50:00 | 06/07/24 19:52:00 | 06/07/24 20:10:00 | 06/08/24 00:27:06 |    103093     |           Good            |
|  38 mab   |   11381    | 06/06/24 19:50:00 | 06/07/24 19:52:00 | 06/07/24 20:10:00 | 06/08/24 00:27:19 |    103093     |           Good            |
```

```{table} WHOTS-19 mooring ADCP deployment and configuration information. All times are in UTC (MM/DD/YY hh:mm:ss).
:name: table-9
:widths: auto
:align: center

|        **Parameter**        |  **ADCP S/N 13917**  |  **ADCP S/N 7637**   |
| :-------------------------: | :------------------: | :------------------: |
|     **Frequency (kHz)**     |         600          |         300          |
|  **Number of Depth Cells**  |          25          |          30          |
|   **Depth Cell Size (m)**   |         2 m          |         4 m          |
|   **Pings per Ensemble**    |          80          |          40          |
| **Time per Ensemble (min)** |        10 min        |        10 min        |
|   **Time per Ping (sec)**   |        2 sec         |        4 sec         |
|   **Time of First Ping**    | 06/15/2023, 23:59:00 | 06/15/2023, 23:59:00 |
| **Transducer 1 Spike Time** | 06/16/2023, 05:40:00 | 06/16/2023, 05:40:00 |
| **Transducer 2 Spike Time** | 06/16/2023, 05:40:15 | 06/16/2023, 05:40:15 |
| **Transducer 3 Spike Time** | 06/16/2023, 05:40:30 | 06/16/2023, 05:40:30 |
| **Transducer 4 Spike Time** | 06/16/2023, 05:40:45 | 06/16/2023, 05:40:45 |
|  **Ice Spike Time Begin**   | 06/16/2023, 00:00:00 | 06/16/2023, 00:00:00 |
|   **Ice Spike Time End**    | 06/16/2023, 00:30:00 | 06/16/2023, 00:30:00 |
|      **Time in Water**      | 06/16/2023, 21:23:00 | 06/16/2023, 21:47:00 |
|        **Depth (m)**        |        47.5 m        |        125 m         |

```

```{table} WHOTS-19 mooring ADCP recovery information. All times are in UTC (MM/DD/YY, hh:mm:ss).
:name: table-10
:widths: auto
:align: center

|        **Parameter**        | **ADCP S/N 13917** | **ADCP S/N 7637**  |
| :-------------------------: | :----------------: | :----------------: |
|     **Frequency (kHz)**     |        600         |        300         |
|  **Number of Depth Cells**  |         25         |         30         |
|   **Depth Cell Size (m)**   |        2 m         |        4 m         |
|   **Pings per Ensemble**    |         80         |         40         |
| **Time per Ensemble (min)** |       10 min       |       10 min       |
|   **Time per Ping (sec)**   |       2 sec        |       4 sec        |
|    **Time of Last Ping**    | 06/07/24, 05:40:00 | 06/07/24, 05:40:00 |
| **Transducer 1 Spike Time** | 06/07/24, 07:32:00 | 06/07/24, 07:21:00 |
| **Transducer 2 Spike Time** | 06/07/24, 07:32:15 | 06/07/24, 07:21:15 |
| **Transducer 3 Spike Time** | 06/07/24, 07:32:30 | 06/07/24, 07:21:30 |
| **Transducer 4 Spike Time** | 06/07/24, 07:32:45 | 06/07/24, 07:21:45 |
|  **Ice Spike Start Time**   | 06/07/24, 05:56:00 | 06/07/24, 05:56:00 |
|   **Ice Spike End Time**    | 06/07/24, 06:26:00 | 06/07/24, 06:26:00 |
|    **Time in the Water**    | 06/16/23, 21:47:00 | 06/16/23, 21:47:00 |
|    **Time out of Water**    | 06/07/24, 00:29:00 | 06/07/24, 00:17:00 |
|        **Depth (m)**        |       47.5 m       |       125 m        |

```

The 300 kHz ADCP at 125 m (SN 7637) operated flawlessly for the entire
deployment and was still recording on recovery. In contrast, the 600 kHz ADCP
at 47.5 m (SN 13917) stopped logging on 25 March 2024. Data collected before
shutdown are good, aside from near-surface side-lobe interference.

The RDI 300 kHz Workhorse Sentinel ADCP, SN 7637, was installed at 125 m with
its transducers facing upward and an external battery pack. It pinged every 4 s
for 160 s once every 10 min—a burst regime selected to reduce aliasing from
large-swell orbital motions. Bin size was 4 m. In total, 51 522 ensembles were
logged, beginning 06/15/2023 23:59:00 and ending 06/07/2024 18:48:59 (see
{numref}`table-9`, {numref}`table-10`, and
{ref}`/appendices.md#whots-19-300-khz-serial-7367`). This instrument also
measured temperature.

The RDI 600 kHz Workhorse Sentinel ADCP, SN 13917, was installed at 47.5 m with
transducers facing upward and an external battery pack. It pinged every 2 s for
160 s once every 10 min, with a 2 m bin size. The instrument logged 40 846
ensembles between 06/15/2023 23:59:00 and 03/25/2024 15:38:59 (see
{numref}`table-9`, {numref}`table-10`, and
{ref}`/appendices.md#whots-19-600-khz-serial-13917`). Upon recovery it was
silent. Diagnostic checks suggest a Y-cable fault: the internal battery was
fully depleted, whereas both external packs were only partially discharged—an
imbalance not expected under normal operation. Data collected before shutdown
are high-quality, apart from near-surface side-lobe interference. This
instrument also measured temperature.

Two VMCMs (SN 0035 at 10 m and SN 0058 at 30 m) were configured by the WHOI/UOP
group to sample every minute; both also recorded temperature.

Recovery details for the C-T instruments appear in {numref}`table-8`. All
WHOTS-19 instruments were retrieved. Biofouling was common—severe near the
surface and detectable, though minor, down to the 125 m ADCP.

Post-recovery inspection found every MicroCAT intact with its antifoulant
capsule. Preliminary checks show high-quality records from all units except
those flagged in {numref}`table-8`; definitive assessment awaits post-deployment
calibrations and QA/QC (see
{ref}`/5_section.md#microcat-data-processing-procedures`,
{ref}`/6_section.md#microcat-data`). One exception is SN 2769, which failed to
log pressure and conductivity, although no external damage to the sensor or its
conductivity cell was observed.
