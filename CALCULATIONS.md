# CO₂ Emissions from Desktop Computer Usage

**NOTE**: These calculations are approximations and will be refined over time.

## Given Data
- Average power when in use: **200 W** (including monitor, speakers, etc.)
- Daily usage: **8 hours**
- Yearly energy consumption: **~584 kWh** (rounded to ~600 kWh in some sources)
- Yearly CO₂ emissions: **175 kg**

## Step 1 – CO₂ Emission Factor per kWh

$$
\frac{175\ \text{kg CO₂}}{584\ \text{kWh}} \approx 0.2997\ \text{kg/kWh} \quad \rightarrow \quad \textbf{≈ 300 g CO₂/kWh}
$$

## Step 2 – Energy Used in 1 Second (when ON)

$$
\text{Power} = 200\ \text{W} = 0.2\ \text{kW}
$$
$$
\text{Time} = 1\ \text{second} = \frac{1}{3600}\ \text{hours}
$$
$$
E = 0.2\ \text{kW} \times \frac{1}{3600}\ \text{h} = 5.5556 \times 10^{-5}\ \text{kWh}
$$

## Step 3 – CO₂ Emissions per Second

$$
\text{CO₂ per second} = E \times \text{emission factor}
$$
$$
\text{CO₂} = (5.5556 \times 10^{-5}\ \text{kWh}) \times (0.2997\ \text{kg/kWh})
$$
$$
\text{CO₂} \approx 1.665 \times 10^{-5}\ \text{kg/s} = \textbf{0.01665 g/s}
$$

## Final Approximation

**≈ 0.0167 grams of CO₂ per second**  
(or $1.67 \times 10^{-5}\ \text{kg/s}$) while the desktop is actively drawing 200 W.

## Important Notes
- Assumes constant **200 W** draw during active use
- Emission factor used: **≈ 300 g CO₂/kWh** (derived from the yearly data)
- Emissions scale linearly with power: idle/sleep modes produce proportionally less
- This calculation is for a **typical desktop PC + monitor**
- Laptops usually consume far less (30–90 W) → lower emissions per second

If you have more accurate power measurements or regional grid factors, feel free to contribute!  
Contact: warithkolawole@protonmail.com