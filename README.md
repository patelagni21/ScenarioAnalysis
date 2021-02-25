# ScenarioAnalysis
Vehicle scenario analysis (65 points) The purpose of this assignment is to build an analysis model to explore what-if  scenarios when buying a new car. We will consider two types of vehicles on the market:

Gasoline powered vehicles that operate solely using gasoline.
Fully electric vehicles that operate solely on battery-stored power and use no gasoline. The batteries are charged by plugging in to an external power source.
Considering Cost
Some of the main considerations that factor into the decision when looking for a car might include:

Cost
Convenience
Driving experience
Environmental reasons

Of the factors above, which ones can be quantified in some way? Which are more qualitative preferences? In this case, convenience and driving experience are qualitative, but cost and environmental impact (in terms of CO2 emission) can be quantified. To build a model to help with your decision, we’ll begin with the things that can be quantified. Since it is most familiar, let’s start with cost.

To simplify our model assume leased cars only. To lease a car we consider the amount due at signing, the number of months for the entire lease, the monthly cost, the milage allowance in 12 months, and the excess mileage cost per mile. We also consider the price of gas for gasoline-powered vehicles and electricity for eletricity-powered vehicles to drive the cars for the lease term.

Considering Carbon
Many people choose to buy an electric car, not because of cost but out of concern for the environment. This is a benefit that is difficult to fully capture, but certain things like greenhouse gas emissions can be measured.

Greenhouse gases (GHGs) trap heat in the Earth’s atmosphere and are believed to contribute to global climate change. Carbon dioxide (CO2) is the main GHG produced by human activity, and the two major human activities responsible for CO2 emission are electric power generation and combustion of fossil fuels for transportation. You can read a little more about CO2 emission on the EPA website.

According to the EPA, there are 8.887 kg of CO2 released with the combustion of each gallon of gasoline. This is the amount of CO2 coming out the tailpipe of a gas powered vehicle.

This means that we can estimate the total CO2 emitted over the three-year lease of a vehicle. Assuming the vehicle consumes 1 gallon of gas for every 34 miles and that the lease allowance milage is 12,000 miles per year, we can compute the number of gallons of gasoline needed to drive an estimated 36,000 miles and multiplying by 8.887kg/gal as follows:

36,000mi/(34 mi/gal) x 8.887 kg/gal = 1,058.82 gal x 8.887kg/gal = 9,409.76kg.

To drive 36,000 miles, the vehicle uses 1,058.82 gallons of gasoline and produces 9,409.76 kg of CO2.

You can do this same calculation for any gas-powered car by plugging in the number of miles driven (M) and the fuel efficiency of the vehicle in miles per gallon (N).


To figure out how much CO2 is emitted in generating the electricity to charge the battery of an electricity-powered car over a three-year lease, let’s begin by estimating the total energy for battery charging needed to drive 36,000 miles. Assuming that it takes 60kWh to fully charge the car and that the car can drive for 238 miles per charge we estimate the total energy needed for battery charging needed to drive 36,000 miles is:

36,000 mi/(238 mi/charge) x 60 kWh/charge = 9,075.6 kWh.

According to the EPA’s Power Profiler website, 998.4 pounds of CO2 are emitted per mWh on average across the United States.

Converting units, there are about .45kg per pound, resulting in the following total CO2 emission in kg to power the car:

9,075.6 kWh * [ 998.4 lbs CO2/ MWh * 1MWh/1000Kwh * 0.45kg/lb ] = 4077.5 kg/CO2

Given all of this, we now have the capability to estimate the CO2 emission resulting from driving an electric vehicle. It boils down to plugging in the number of miles driven (M), battery storage capacity (E), and the driving range on a charge (R) into the following equation.


This equation looks hairy, but we can deconstruct it by noticing that the quantity in brackets on the left is electricity consumption, and the quantity in brackets on the right is essentially just unit conversions to get us from kWh of electricity to kg of CO2.

Given Equation 2 and Equation 1 from the previous section, we can figure out the CO2 emissions from any gas-powered car and any electric car, and that’s what we will do now.
