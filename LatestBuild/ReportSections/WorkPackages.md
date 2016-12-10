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
