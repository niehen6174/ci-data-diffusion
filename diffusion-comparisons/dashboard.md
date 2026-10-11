# SGLang-Diffusion Nightly Performance Dashboard

*Generated: Oct 11 | Commit: `11bfd86`*

*Methodology `client-e2e-v1`: client-side latency through each framework's public API, from submit until the output is downloaded; 1 identical client warmup request(s) per case, discarded. First request = the first request after the server reports ready. Server perf dumps are telemetry only.*

*Excluded 23 historical run(s) from baselines and trends because their measurement methodology or warmup count differs. Missing metadata is not treated as matching explicit metadata.*

## SGLang-Diffusion Performance

| Model | Risk | Client samples | Server samples | First request (s) | sglang median (s) |
|-------|------|----------------|----------------|-------------------|---------|
| Anima-Base-v1.0-Diffusers | ✅ | 3 | 3/3 | 2.46 | **2.45** |
| FLUX.1-dev | ✅ | 3 | 3/3 | 4.30 | **4.28** |
| FLUX.2-dev | ✅ | 3 | 3/3 | 13.13 | **13.04** |
| Qwen-Image-2512 | ✅ | 3 | 3/3 | 8.18 | **8.12** |
| Qwen-Image-Edit-2511 | ✅ | 3 | 3/3 | 14.61 | **14.60** |
| Z-Image-Turbo | ✅ | 3 | 3/3 | 0.80 | **0.70** |
| Wan2.2-T2V-A14B-Diffusers | ✅ | 3 | 3/3 | 203.19 | **203.29** |
| Wan2.2-TI2V-5B-Diffusers | ✅ | 3 | 3/3 | 54.73 | **54.76** |
| LTX-2.3 | ✅ | 3 | 3/3 | 11.49 | **11.40** |
| ideogram-4-fp8 | ✅ | 3 | 3/3 | 3.85 | **3.84** |
| Cosmos3-Super | ✅ | 3 | 3/3 | 119.61 | **119.63** |
| Wan2.2-I2V-A14B-Diffusers | ✅ | 3 | 3/3 | 198.12 | **197.92** |
| MiniMax-H3 | ✅ | 3 | 3/3 | 74.49 | **74.77** |

## SGLang Server-Side Breakdown

| Model | Server total (s) | Text encode (s) | Denoise (s) | Decode (s) | Median denoise step (ms) |
|-------|------------------|-----------------|--------------|------------|---------------------------|
| Anima-Base-v1.0-Diffusers | 2.44 | 0.02 | 2.19 | 0.22 | 73.47 |
| FLUX.1-dev | 4.19 | 0.03 | 3.99 | 0.01 | 80.29 |
| FLUX.2-dev | 13.01 | 0.36 | 12.19 | 0.01 | 243.09 |
| Qwen-Image-2512 | 8.06 | 0.23 | 7.76 | 0.06 | 155.96 |
| Qwen-Image-Edit-2511 | 14.53 | N/A | 13.75 | 0.12 | 346.19 |
| Z-Image-Turbo | 0.63 | 0.13 | 0.49 | 0.01 | 57.39 |
| Wan2.2-T2V-A14B-Diffusers | 203.24 | 0.28 | 200.36 | 2.26 | 5011.15 |
| Wan2.2-TI2V-5B-Diffusers | 54.68 | 0.34 | 47.69 | 6.61 | 962.96 |
| LTX-2.3 | 11.31 | 0.40 | 8.19 | 0.93 | 273.44 |
| ideogram-4-fp8 | 3.74 | 0.13 | 3.53 | 0.08 | 179.33 |
| Cosmos3-Super | 119.06 | 0.00 | 116.11 | 2.40 | N/A |
| Wan2.2-I2V-A14B-Diffusers | 197.85 | 0.32 | 192.42 | 2.19 | 4805.29 |
| MiniMax-H3 | 74.69 | 0.05 | 72.44 | 1.35 | 1463.96 |

### Latency Trend: anima_base_t2i_1024

![Latency Trend anima_base_t2i_1024](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_anima_base_t2i_1024.png)


### Latency Trend: flux1_dev_t2i_1024

![Latency Trend flux1_dev_t2i_1024](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_flux1_dev_t2i_1024.png)


### Latency Trend: flux2_dev_t2i_1024

![Latency Trend flux2_dev_t2i_1024](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_flux2_dev_t2i_1024.png)


### Latency Trend: qwen_image_2512_t2i_1024

