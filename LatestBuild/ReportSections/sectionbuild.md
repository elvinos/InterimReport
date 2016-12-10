# Aims and Objectives

The announcement of the new £300million University of Bristol Campus in Temple Quarter \cite{November58:online}, presents an exciting new opportunity for development of digital innovations in sustainable energy. The government's 2020 smart meter rollout, is the first step for creating a smart energy grid, key to achieving a low-carbon, efficient energy for the UK \cite{SmartEne79:online}. The UK's vision is inline with the University of Bristol's new strategy, seeking to boost it's world-class research capacity and promote policy innovation in sustainability \cite{universi93:online}. Create a world leading sustainable digital campus, holds as an attractive means for the University to achieve it's vision. Consequently, aim of the group project is to bring a host of new digital technologies reducing both energy costs and energy usage, uniting these themes, to radically increase the new campus's sustainability.

\begin{figure}[H]
\centering
\includegraphics[width=1\textwidth]{groupDia}
\caption{Group Design Project Diagram Showing Relationships Between Individual Projects}
\label{groupDia}
\end{figure}

Figure \ref{groupDia} shows how the separate themes of the project are split, where research in Occupancy Sensing, Smart Metering and Building Services will evaluate how energy usage in the new campus can be optimised. District Heating, Energy Pricing and Peak Demand Reduction, all analyse methods of reducing energy costs for the University. Where new energy pricing structures coupled with peak demand reduction technologies, can reduce the load on the grid, helping support sustainable energies. When these separate streams are brought together in 5^th^^ year, a smart "brain" will be created, combining usage data with reduction in energy costs to provide sustainable energy services to the campus in that will push the University to meet it's carbon neutral 2030 goal \cite{universi93:online}.

## Individual Project Aim

The aim of this individual project is to investigate the feasibility of a battery energy storage system to reduce peak energy demand charges for a new University of Bristol campus. The University’s peak demand charges will be analysed and simulated, showing how peak demand is charged in a normal use case. Different peak shaving system architectures will then be added to the model, to find an optimum solution for the system's design with respect to the system capital cost against peak demand charge savings. A comparison between using a micro system, for room by room use, or a macro system, being applied to the whole campus will be conducted. The outputs of the project for 5^th^ year will be a flexible model which produces an optimum peak shaving system architecture for a given University scenario.

## Objectives

**Literature Review**
\begin{enumerate}
\item Research different peak shaving systems available on the market and similar systems designs in literature, highlighting relevant modelling techniques and limitations.
\item Perform a detailed literature review to investigate applicable peak shaving technologies based on similar use cases and performance. Research will include:
    \begin{itemize}
 \item a down-selection of different energy storage solutions, looking at their applicability to a University peak shaving system, comparing parameters such as; power-ratings , discharge times, charge times and costs.
\item investigating different prediction methods for peak demand surges, identifying limitations in current technology.
    \end{itemize}
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
# Background and Summary of Key Work and References

The following literature review provides a comprehensive overview of current research into using Energy Storage Systems (ESS) to reduce peaks in energy demand and lower utility costs for the consumer. Peak demand reduction is synonymous with peak shaving; the ability to control energy usage from a supplier during intervals of high demand, to limit or reduce demand charges\cite{schneiderRECPS}. As this project is investigating reducing the peak demand charge for the University of Bristol, a thorough understanding of the charging structure is given in section \ref{peak-demand-charges}, providing context for the system to solve.  Section \ref{current-peak-demand-management-methods-and-energy-storage-systems-usage} evaluates traditional methods of peak shaving, covering a brief look at ESS's current usage. Section \ref{peak-shaving-systems-literature-review} includes a broad range of research around using ESS in different case studies, optimising the system architecture and analysis on ESS's financial return on investment (ROI). This research will help in defining the system architecture to be modelled, highlighting relevant modelling techniques to consider while showing the limitations in current research. Finally section \ref{peak-shaving-technologies---electrical-storage-system-ess} analyses the applicability of different ESS's, down-selecting to leave a shortlist of ESS's to be modelled.

