# ContEx Change Log

## In progress (v0.2.0 dev - commits to master)
- Documentation for overall package, BarChart, Axis, Scale, CategoryColourScale, ContinuousLinearScale
- Renamed :data to :dataset in various plot types to avoid ambiguity
- ** BREAKING ** Renamed BarPlot to BarChart
- ** POTENTIALLY BREAKING ** Renamed ContinuousScale to ContinuousLinearScale, renamed constructor from new_linear() to new(). Used internally, so shouldn't cause any issues.
- Fixed incorrect closed path in sparkline
- Allowed forcing of value range in `BarChart` (`BarChart.force_value_range\2`)
- Changed `BarChart` colour handling to pass through to `ColourCategoryScale`
- Changed `new\3` to `new\1` on various plots as width & height are now set by `Plot`
- Prevented infinite loop in `ColourCategoryScale` when setting palette to `nil` (turns out `nil` is an atom)
- Fixed divide by zero error in `ContinuousLinearScale` (needed to test for float as well as integer)
- Enabled legend for point plot
- Added multiple series for point plot (note - must share a common x value at this stage)


## v0.1.0 : 2020-01-15
Initial version extracted from bigger project