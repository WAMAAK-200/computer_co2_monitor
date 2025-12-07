# Computer Carbon Footprint Estimator
A Python program using TkInter that helps you track your computer usage and provides advice for how to make your computer usage as envinronmentally friendly as possible

> **Warning: Accuracy Note**
> 
> This tool is an **estimate** — it uses a baseline of **0.00001665 kg** (0.01665 g) of CO₂ **per second** while your computer is on.
> 
> Real emissions vary significantly depending on your hardware:
> - **Laptops**: often **lower** (0.004–0.010 g/s)
> - **Typical desktops + monitor**: ~0.01665 g/s (our default)
> - **Gaming PCs / workstations with high-end GPUs**: often **much higher** (0.03–0.05+ g/s)
> 
> **You can (and should!) adjust the value in the app** if you know your system’s actual power draw (e.g. from a watt meter, BIOS, or tools like HWMonitor).

# Computer CO₂ Monitor 🖥️🌍

**Real-time carbon footprint tracker for your laptop or desktop** — built with Python + Tkinter.

Tracks how much CO₂ your computer emits **every second** based on actual power draw and your country's electricity grid.

![](assets/screenshot.png)  
*(Live counter in action — 0.016 g CO₂ per second on a typical desktop)*

### Why This Matters
- A typical desktop (200 W) used 8 hours/day emits **~175 kg CO₂ per year**
- That's like driving **700 km** in an average car
- Small habits (sleep mode, lower brightness, efficient hardware) = big savings

---

### Accurate CO₂ Calculation (Per Second)

Based on real-world data:

| Assumption                    | Value              | Notes                                  |
|-----------------------------|--------------------|----------------------------------------|
| Average power (on, with monitor) | **200 W**         | Includes typical desktop + monitor     |
| Daily usage                   | 8 hours            | Standard office/gaming day             |
| Yearly energy                 | ~584 kWh           | 200 W × 8 h × 365 days                 |
| Yearly CO₂ emissions          | **175 kg**         | Common global estimate                 |

#### Emission Factor
$$
\frac{175\ \text{kg CO₂}}{584\ \text{kWh}} \approx \textbf{0.300 kg/kWh} \quad (300\ \text{g/kWh})
$$

#### CO₂ per Second (when powered on)
$$
\text{Power} = 0.2\ \text{kW},\quad \text{Energy per second} = 0.2 \times \frac{1}{3600}\ \text{h} = 5.556 \times 10^{-5}\ \text{kWh}
$$
$$
\text{CO₂} = (5.5556 \times 10^{-5}\ \text{kWh}) \times (0.2997\ \text{kg/kWh}) \\
\approx 1.665 \times 10^{-5}\ \text{kg/s} = \textbf{0.01665 g/s}
$$

**Your computer emits ~0.01665 g CO₂ every second it's on.**

> **Laptops**: Use ~50–90 W → only **0.004–0.008 g/s**  
> **Gaming PCs**: Can exceed 500 W → up to **0.04+ g/s**

---

### Features
- Live second-by-second CO₂ counter
- Adjustable power profile (laptop, desktop, gaming rig)
- Region-based grid emission factors (coming soon)
- Eco tips to reduce your footprint
- Built on real hardware data (SPECpower benchmarks)

---

### Quick Start

```bash
# Clone and enter
git clone https://github.com/WAMAAK-200/computer_co2_monitor.git
cd computer_co2_monitor

# Install dependencies
pip install -r requirements.txt

# Run
python src/main.py
```
