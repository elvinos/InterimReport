# Aims and Objectives

Give a background to what the project is - done as a group

\newpage

## Individual Project Aim

The aim of this individual project is to investigate the feasibility of a battery energy storage system to reduce peak energy demand charges for a new University of Bristol campus. The University’s peak demand charges will be analysed and simulated, showing how peak demand is charged in a normal use case. Different peak shaving system architectures will then be added to the model, to find an optimum solution for the system's design with respect to the system capital cost against peak demand charge savings. A comparison between using a micro system, for room by room use, or a macro system, being applied to the whole campus will be conducted. The outputs of the project for 5^th^ year will be a flexible model which produces an optimum peak shaving system architecture for a given University scenario.

## Objectives

**Literature Review**
\begin{enumerate}
\item Perform a detailed literature review to investigate applicable peak shaving technologies based on similar use cases and performance. Research will include:
    \begin{itemize}
 \item a down-selection of different energy storage solutions, looking at their applicability to a University peak shaving system, comparing parameters such as; power-ratings , discharge times, charge times and costs.
\item investigating different prediction methods for peak demand surges, identifying limitations in current technology.
    \end{itemize}
\item Conduct research of different peak shaving systems, highlighting relevant modelling techniques and limitations.
\end{enumerate}

**Definition of System Architectures**
\begin{enumerate}[resume]
\item Define peak shaving system architectures, establishing the key performance variables.
\end{enumerate}

**Modelling and Analysis**
\begin{enumerate}[resume]
\item Analyse the University’s current peak demand charges. This will include understanding the University’s current demand charge structure and collecting typical energy usage data. Parameters such as time of day and sources of energy peaks will be included.
\item Produce a simulation to optimise the peak shaving system, comparing metrics including; unit cost and reduction in peak kWh charges based on University billing structure. This model will provide a comparative analysis between the different system architectures. This will detail savings against the University’s current peak demand charges. The model will be comprised of three stages:
\begin{enumerate}
\item A simulation of the University's a normal energy use case and peak demand charges, for use as a datum.
\item Inclusion of energy storage systems, simulating logic and detailing any prediction methods.
\item Addition of other factors to improve the model, taken from the literature review. This will take into other technologies such as peak load shedding to understand if peak demand can be further reduced.
\end{enumerate}
\item Analyse others areas where the system could deliver further benefits, such as AC to DC conversion, PV’s, micro-grids and increased sustainability.
\end{enumerate}

**Evaluation**
\begin{enumerate}[resume]
\item Evaluate results of the simulation, concluding on the effectiveness of different peak shaving system architectures against particular scenarios.
\end{enumerate}

\newpage
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


## Peak Shaving Systems - Modelling Techniques
As this project is assessing the feasibility of a electrical energy storage system that reduces peak demand for the University, a review was performed to understand research into peak shaving systems. Literature around the subject is quite vast and varied, with products such as as ABB’s energy storage smart grid products, designed to perform load levelling at grid level \cite{abbpeakshave}. However these technologies are largely focused around supply levelling, using forecasting methods and large battery storage systems to offset excess supply \cite{5559470}, where micro level loads are ignored and paybacks periods on EES systems are ignored. Supply levelling technologies on a macro scale for homes can also be found in research, where the use large batteries to reduce power fluctuations brought by the use of renewable technologies. In \cite{Allik20161116}, shiftable water heating was used as a the main storage device in houses, accounting for 50% of household electricity use. Excess load from wind turbines can be used to heat water in these periods bypassing an inverter making a more efficient use of the external energy. \cite{7564619}

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
