# Computer Carbon Footprint Estimator
A Python program using TkInter that helps you track your computer usage and provides advice for how to make your computer usage as envinronmentally friendly as possible

NOTE: This won't be 100% accurate and uses a baseline of 0.0084 for carbon emission of a computer per second, this may vary from computer to computer where this number could either be higher or lower
For that reason, you may wish to apply your existing knowledge of your computer's specs in order to estimate whether or not this number would be higher or lower, where for that reason you may choose to adjust the baseline
This would especially be the case if you have a high quality graphics card


# 📘 Conda Environment Setup

Follow the steps below to create and activate the Conda environment for this project.

---

## 1. Create Conda Environment (Python 3.14)

> ⚠️ Python 3.14 is not officially released. Use the latest available alpha through Conda.

```bash
conda create -n power-env python=3.14
```

If Conda does not recognize Python 3.14 yet:

```bash
conda create -n power-env python=3.13
```

---

## 2. Activate the Environment

```bash
conda activate power-env
```

---

## 3. Install Dependencies

### Install standard packages

```bash
pip install pandas==2.2.3
pip install numpy==2.1.2
pip install matplotlib==3.9.2
```

### Install PyTorch (Nightly CPU Build)

> Stable PyTorch does not support Python 3.14 yet.

```bash
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/nightly/cpu
```

### Optional (Linux only): Tkinter

```bash
sudo apt install python3-tk
```

---

## 📁 4. (Optional) Install Jupyter Kernel

```bash
pip install ipykernel
python -m ipykernel install --user --name power-env --display-name "Python (power-env)"
```

---

## 5. Run the Project

```bash
python main.py
```

---

# requirements.txt

```
pandas==2.2.3
numpy==2.1.2
matplotlib==3.9.2
tk
torch --index-url https://download.pytorch.org/whl/nightly/cpu
torchvision --index-url https://download.pytorch.org/whl/nightly/cpu
torchaudio --index-url https://download.pytorch.org/whl/nightly/cpu
```