## Peak Demand Charges
The University of Bristol's infrastructure, spans across three sites; the City Centre, Stoke Bishop and Langford. Across these places, the majority of facilities receive separate energy bills, allowing a high degree of granularity in the understanding energy charges \cite{Jbrentmeet}. These costs are broken down into several factors, where many separate bills are bundled together under the same theme
\cite{Jbrentmeet}. These different charges are:
\begin{multicols}{2}
\begin{enumerate}
\item Unit Charge
\item Distribution Use of System (DUoS)
\item Feed-In Tariff (FIT)
\item Transmission Network Use of System (TNUoS)
\end{enumerate}
\end{multicols}

The charges that peak-shaving system will target are DUoS, TNUoS and Unit Cost (by secondary means). DUoS charges include the capacity charge; where the customer pays for a maximum energy demand level that the institution will not exceed \cite{Deconstr52:online}. The capacity charge is set at a bar higher than the actual maximum demand, reducing the risk of breaching this threshold. If breached, the customer incurs substantial penalties, and the supplier increases the threshold for the next billing period. By levelling off peaks in energy demand, the capacity charge threshold can decrease; this will be the key focus for the peak-shaving system.  

TNUoS charges come from three half-hour periods when the UK's National Grid energy demand is greatest, referred to as Triads. These dates lie between November and February and must be separated by at least ten days during the financial year, calculated yearly \cite{TriadsWh7:online}. The average maximum (peak) demand across the three Triad periods \cite{TNUoSTra99:online}, is multiplied by tariff in the respective zone in cost per kW \cite{TNUoScha93:online}. Combined they become the TNUoS charge, added to the customer's end of year bill. Being able to radically reduce peaks through using ESS or generation in these periods will reduce the bills cost significantly.

Energy unit costs come at three different rates, green, amber and red \footcite[See page 27 of][]{SWEB201492:online}, depending on the time of day; where energy usage in red periods are significantly higher (generally between 5pm-7pm). Section \ref{forecasting} discusses literature around these charges.

## Current Peak Demand Management Methods and Energy Storage Systems Usage

Traditionally there are two methods for reducing peak demand for industrial complexes. These are:

* **Load Shedding**: This is reducing energy usage, by understanding which parts of the system can be switched off during periods of peak demand \cite{6199851}. Scheduling can be an intelligent system or use simple forecasting tool \cite{Reducing37:online}. Often load shedding is calculated daily using a schedule to set the maximum limit; assuming that this limit will not change during the day \cite{6938948}.
    * *Limitations*: This method can typically lead to significant forecasting errors were reactive methods are often is better \cite{6938948}. Due to the free flow of staff and students at the University's facilities, predicting peak demands accurately can become a greater challenge.
* **On-site Generation**: Adding of the grid capacity to the consumer \cite{schneiderRECPS}. The university currently uses some generators to reduce red zone unit charges.
    * *Limitations*: The University currently has 0.5MW of PhotoVoltaic (PV) installed using nearly all available space. These PV's make up only 0.5\% of the total energy demand \cite{Jbrentmeet} meaning on-site generation to offset peak demand has a negligible effect in flattening the University's demand in it's standard form.

Due to these limitations and statistics such as "40% of energy use in the campus comes from 5% of the space, predominantly labs” \cite{brentemail}, make the University an interesting case study how developments in ESS, could present a better method of reducing peak demand charges.

There are a limited number of peak shaving ESS solutions available commercially. ABB offers energy-storage, smart-grid products, perform load levelling at grid level \cite{abbpeakshave}. These systems are designed primarily for supply levelling, using forecasting methods and large electrical storage systems to offset excess energy supply produced from renewable energies \cite{5559470}, rather than targeting bill reduction for its' customer. One Cycle Control have created technologies to regulate peak-load and mitigate peak demand charges for commercial/industrial facilities using Li-ion batteries \cite{peakload38:online}. The technologies proved effective at reducing peak demand charges, but the cost of the ESS \cite{Demonstr51:online} reduces their financial feasibility. It is clear that the ESS selected the most important factor regarding the systems cost while being able to sense peak loads and respond actively will maximise the performance of the system. Section \ref{peak-shaving-technologies---electrical-storage-system-ess} evaluates these two different technologies.

##  Peak Shaving Systems Literature Review
Acknowledging limitations in commercial ESS technology, a literature review was performed investigating research relevant to designing a peak-shaving system architecture using an ESS. Research is grouped, highlighting each section's significance to achieving the objectives of the project.

