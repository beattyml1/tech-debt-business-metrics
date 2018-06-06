Technical Debt Business Metrics and Calculations
================================================
### Given 
time_cost = person months spent on fix/refactor/project total including training and any temporary lost efficiency 

total_improvement = specific to scenario

### Then 

payoff_period = time_cost / total_improvement

roi_amount (months) = (total_improvement * roi_period) - time_cost

roi_percent = roi_amount /time_cost

To combine multiple sources of improvement

total_improvement = sum(improvements)


Efficiency Improvements
=======================

### Given

efficiency_loss = fraction of development time lost to technical debt/issues being addressed 

percent_improvement = percent reduction in efficiency loss expected to acheived by this fix/refactor/project expressed as fraction/decimal

n = number of developers impacted

roi_period = period over which to evaluate ROI

### Then

total_improvement = (efficiency_loss * percent_improvement * n)

Blockers
========
### Given
value_of_unblocked_PBIs
cost_of_unblocking (= time_cost)
cost_of_unblocked

### Then 
total_improvement = value_of_unblocked_PBIs * (cost_of_unblocking / (cost_of_unblocking + cost_of_unblocked))

Optimization
=============
## Server Costs
CPU Time, RAM, HD

## User Cost
User 

Defect Risk
===========
## Semi-Known Single Defect
### Given
cost_of_defect = The average cost to business of the likely class of defect
chance_of_defect = The chance a defect will happen
percent_improvement = The percent reduction in chance of defect happening

### Then
risk_of_defect = cost_of_defect * chance_of_defect
total_improvement = cost_of_defect * percent_improvement

## Unknown Multiple Defects
### Given
cost_of_defect = The average cost to business of the likely class of defect
expected_number_of_defects = The expected number of defects
expected_percent_defect_reduction = The expected number of defects

### Then
risk_of_defects = cost_of_defect * expected_number_of_defects
total_improvement = risk_of_defects * expected_percent_defect_reduction
