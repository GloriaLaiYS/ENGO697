# ENGO697
ENGO697 Directed Project

## WHAT IS IT?

This model simulates the dynamics of a housing market within city of Calgary. It explores how various factors such as residences' budgets, housing prices, and proximity to amenities like train stations influence the movement of residents and the fluctuation of housing prices. The model aims to show how individual decisions at the residence level aggregate to form broader market trends.

<div align="center">
  <img style="width:500px;" src="/screenshoot1.png" alt="NetLogo Calgary Housing">
</div>
<div align="center">
  <img style="width:500px;" src="/screenshoot2.png" alt="NetLogo Calgary Housing">
</div>

## HOW IT WORKS

This model loads 3 different GIS datasets: a point file of LRT stations, a polygon file of community boundary and another polygon file of city of Calgary boundary. Residences and houses are the primary agents in this model randomly located within the city boundary.  

* Houses and Residences: Residences and houses are the primary agents in this model randomly located within the city boundary. Houses have attributes like price and proximity to train stations, the price of houses is originally decided by how close to nearest train station. While residences have budgets and a move-out timer. 

* Housing Price Adjustments: House prices adjust based on occupancy and market fluctuations. Prices increase when occupied and decrease when not, with additional adjustments based on the average residence budget. 

* Residence Movement: Residences move based on their move-out timer. When it's time to move, they choose a new house based on affordability and proximity to train stations. 

* Budget Adjustments: Residences' budgets adjust over time, also influenced by market conditions and their length of stay in a house. 

## HOW TO USE IT

Step 1: Users should firstly customize (or use default values) the initial number of houses in each community in City of Calgary by using the slider, number can range from 1 to 50. Another number users can customize is the number of residences inside the whole city, which can be chosen from 1 to 4000. User can choose the housing increase percentage from 0 to 1 from chooser to decide how the housing increases if the residence budget is higher, when the chooser = 0.1, 10% of the housing will keep increases by 2%. 

  

Step 2: Press the SETUP button. This randomly locates houses inside each community and residences with predefined attributes in Step 1. Housing price is decided by its distance to station, and the residence budget randomly ranges from 90000 to 98000. The monitor called houses per residence demonstrates the ratio of the number of houses per residence within the city.  Three other monitors indicate the Average Housing Price, Average Residence Budget and their ratio. Additionally, a button can show/ hide the name of different stations. 


Step 3: Press the GO button to start simulation and view the plot that shows average housing price and residence budget changed as movement of residence. Users can change the value of housing increase percentage chooser 



## THINGS TO NOTICE

Observe how house prices and residence budgets change over time in response to market conditions from the plot. 

Notice the patterns of residence movement, particularly in relation to train stations. 

Pay attention to how the ratio of house prices to residence budgets affects the overall market dynamics. 

## THINGS TO TRY

Change different initial number of residence and housing to have various houses per residence ratio to see how it affects the price and budget. 

Choose the housing increase percentage from 0 to 1 from chooser to decide how the housing increases if the residence budget is higher.

Observe in which situation the housing price is stable and not complied with residence budget. 

## EXTENDING THE MODEL

The model can be improved with Introducing more new factors like interest rates or economic growth indicators that impact budgets and prices. 

The number of turtles like houses and residences should be dynamic as well. As the housing price is lower, more residences turtles should be created and vice versa.  

Add more detailed behaviors to residences, such as preferences for specific communities or house types ( not all residences prefer houses close to LRT stations). 


## CREDITS AND REFERENCES

* Crooks, A., Malleson, N., Manley, E., & Heppenstall, A. (2019).https://doi.org/10.4135/9781529793543 Agent-Based Modelling & Geographical Information Systems: A Practical Primer. 

* Wilensky, U. (1999). NetLogo. http://ccl.northwestern.edu/netlogo/. Center for Connected Learning and Computer-Based Modeling, Northwestern University, Evanston, IL.

* NetLogo 6.4.0 User Manual: NetLogo Dictionary. (n.d.). https://ccl.northwestern.edu/netlogo/docs/dictionary.html

* NetLogo 6.4.0 User Manual: GIS Extension. (n.d.). https://ccl.northwestern.edu/netlogo/docs/gis.html

* NetLogo. (n.d.). Teletortoise/public/modelslib/Code Examples/GIS/GIS General Examples.nlogo at master · NetLogo/Teletortoise. GitHub. https://github.com/NetLogo/Teletortoise/blob/master/public/modelslib/Code%20Examples/GIS/GIS%20General%20Examples.nlogo