### Forecasting and ESS in Load Shifting
By understanding when energy prices will be greater and when loads are typically larger, an ESS can be switched on during these periods to reduce demand from the grid. Energy costs are shifted, purchasing energy at cheaper rates and using this energy during peak times. For western power, there is a 17000\% increase in price during this period \footcite[25.405 p/kWh in red times to 0.147p/kWh in green times][]{SWEB201492:online}. Looking at the gap in energy prices, demand charges and investment costs for an ESS, for NaS, Li-ion and Flow batteries, a basic on/off algorithm to shift energy purchasing from peak to off-peak times does not produce a viable return on investment (ROI) \cite{7555795}.  \cite{7555793} highlights that billing peak periods were directly correlated with peak demand, requiring large ESS to offset this demand. \cite{5590194} used real hourly spot prices to decide the best times to turn on and off Vanadium Redox Batteries (VRB) and  Polysulfide Bromide Batteries (PSB). Through sequential quadratic programming (SQP), battery sizes were optimised, finding PSB's had a better business case for load shifting. The fundamental differences between \cite{5590194} and \cite{7555795}, were the reduction in the size of the problem and the granularity of the pricing data used. \cite{shen2016} and \cite{6461115} both look at different modelling techniques to simulate load shifting with EES. Using an agent-based simulation, \cite{6461115} was able to reduce the diversity in load consumptions patterns, consequently reducing peak demand, creating an active market to trade energy demand.  \cite{shen2016} looked at how the peak rebate scheme may lower ROI for ESS’s. Neither modelling methods are appropriate for this project. \cite{6938948} evaluated different control strategies combining many forecasts to reduce errors in peak shaving over a monthly period. Weighted and lowest error forecasts were the best strategies for an energy management system and should be added to the system architecture if forecasting is used. \cite{Bennett2015122} added a real-time operator to create and intelligent scheduling system based on a house to forecast. This system significantly improved the state of charge of the battery, allowing more energy available to reduce peaks, highlighting that forecasts combined with real-time information can increase the performance of the system further.

### Supply Levelling
Supply levelling has been the most common use for ESS \cite{iearoadmapes}, using large batteries to reduce power fluctuations brought by the use of renewable technologies. Supply levelling works by storing excess supply, reducing peaks in supply rather than in demand. The technology is, therefore, similar to peak shaving. \cite{Allik20161116} looked at improving supply on the micro (house) scale. Shiftable water heating was used as the primary storage device in houses, accounting for 50% of household electricity use. Excess load from wind turbines can be used to heat water in these periods bypassing an inverter making a more efficient use of the external energy. Minimising conversion through invertors makes a large difference in the efficiency of the system.

### Battery Sizing and Financial Modelling
There have been numerous studies conducted looking into the business cases for ESS's. \cite{7555795} and \cite{7555793} model a broad use of using ESS's to reduce the cost of all energy charges, finding that the ROI is unlikely to be feasible until 2020. Papers including \cite{1300158} and \cite{6175723} evaluated financial models for particular case studies, showing that bespoke solutions achieved greater peak shaving reductions than returns promised by current generic products \cite{abbpeakshave}. \cite{7555795}, \cite{7555793}, \cite{1300158} and \cite{6175723}  enable a strong argument that a bespoke solution for the University offer a better business case for ESS than commercial technology.

Investigating the benefits of a decentralised system, reducing peaks on a small scale rather than using one large central ESS,  \cite{6604477} analysed both peak shaving and battery longevity for a large data centre. The ability to forecast when a machine will spike in power usage follows a similar to people within a building.  Through both experimentation and modelling,  \cite{6604477} showed that when regarding the batteries lifespan, the ability to regulate load through a series of batteries can be more favourable than a centralised system.  \cite{Demonstr51:online} supports using a decentralised system. A simulation of the impact of lithium-ion batteries operated under a peak-shaving control algorithm identified the cost-optimal battery configurations, and their impact on grid demand revealing that small short duration batteries was more favourable and cost effective for the customer. The model for this project will assess if this is also the case for a University facility understanding that a few rooms such as labs contribute to the majority of peak loads.

