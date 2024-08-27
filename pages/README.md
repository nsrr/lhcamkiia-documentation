## About

To facilitate research on the role of CaMKIIα neurons in the lateral hypothalamus (LH-CaMKIIα neurons) as one of the most potent wake-promoting neuronal populations identified to date (Heiss et al., 2024), the Sleep Neurobiology Laboratory at SRI International releases the LH-CaMKIIα dataset. This dataset contains 3 sets of EEG/EMG recordings from adult mice recorded in their home cage using conventional tethered electrodes. The experiments conducted were designed to test the effects of pharmacogenetic activation of LH-CaMKIIα neurons during the inactive phase after bilateral injection of AAVs at -1.4 mm AP, -1.2 mm ML, -4.7 mm DV from pia as follows:

1. Male C57BL6/J mice (N=4) were injected with AAV8-CaMKIIα-hM3D(Gq)-mCherry and dosed with either ALM or VEH at ZT4 and SAL or CNO at ZT5 while EEG/EMG was recorded from ZT3 to ZT12 (Fig. 1 of Heiss et al., 2024);

2. Male and female Vglut2-IRES-Cre mice (N=8) were injected with AAV8-hSyn-DIO-hM3D(Gq)-mCherry and dosed with either DCZ or SAL at ZT2 and recorded from ZT0 to ZT12 (Fig. S1 of Heiss et al., 2024); 

3. Male and female Gad2-IRES-Cre;R26R-EYFP mice (N=10) and C57BL6/J littermates (N=9) were co-injected with 100 nL of a 50-50 mixture of AAV8-CaMKIIα-hM3D(Gq)-mCherry and AAV-CMV-FLEX-mCherry/DTA (Sr10) into the LH to ablate inhibitory neurons in Cre-expressing mice in the same area (Figs. 4 and S5 of Heiss et al., 2024). During the experiments, mice were dosed with either CNO or SAL at ZT4 and recorded from ZT3 to ZT12.  

## Methods

See Methods section in: [Heiss JE, Zhong P, Lee SM, Yamanaka A, Kilduff TS. Distinct lateral hypothalamic CaMKIIα neuronal populations regulate wakefulness and locomotor activity. Proc Natl Acad Sci U S A. 2024 Apr 16;121(16):e2316150121. doi: 10.1073/pnas.2316150121. Epub 2024 Apr 9. PMID: 38593074; PMCID: PMC11032496.](https://pubmed.ncbi.nlm.nih.gov/38593074/)

## Data overview

[EDF files](:files_path:/) exported by a Tucker-Davis Technologies, Inc. (TDT) RZ2 system from tethered recordings, containing bilateral EEG recordings (Channels 1 and 2) from occipito-parietal configuration for redundancy in case one EEG channel failed. Channel 3 corresponds to nuchal EMG. All 3 channels were digitized at 813 Hz and bandpassed at 0.5-300 Hz.

[MAT files](:files_path:/processed_mat_files/) containing processed EEG files used for analysis. These files were created in Matlab R2015b and can be opened in Matlab, Octave or Python. Each file contains the following variables:

<table>
<tr><td><b>Variable</b></td><td><b>Meaning</b></td></tr>
<tr><td>Ztdosing</td><td>Zeitgeber Time (ZT) of first dose</td></tr>
<tr><td>Ztfirsth</td><td>First ZT hour included in analysis (previous ZT times are not quantified)</td></tr>
<tr><td>Ztlasth</td><td>Last ZT hour included in analysis (Later ZT times are not quantified)</td></tr>
<tr><td>bd</td><td>Table with Mean bout duration for every epoch scored as WA, NREM and REM at every ZT hour analyzed</td></tr>
<tr><td>f</td><td>Frequency bins (in Hz) used for FFT</td></tr>
<tr><td>pnr1</td><td>Table with the average NREM power of EEG1 channel at each frequency bin, for each ZT hour quantified.</td></tr>
<tr><td>pnr2</td><td>Table with the average NREM power of EEG2 channel at each frequency bin, for each ZT hour quantified.</td></tr>
<tr><td>pr1</td><td>Table with the average REM power of EEG1 channel at each frequency bin, for each ZT hour quantified.</td></tr>
<tr><td>pr2</td><td>Table with the average REM power of EEG2 channel at each frequency bin, for each ZT hour quantified.</td></tr>
<tr><td>pwa1</td><td>Table with the average Wake power of EEG1 channel at each frequency bin, for each ZT hour quantified.</td></tr>
<tr><td>pwa2</td><td>Table with the average Wake power of EEG2 channel at each frequency bin, for each ZT hour quantified.</td></tr>
<tr><td>pt</td><td>Percentage of time in WA, NREM and REM state for each ZT hour quantified.</td></tr>
<tr><td>scr</td><td>Sleep scoring of the whole recording. 0= WA, 1 = NR, 2=REM. Epochs with artifacts are scored as the main state +0.1</td></tr>
<tr><td>sel</td><td>EEG channel selected for quantification</td></tr>
<tr><td>strattime</td><td>UTC time when EEG recording started</td></tr>
<tr><td>zt0time</td><td>UTC time corresponding to lights on</td></tr>
</table>

## Access and usage restrictions

The LH-CaMKIIα dataset is only available for non-commercial use.

## Citation and acknowledgement

When using this dataset, users must cite the following:

>[Zhang GQ, Cui L, Mueller R, Tao S, Kim M, Rueschman M, Mariani S, Mobley D, Redline S. The National Sleep Research Resource: towards a sleep data commons. J Am Med Inform Assoc. 2018 Oct 1;25(10):1351-1358. doi: 10.1093/jamia/ocy064. PMID: 29860441; PMCID: PMC6188513.](https://pubmed.ncbi.nlm.nih.gov/29860441/)

>[Heiss JE, Zhong P, Lee SM, Yamanaka A, Kilduff TS. Distinct lateral hypothalamic CaMKIIα neuronal populations regulate wakefulness and locomotor activity. Proc Natl Acad Sci U S A. 2024 Apr 16;121(16):e2316150121. doi: 10.1073/pnas.2316150121. Epub 2024 Apr 9. PMID: 38593074; PMCID: PMC11032496.](https://pubmed.ncbi.nlm.nih.gov/38593074/)

Users must include the following text in any Acknowledgements:

> The recordings deposited here were supported by National Institutes of Health grants R01NS077408 and R01NS098813 to Thomas S. Kilduff. The National Sleep Research Resource was supported by the U.S. National Institutes of Health, National Heart Lung and Blood Institute (R24 HL114473, 75N92019R002).

## Changelog

*August 2024*

- Make LH-CaMKIIα dataset available for data requests

## References

- LH-CaMKIIα GitHub Documentation: https://github.com/nsrr/lhcamkiia-documentation

## Questions?

Please reach out to us at support@sleepdata.org or in the [Forum](https://sleepdata.org/forum) if you have questions.
