# Visual Outputs

### 01. 3x3 Mean Filter
- **Test matrix center:** `22.2222` (`200 / 9`) · **Gaussian noise ($\sigma=0.05$) PSNR:** `26.4 dB` $\rightarrow$ `27.1 dB`

![01 Mean Filter](outputs/01_mean_filter.png)

### 02. 3x3 Weighted Average Filter
- **Test matrix center:** `28.1250` (`450 / 16`) · **Gaussian noise ($\sigma=0.05$) PSNR:** `26.4 dB` $\rightarrow$ `28.6 dB`

![02 Weighted Average Filter](outputs/02_weighted_average_filter.png)

### 03. 5x5 Gaussian Spatial Filter ($\sigma = 1.0$)
- **Test matrix center:** `22.8023` · **Gaussian noise ($\sigma=0.05$) PSNR:** `26.4 dB` $\rightarrow$ `26.9 dB`

![03 Gaussian Filter](outputs/03_gaussian_filter.png)

### 04. 3x3 Median Filter
- **Test matrix center:** `20.0000` · **5% Salt-and-Pepper noise PSNR:** `17.9 dB` $\rightarrow$ `29.7 dB`

![04 Median Filter](outputs/04_median_filter.png)

### 05. 3x3 Laplacian Sharpening Filter
- **Test matrix sharpened center:** `170.0000` · **SciPy match:** `True`

![05 Laplacian Filter](outputs/05_laplacian_filter.png)

### 06. Sobel Edge Detection Filter
- **Test matrix gradient magnitude:** `360.0000` · **SciPy match:** `True`

![06 Sobel Filter](outputs/06_sobel_filter.png)

### 07. High-Boost Sharpening Filter ($A = 1.5$)
- **Test matrix center:** `52.7778` (`475 / 9`) · **SciPy match:** `True`

![07 High Boost Filter](outputs/07_high_boost_filter.png)

### 08. Ideal Low-Pass Filter (ILPF, $D_0 = 40$)
- **Sample $H(D)$ at $D=[0,1,2,3]$ ($D_0=2$):** `[1.0000, 1.0000, 1.0000, 0.0000]`

![08 Ideal Low Pass Filter](outputs/08_ideal_low_pass_filter.png)

### 09. Butterworth Low-Pass Filter (BLPF, $n = 2, D_0 = 40$)
- **Sample $H(D)$ at $D=[0,1,2,3]$ ($D_0=2$):** `[1.0000, 0.9412, 0.5000, 0.1649]`

![09 Butterworth Low Pass Filter](outputs/09_butterworth_low_pass_filter.png)

### 10. Gaussian Low-Pass Filter (GLPF, $D_0 = 40$)
- **Sample $H(D)$ at $D=[0,1,2,3]$ ($D_0=2$):** `[1.0000, 0.8825, 0.6065, 0.3247]`

![10 Gaussian Low Pass Filter](outputs/10_gaussian_low_pass_filter.png)

### 11. Ideal High-Pass Filter (IHPF, $D_0 = 40$)
- **Sample $H(D)$ at $D=[0,1,2,3]$ ($D_0=2$):** `[0.0000, 0.0000, 0.0000, 1.0000]`

![11 Ideal High Pass Filter](outputs/11_ideal_high_pass_filter.png)

### 12. Butterworth High-Pass Filter (BHPF, $n = 2, D_0 = 40$)
- **Sample $H(D)$ at $D=[0,1,2,3]$ ($D_0=2$):** `[0.0000, 0.0588, 0.5000, 0.8351]`

![12 Butterworth High Pass Filter](outputs/12_butterworth_high_pass_filter.png)

### 13. Gaussian High-Pass Filter (GHPF, $D_0 = 40$)
- **Sample $H(D)$ at $D=[0,1,2,3]$ ($D_0=2$):** `[0.0000, 0.1175, 0.3935, 0.6753]`

![13 Gaussian High Pass Filter](outputs/13_gaussian_high_pass_filter.png)

### 14. Huffman Coding (8-bit Grayscale)
- **6-symbol check:** `2.2000` avg bits vs entropy `2.1435` bits · **Image (`256x256`):** `524,288` bits $\rightarrow$ `490,798` bits (`1.068x`, `7.4890 bpp`, lossless `True`)

![14 Huffman Coding](outputs/14_huffman_coding.png)

### 15. Arithmetic Coding (4-bit Quantized Grayscale, Block = 32)
- **5-symbol check (`a1 a2 a3 a3 a4`):** `[0.06752, 0.06880)`, tag `0.06816` · **Image (`256x256`):** `262,144` bits $\rightarrow$ `250,332` bits (`1.047x`, `3.8198 bpp`, lossless `True`)

![15 Arithmetic Coding](outputs/15_arithmetic_coding.png)
