# Summary of Key Work and References

The following literature review outlines the key technologies required for developing a optimised peak shaving system and conducting research intended to justify and develop on the project objectives. Section \ref{peak-demand-charges-and-loads} looks at pricing structures, defining the problem which the system has to solve; highlighting the limitations in current commercially available technology.  Section \ref{peak-shaving-technologies} explores the technologies that can be used to define the system architecture. Finally, section \ref{peak-shaving-systems} evaluates current research of energy storage peak shaving systems, providing a reference for shortlisting different system architectures.

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

## Peak Shaving Systems
As this project is assessing the feasibility of a electrical energy storage system that reduce peak demand for the University, a review was performed to understand research into peak shaving systems. There are a few commercial products which were assessed first to give guidance on the architecture of a peak shaving system. A literature review is then given to understand research around the subject.

### Market Survey
ABB offers energy-storage, smart-grid products, perform load levelling at grid level \cite{abbpeakshave}. These systems are designed primarily for supply levelling, using forecasting methods and large electrical storage systems to offset excess supply produced from renewable energy sources \cite{5559470}. ABB’s products however, do not look at depth into reducing actual energy costs for the customer, described in section \ref{peak-demand-charges-and-loads}. One Cycle Control have created technologies to regulate peak-load and mitigate peak demand charges for commercial industrial facilities using Li-ion batteries\cite{peakload38:online}. The technology proved an effective system at reducing peak demand charges, but it's financial feasibility is limited by the cost of the storage systems \cite{Demonstr51:online}. It is clear that the ESS is the most important factor in terms of the systems cost, whilst being able to sense peak loads and respond actively will maximise the performance of the system. Section \ref{peak-shaving-technologies} will evaluate these two different technologies.

###  Peak Shaving Systems Literature Review
Understanding the limitations in current market technology, literature review was performed looking at different research around the battery type and size required to make appropriate savings, defining micro level loads on a building or even room and the effect EES’s can have at this level.

#### Forecasting
By understanding when energy prices will be greater and when loads are typically larger, a ESS can be switched on during these periods to reduce demand from the gird. Energy costs can be shifted purchasing at a cheaper rate and using this during peak times. This method, reduces peak demand through reducing the total energy demand from the grid. Looking at the gap in energy prices, demand charges and investment costs for a BESS system, for NaS, Li-ion and Flow batteries, a basic on/off algorithm to shift energy purchasing from peak to off peak times does not produce a viable return on investment (ROI) \cite{7555795}.  \cite{7555793} highlighted that billing peak periods, were directly correlated meaning that the largest demand was required at the most expensive periods, requiring large ESS to offset this demand. \cite{5590194} used real hourly spot prices to decide the best periods to turn on and off VRB and PSB batteries. Through sequential quadratic programming (SQP), the battery sizes could be optimised to finding PSB batteries have a better business case for load shifting. The key differences between \cite{5590194} and \cite{7555795}, were the reduction in the size of the problem and the granularity of the pricing data used. \cite{shen2016} and \cite{6461115} both look at different modelling techniques to simulate load shifting with EES. Using an agent-based simulation \cite{6461115}, the diversity in load consumptions patterns allowed peak demand to be reduced if all energy use is dynamic.  \cite{shen2016} look at how the peak rebate scheme may lower ROI for ESS’s. \cite{6938948} evaluated different control strategies combing multiple forecasts to reduce errors in peak shaving over a monthly period. It was found that using weighted and lowest error forecasts were the best strategies for an energy management system. \cite{Bennett2015122} added a real time operator to create and intelligent scheduling system based on a house. This system greatly improved the state of charge of the battery, allowing more energy available to reduce peaks. The research highlights that forecasts combined with real time information can increase the performance of the system further.

#### Supply Levelling
Supply levelling has been the most common use for ESS \cite{iearoadmapes}, using large batteries to reduce power fluctuations brought by the use of renewable technologies. Supply levelling works by storing excess supply, reducing peaks in supply rather than in demand. Peak sensing technology is therefore similar to peak shaving. \cite{Allik20161116}, looked at improving supply on the micro (house) scale. Shiftable water heating was used as a the main storage device in houses, accounting for 50% of household electricity use. Excess load from wind turbines can be used to heat water in these periods bypassing an inverter making a more efficient use of the external energy. Minimising conversion through invertors, makes a large difference in the efficiency of the system.

#### Battery Sizing and Financial Modelling
There have been numerous studies conducted looking into the business case for ESS technologies for industrial/ commercial and household level consumption. Models such as \cite{7555795} and \cite{7555793} look very broadly at a reduction in cost across all energy charges. Papers including \cite{1300158} and \cite{6175723} evaluated a financial models for particular case studies. Applying bespoke solution helped to maximise the peak demand reduction greater than what is promised by current generic products \cite{abbpeakshave}. This enables a strong argument that a bespoke solution for the University would have improved performance over a generic system and a much shorter ROI. Further research has indicated could be benefits for decentralised system, reducing peaks on a small scale rather than using one large central ESS.  \cite{6604477} looked at both minimising peak demand, whilst maximising the lifetime on the battery for a large data centre. Although although based in one location, the ability to forecast when a machine will spike in power usage, follows a similar to people within a building.  Through both experimentation and modelling, it was revealed that when the batteries lifespan is taking into account, being able to regulate load through a series of batteries attached to their own systems can be more favourable than a decentralised system. This idea is supported by \cite{Demonstr51:online}, where a simulation was ran of the impact of lithium-ion batteries operated under a peak-shaving control algorithm to identify cost-optimal battery configurations and their impact on metered load. \cite{Demonstr51:online} showed that small short duration batteries were much more favourable and cost effective for the customer. The model for this project will assess if this is also the case for a University facility based on it’s usage supported by evidence such as  "40% of energy use in the campus comes from 5% of the space, predominantly labs” \cite{brentemail} .

Finally \cite{20160601898032}, \cite{Levron201280} all \cite{5371839} all show alternate ways of optimising the battery sizing configuration.\cite{5371839}, using an alternate non numeric modelling method, focusing on ultra capacitors finding the optimal energy storage of fueled systems. The results emphasise the constraint of storage capacity, showing limited value gained after a specific size. This supports evidence that an optimum ESS type and size can be found for a particular use case. \cite{Levron201280} created an analytical modelling, leveraging intuitive energy band to regulate the peak load giving an optimum storage size for a given system. \cite{20160601898032} looks specifically at Vanadium Redox Flow Batteries (VRFB) arguing it’s benefits over other ESS methods. A  MATLAB/Simulink was made for a residential use case, showing that can regulate frequency effectively due to its fast response time, while still performing peak-shaving services. A more specified constrained approach to one that is proposed for this project.


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

\newpage
