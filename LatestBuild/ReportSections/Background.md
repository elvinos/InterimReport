# Summary of Key Work and References

The following literature review outlines the key technologies required for developing a optimised peak shaving system and conducting research intended to justify and develop on the project objectives. Section \ref{peak-demand-charges-and-loads} looks at pricing structures, defining the problem which the system has to solve; highlighting the limitations in current commercially available technology.  Section \ref{peak-shaving-technologies} explores the technologies that can be used to define the system architecture. Finally, section \ref{peak-shaving-systems---modelling-techniques} evaluates current research of energy storage peak shaving systems, providing a reference for shortlisting different system architectures.

## Peak Demand Charges and Loads

### Pricing Structure
* A charge based on a price per kW, typically the peak kW of the billing period\cite{schneiderRECPS}
* Calculated using demand intervals, a short timeframe (often 15 minutes) during which overall usage is aggregated and tracked as a total
    * The average calculated is the kW demand for this period
* Peak Shaving is the ability to control your usage from a supplier during intervals of high demand, in order to limit or reduce demand penalties for the billing period
* After generation costs these are generally the second largest cost per kWh on an energy bill

### Current Peak Demand Management Techniques

* To reduce peak demand, you will want to do electrical load planning and management. What this means, simply, is scheduling the use of electrical equipment to get the work done at the lowest possible electric load at any one time \cite{Reducing37:online}
* Key two main methods:
    * Reducing usage through load shedding- understands which parts of the system can be switched off during periods of peak demand  - these can be intelligent \cite{6199851}
    * Adding capacity with on-site generation \cite{schneiderRECPS}

### Typical Loads

* A major factor is how to handle surge loads. Surge loads occur when large electric motors are started. These large motors can draw  ve times normal operating current for a short period of time. It is usually necessary to use some type of load starting device such as a soft starter or to start the motors sequentially \cite{baldorPS}.

## Peak Shaving Technologies


### Electrical Energy Storage (EES) System

The chosen Electrical Energy Storage (EES) System is the main technology which will effect the cost and feasibility of a peak shaving system. where of these technologies are not suitable for a University peak shaving system. An Electrical Energy Storage (EES) is the process of converting electrical energy into a form that can be stored for later use \cite{Chen2009291}. There are various energy storage technologies available for large-scale applications which can be divided into four kinds, i.e. mechanical, electro-magnetic, chemical and electrochemical.

Due to the inherent properties of mechanical and These technologies into different use cases, categorised as:

* **Energy Management:** for large scale storage, these are typically used by power plants for load leveling, ramping/load following, and spinning reserve.
    * PHS, CAES and CES are the typical technologies for high generation above 100MW - these methods are on a scale to large to be considered for this system
    * Large-scale batteries, flow batteries, fuel cells, solar fuels, CES and TES are suitable for medium-scale energy management with a capacity of 10–100 MW, are appropriate for consideration for this system
* **Power quality:** For fast response times for power quality such as the instantaneous voltage drop, flicker mitiga- tion and short duration UPS
    * Flywheel, batteries, SMES, capacitor and super-capacitor millisecond response time lower than 1 MW - suitable perhaps in addition to large scale battery, flywheel efficieny to low for operational use.
* **Bridging power:** Relatively fast response (< 1 s) but also have relatively long discharge time (hours) The typical power rating for these types of applications is about 100 kW–10 MW.
    * Batteries, flow batteries, fuel cells and Metal-Air cells
\cite{Chen2009291}
By removing energy storage methods that would not be appropriate for the system, a table was created to compare the differing technologies. Due to only batteries and capacitors providing the response time and efficiencies required to make the system justifiable, only rechargeable batteries were compared. It is apparent from the literature review that the model of a University peak demand reduction system will need to compare different battery parameters along with their cost, in order to optimise the model.

### Peak Demand Sensing

* Two systems, fixed scheduled and anticipated \cite{20164002874437} - good citation for university modelling
* Online framework will continuously monitor the real-time demand reduction whilst actively perform peak demand reduction
    * Required supply  from battery for the next interval is defined, in which to reduce the mean absolute percentage error (MAPE) it is computed by bringing the scheduled profile towards the forecasted supply, by an approximate factor
    * Four zones in which the battery acts, that is charge, discharge, standby and idle. standby is where the battery is boost supplying
    * Boundaries are set for predicted peak
    * forecasted and present demand misalignment is reduced, fluctition along the threshold is minimised and energy is conserved only at an interval of potential peak demand.
    * These use a method of taking power off the grid at an off peak time
    * Thresholds are adjusted accordingly
    * Both active and passive work , but peak reduction is much more consistent for active
    * Where the real-time active control strategy achieved percentage reduction of up to 8.64%, with accuracy of 70.52% or percentage difference of 29.48% away from the ideal reduction and has percentage performance of 77.08% in achieving the peak demand reduction.

## Peak Shaving Systems - Modelling Techniques

* \cite{Leadbetter2012685} This reference looks at using using a generic battery technology with an investor and controller
