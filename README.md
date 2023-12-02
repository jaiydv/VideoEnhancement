
# Video Enhancement Project

## Overview

This project focuses on enhancing the quality of a video by upscaling its resolution and reducing noise. The primary goal is to achieve significant improvements in video quality, particularly by increasing its resolution and eliminating unwanted noise. The project uses the capabilities of a suitable model, similar to [TensorPix AI](https://tensorpix.ai/).

## Prerequisites

- Python
- [GFPGAN](https://github.com/TencentARC/GFPGAN): A Generative Face Perfector for High Fidelity Face Image Synthesis
- [MoviePy](https://zulko.github.io/moviepy/): A Python module for video editing

## Sample Input and Sample Output

### output 
![image](https://github.com/jaiydv/VideoEnhancement/assets/85070747/40a46405-2e98-419c-b86c-17abbae9dc6e)  ![image](https://github.com/jaiydv/VideoEnhancement/assets/85070747/d4944198-9d0e-4f6f-ac3d-34bf7f1310fb)





## Usage

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/yourusername/VideoEnhancement.git
   cd VideoEnhancement
   ```

2. **Install Dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run Video Enhancement:**

   Run the Assignment-3.ipynb 

   This notebook processes the input video, upscales its resolution, and reduces noise and it also contains the logic for evaluation metrics

Certainly! You can add a section to your README to include information about the evaluation metrics used, such as PSNR (Peak Signal-to-Noise Ratio). Here's an example:

---

# Video Enhancement Project

...

## Evaluation Metrics

### PSNR (Peak Signal-to-Noise Ratio)

Peak Signal-to-Noise Ratio is a commonly used metric to evaluate the quality of reconstructed images or videos. It measures the ratio between the maximum possible power of a signal and the power of corrupting noise that affects the quality of its representation.

In the context of video enhancement, PSNR can provide insights into the quality improvement achieved by comparing the enhanced video frames with the original frames.

### Result of given inputs
Average Psnr values of given videos

1. Test1.mp4 - 35.616481395426824 dB
2. Test2.mp4 - 37.27242529287235 dB
3. Test3.mp4 - 37.27242529287235 dB

#### How to Calculate PSNR

The formula for calculating PSNR is as follows:

\[ PSNR = 10 \cdot \log_{10}\left(\frac{{\text{{MAX}}^2}}{{\text{{MSE}}}}\right) \]

Where:
- \(\text{{MAX}}\) is the maximum possible pixel value of the image or video frames (usually 255 for 8-bit images).
- \(\text{{MSE}}\) is the Mean Squared Error between the original and enhanced frames.

### Example Usage

```bash
run the Evaluation cell of Assignment-3.ipynb
```

This script calculates the PSNR between corresponding frames of the original and enhanced videos.

---

## Project Structure

- `inference_gfpgan.py`: Script for running GFPGAN inference on video frames.
- `Assignment-3.ipynb`: Colab notebook to run the file
- `frames/`: Folder to store video frames.
- `restored_imgs/`: Folder to store restored video frames.
- `results/`: Folder to store final video outputs.

## How to Run

1. Place your input video  in the `results/` folder.
2. Run the video enhancement cell of Assignment-3.ipynb.

## Results

The enhanced video (`final_result.mp4`) will be available in the `results/` folder.


## License

This project is licensed under the [MIT License](LICENSE).

---