\cite{20160601898032}, \cite{Levron201280} all \cite{5371839} all show alternate ways of optimising the battery sizing configurations. \cite{5371839}, used a non-numeric modelling method, focusing on ultra-capacitors to find the optimal ESS. The results emphasised the constraint of storage capacity, showing that limited value is gained after a particular size of ESS is used. Finding this size for the University will be the primary focus of this projects model.  \cite{Levron201280} created an analytical modelling, leveraging intuitive energy bands to regulate the peak load giving an optimum storage size for a given system, a simple and effective method of modelling battery usage. \cite{20160601898032} looked specifically at Vanadium Redox Flow Batteries (VRFB) arguing it benefits over other ESS methods. A  MATLAB/Simulink was made for a residential use case, showing that VRFB can regulate it's frequency efficiently, due to its fast response time, while still performing peak-shaving services. A more specified approach to \cite{20160601898032} model is proposed for this project.

## Peak Shaving Technologies - Electrical Storage System (ESS)

The chosen Electrical Storage System (ESS) is the chief technology which will affect the cost and feasibility of a peak shaving system, where of these technologies are not suitable for a University peak-shaving system. An ESS converts electrical energy into a form stored for later use \cite{Chen2009291}.  Electrochemical batteries characterise a pollution-free operation, low maintenance, high round-trip efﬁciency, long cycle lives, batteries arguably being the most appropriate technology for peak shaivng\cite{liao2016a} \cite{Dunn928}. These have been chosen as the main focus for this study. The various storage methods can be characterised for different uses summaries below:

* **Energy Management:** for large scale storage, these are typically used by power plants for load levelling, ramping/load following, and spinning reserve.
    * Pumped Hydroelectric Storage (PHS), Compressed Air Energy Storage (CAES) and Cryogenic Energy Storage (CES) are the conventional technologies for high generation above 100MW. All these methods are on a scale too large to be considered for this project.
    * Large-scale batteries, flow batteries, fuel cells, solar fuels, CES and Thermal Energy Storage (TES) are suitable for medium-scale energy management with capacities of 10–100 MW. These are appropriate for consideration for this project.
* **Power quality:** For fast response times for power quality such as the instantaneous voltage drop, flicker mitigation and short duration uninterrupted power supply
    * Flywheels, Batteries, Superconducting Magnetic Energy Storages (SMES), capacitors and supercapacitors have millisecond response time lower for storage sizes less than 1 MW - suitable perhaps in addition to large scale battery, flywheel efficiency, however, is too low for operational use, so has been removed from this study.
* **Bridging power:** Relatively fast response (< 1 s) but also have relatively long discharge time (hours). The typical power rating for these types of applications is about 100 kW–10 MW.
    * Batteries, flow batteries, fuel cells and Metal-Air cells
\cite{Chen2009291}

By removing energy storage methods that would not be appropriate for the system, a table was created to compare the differing technologies, included in the appendix. Batteries along with capacitors provide the response time and efficiencies required to make the system justifiable, where only rechargeable batteries were compared. From section \ref{battery-sizing-and-financial-modelling} a model of a University peak demand reduction system will need to compare different battery parameters along with their cost, to optimise the model.

\newpage
# Project Work-plan

This section describes the breakdown of the different work packages required to complete the aims and objectives set out in section \ref{aims-and-objectives}.

#### Work Package 1: Literature Review (Objectives 1 and 2)

\begin{enumerate}[ label={1.\arabic*}]
\item Understand the University's energy pricing structure, defining the problem the peak shaving system will solve.
\item Perform a market survey of peak shaving systems available commercially and review literature of relevant research around peak shaving systems.
\item Evaluate different energy storage systems, looking at metrics including; power-ratings , discharge times, charge times and costs. Producing a shortlist of relevant ESS's to be modelled .\\ \textit{Output:} Table defining EES parameters shortlisted.
\item Evaluate prediction methods for peak demand surges, understanding limitations in current technology providing parameters to be modelled.
\end{enumerate}

#### Work Package 2: Definition of System Architectures (Objective 3)

