# Dataset for PAPR Reduction with Supervised Neural Network

This repository provides the dataset used for training and testing a supervised neural network for PAPR reduction in OFDM systems.

## Dataset Description
- **OFDM symbols:** 1,000,000  
- **Subcarriers:** 64  
- **Pilots:** 10 pilot subcarriers  
- **Modulation:** QPSK (normalized to unit energy)  

## Files
- **`symbol_Ori_.zip`**  
  OFDM symbols with **pilot subcarriers set to zero**.  
  ➝ Used as the **input to the neural network**.  

- **`symbol_final_no.zip`**  
  OFDM symbols where the pilot subcarriers are **filled with values that drive the PAPR to 8 dB**.  
  ➝ Used as the **expected output (labels) during training**.  

## Notes
- The dataset is **not yet split into training and testing sets**.  
  ➝ The provided code automatically performs this split.  
- The dataset is also **not separated into real and imaginary parts**.  
  ➝ The code handles this preprocessing step as well.  

## Reference
For full details, see the paper:  
[DOI: 10.1109/TLA.2025.11045671](https://doi.org/10.1109/TLA.2025.11045671)  

## Code
The implementation used in the paper is available at:  
[https://github.com/BiaSabrina/PAPR-Reduction-Code](https://github.com/BiaSabrina/PAPR_Reduction_Code)
