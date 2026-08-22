# Uniform Quantization and PCM

## Experiment 4 - Uniform Quantization and PCM

### Objective

* Implement uniform quantization and PCM encoding.
* Study the effect of quantization resolution.
* Measure quantization error and SQNR.
* Compare measured SQNR with the theoretical approximation.

### Bit Resolutions

The experiment uses:

* 2 bits → 4 levels
* 3 bits → 8 levels
* 4 bits → 16 levels
* 6 bits → 64 levels
* 8 bits → 256 levels

The number of quantization levels is:

L = 2^n

### Theoretical SQNR

For a full-scale sinusoid:

SQNR ≈ 6.02n + 1.76 dB

### Required Visualizations

* Original and quantized waveform
* Staircase quantizer characteristic
* Quantization error waveform
* Quantization error histogram
* SQNR versus number of bits

### Mandatory Validation

For every bit resolution:

* Quantizer indices are checked to be within 0 to L-1.
* PCM word length is checked to be exactly n bits.

### Observation

As the number of bits increases, the number of quantization levels increases. Therefore, the quantization step size and error decrease, while SQNR increases.

The measured SQNR is expected to be close to the theoretical value of 6.02n + 1.76 dB, with small differences due to the finite sampled signal and the approximation used by the theoretical formula.

### Files

* `uniform_quantization_pcm.py`
* `Experiment_4_Uniform_Quantization_PCM.ipynb`
* `Experiment_4_Uniform_Quantization_PCM.pdf`