![Latency Trend qwen_image_2512_t2i_1024](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_qwen_image_2512_t2i_1024.png)


### Latency Trend: qwen_image_edit_2511

![Latency Trend qwen_image_edit_2511](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_qwen_image_edit_2511.png)


### Latency Trend: zimage_turbo_t2i_1024

![Latency Trend zimage_turbo_t2i_1024](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_zimage_turbo_t2i_1024.png)


### Latency Trend: wan22_t2v_a14b_720p

![Latency Trend wan22_t2v_a14b_720p](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_wan22_t2v_a14b_720p.png)


### Latency Trend: wan22_ti2v_5b_720p

![Latency Trend wan22_ti2v_5b_720p](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_wan22_ti2v_5b_720p.png)


### Latency Trend: ltx2.3_twostage_ti2v_2gpus

![Latency Trend ltx2.3_twostage_ti2v_2gpus](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_ltx2.3_twostage_ti2v_2gpus.png)


### Latency Trend: ideogram4_fp8_t2i_2gpu

![Latency Trend ideogram4_fp8_t2i_2gpu](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_ideogram4_fp8_t2i_2gpu.png)


### Latency Trend: cosmos3_super_t2v_2gpu

![Latency Trend cosmos3_super_t2v_2gpu](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_cosmos3_super_t2v_2gpu.png)


### Latency Trend: wan22_i2v_a14b_720p

![Latency Trend wan22_i2v_a14b_720p](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_wan22_i2v_a14b_720p.png)


### Latency Trend: minimax_h3_t2va_5s

![Latency Trend minimax_h3_t2va_5s](https://raw.githubusercontent.com/sgl-project/ci-data-diffusion/main/diffusion-comparisons/charts/latency_minimax_h3_t2va_5s.png)


## SGLang Performance Trend (Last 7 Runs)

| Date | Commit | anima_base_t2i_1024 (s) | flux1_dev_t2i_1024 (s) | flux2_dev_t2i_1024 (s) | qwen_image_2512_t2i_1024 (s) | qwen_image_edit_2511 (s) | zimage_turbo_t2i_1024 (s) | wan22_t2v_a14b_720p (s) | wan22_ti2v_5b_720p (s) | ltx2.3_twostage_ti2v_2gpus (s) | ideogram4_fp8_t2i_2gpu (s) | cosmos3_super_t2v_2gpu (s) | wan22_i2v_a14b_720p (s) | minimax_h3_t2va_5s (s) | Trend |
|------|--------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|---------|-------|
| Oct 11 | `11bfd86` | 2.45 | 4.28 | 13.04 | 8.12 | 14.60 | 0.70 | 203.29 | 54.76 | 11.40 | 3.84 | 119.63 | 197.92 | 74.77 | :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Oct 11 | `89e24e7` | 2.45 | 4.29 | 13.06 | 8.12 | 14.56 | 0.69 | 203.14 | 54.75 | 11.91 | 3.83 | 119.53 | 197.82 | 74.69 | :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Oct 09 | `1203eb9` | 2.44 | 4.29 | 13.01 | 8.12 | 14.57 | 0.69 | 207.26 | 54.70 | 11.71 | 3.84 | 119.45 | 201.08 | 74.89 | :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_down: |
| Oct 07 | `1e86143` | 2.47 | 4.30 | 13.02 | 8.52 | 14.53 | 0.69 | 206.71 | 54.90 | 19.00 | 3.82 | 119.17 | 201.00 | 77.23 | :arrow_down:  :arrow_down:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :arrow_up:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Oct 05 | `a977e3b` | 3.25 | 4.44 | 13.05 | 8.35 | 14.81 | 0.76 | 206.51 | 55.51 | 13.53 | 3.81 | 118.43 | 200.87 | 77.07 | :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Oct 03 | `5b5d721` | 3.26 | 4.47 | 13.02 | 8.37 | 14.83 | 0.76 | 206.80 | 54.51 | 14.73 | 3.81 | 118.51 | 201.10 | 77.44 | :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :arrow_down:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow:  :left_right_arrow: |
| Oct 01 | `41cbe65` | 3.31 | 4.46 | 13.12 | 9.02 | 14.92 | 0.77 | 207.96 | 55.06 | 17.30 | 3.83 | 119.24 | 201.70 | 77.45 | -- |

---
*Generated by `generate_diffusion_dashboard.py` in SGLang nightly CI.*