\begin{enumerate}[ label={2.\arabic*}]
\item Investigation and of different peak demand sensing methods
\item Investigation of smart metering technologies
\item Investigation of energy conversion technologies and further methods of splitting supply between energy storage devices and the grid
\item Investigate storage health monitoring and it's effects on a peak shaving system
\item Investigation of different ESS locations to be modelled, comparing decentralised and centralised formats
\item Quantitive assessment of key parameters of different peak shaving technologies, down-selecting most feasible options to be modelled
\item Establish a set of system architectures to be modelled.
\end{enumerate}

#### Work Package 3: Analysis University Peak Demand Charges (Objective 4)

\begin{enumerate}[ label={3.\arabic*}]
\item Collect data on the University's energy usage
\item Collect data on University energy charges relevant to peak demand
\item Analyse data, identifying any key trends such as time of day peaks, or locations peak usage comparing to costs.
\item Investigate best practices to create representative model of the University's energy data.
\end{enumerate}

#### Work Package 4: Simulation of System Architectures (Objective 5)

\begin{enumerate}[ label={4.\arabic*}]
\item Create a simulation of the University's a normal energy use case and peak demand charges, showing a accurate profile of how the University is charged
\item Add of energy storage systems, simulating logic and detailing any prediction methods taken from WP2.
\item Add further technologies such as peak load shedding to understand if peak demand can be further reduced cost effectively.
\item Run model for different locations in the campus quantitively comparing the difference between a decentralised and centralised systems
\end{enumerate}

#### Work Package 5: Evaluation of Simulation (Objective 6 and 7)

\begin{enumerate}[ label={5.\arabic*}]
\item Evaluate other areas where the system can provide further benefit to the University campus, including micro-grids and PV's.
\item Evaluate results of the simulation, concluding on the effectiveness of different peak shaving system architectures.
\end{enumerate}

#### Work Package 6: Conclusions and Further Work

\begin{enumerate}[label={6.\arabic*}]
\item Identify all findings from work packages, condensing findings to provide recommendations and identify areas for future work
\item Identify transition points for the projects integration into the $5^{th}$ year group project.
\item Final report write up
\item Group project poster creation
\end{enumerate}

A Gantt Chart for the project has been included below.

\newpage

\begin{landscape}

\begin{figure}[H]
\centering
\includegraphics[height=0.92\textwidth]{GanttChartDP.pdf}
\caption{Gantt Chart, Detailing Project Timeline}
\label{GanttChart}
\end{figure}

\end{landscape}

\newpage


# Project Resources

The following section highlights the resources required to complete this individual project.

* **MATLAB and Simulink software** - This will be used to create the simulation of the peak shaving system
    * Available under the University student license, already installed
    * Modelling support, including additional training sessions from Mike McCann (A University of Bristol modelling specialist) in order to fully use the software
* **MS Excel** - This will be used for tabulating data, down-selecting selecting energy storage systems and developing cost- benefit analysis models
* **University Energy Usage Data** - To be obtained from the University estates department, John Brenton and Chris Jones
* **University Energy Charges Data** - To be obtained from the University estates department, John Brenton and Chris Jones
* **Arup Support and Expertise** - Guidance from in-house experts to maximise quality of research in WP2. This can be obtained through contacting Peter Cooper (Project Industrial Sponsor).

# Project Risks

This sections highlights the key project risks that this individual project may encounter. Included with the risks are mitigations strategies, chosen to reduce the consequences if these risk's occur, see table \ref{risktab}. Risks are measured using the IPTQ method, explained below:

* \textbf{P}: Probability of occurrence, \textit{1=low, 2=medium, 3 = high}
* \textbf{T}: Time delay caused by risk, \textit{1=low, 2=medium, 3 = high}
* \textbf{Q}: Negative effect on quality of work, \textit{1=low, 2=medium, 3 = high}
* \textbf{I}: Impact of risk, $I=P\times$ $(T+Q)$

The quality of the mitigation is measured by the percentage reduction in the risk's impact:

\begin{eqnarray}
 \%Reduc =\frac{\text{Impact pre-mitigation}-\text{Impact post-mitigation}}{\text{Impact pre-mitigation}}   \nonumber
\end{eqnarray}


\newpage

\begin{landscape}

\begin{table}[H]
\centering
\caption{Table Showing the Project Risks and Mitigations}
\includegraphics[height=0.8\textwidth]{risktab.eps}
\label{risktab}
\end{table}

\end{landscape}
