# deep-learning-super-resolution# 🛰️ IADF SCHOOL: Deep Learning for Super-Resolution in Remote Sensing

![Logo](images/summer_school_2025.png)

Remote sensing is essential for understanding our planet and supports key applications such as climate monitoring, urban development, biodiversity conservation, and disaster management. With the increasing availability of data from Earth Observation (EO) satellites (e.g., Sentinel), there is a growing need for advanced image processing techniques.

**Super-resolution** is a deep learning technique that increases the spatial resolution of satellite images, helping extract finer details from low-resolution data. This enhances decision-making in areas like environmental monitoring, land use planning, and emergency response.

This repository explores deep learning-based **image super-resolution** for remote sensing, with practical notebooks, visualizations, and evaluation metrics.

---

## 💻 Software Requirements

- **Git**

  ```bash
  sudo apt-get install git
  ```

- **Visual Studio Code**  
  [https://code.visualstudio.com](https://code.visualstudio.com)

  ```bash
  sudo dpkg -i code_1.93.0-1725459079_amd64.deb
  ```

- **Anaconda**  
  [https://www.anaconda.com/download](https://www.anaconda.com/download)

  ```bash
  chmod +x Anaconda3-2024.06-1-Linux-x86_64.sh
  ./Anaconda3-2024.06-1-Linux-x86_64.sh
  source ~/.bashrc
  ```

> 💡 **Recommendation**  
> To prevent automatic activation of the base environment:
> ```bash
> conda init --reverse $SHELL  # Answer "yes" if prompted
> conda config --set auto_activate_base false
> ```

---

## 🧪 Environment Setup

This project uses a Conda environment defined in `environment.yml` for easy reproducibility.

1. Clone the repository and move into the project folder:
   ```bash
   git clone https://github.com/your-user/DEEP-LEARNING-SUPER-RESOLUTION-main.git
   cd DEEP-LEARNING-SUPER-RESOLUTION-main
   ```

2. Create and activate the environment:
   ```bash
   conda env create -f environment.yml
   conda activate dlsr-env
   ```

3. Launch Jupyter Notebook:
   ```bash
   jupyter notebook
   ```

4. In Jupyter, select the `dslr-env` kernel.

5. If new packages are added later:
   ```bash
   conda env update -f environment.yml --prune
   ```

---

## 📦 Main Dependencies

The Conda environment includes all necessary dependencies listed in [`environment.yml`](environment.yml):

- Python 3.13
- NumPy, Matplotlib, Pillow
- OpenCV
- PyWavelets, Scikit-Image, Scikit-Learn
- SciPy, Tifffile, ImageIO
- PyTorch (via pip: `torchsr`)

---

## 📁 Project Structure (example)

```
DEEP-LEARNING-SUPER-RESOLUTION-main/
├── notebooks/
│   ├── 01_upsampling_comparison.ipynb
│   ├── 02_psnr_ssim_evaluation.ipynb
├── images/
│   ├── image_hr.png
│   ├── image_lr_2.png
│   ├── summer_school_2025.png
│   └── ...
├── outputs_upsampling/
│   ├── nearest.png
│   ├── bilinear.png
│   └── ...
├── environment.yml
└── README.md
```

---

## 📫 Contact

For questions or contributions, feel free to open an issue or contact us via pull request.
