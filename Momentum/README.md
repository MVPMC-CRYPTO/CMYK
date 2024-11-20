# Momentum

![Preview of strategy](https://github.com/CMYKSCRIPTS/Momentum/blob/MASTER/DOCS/MainPreview.png?raw=true)
## Core Properties
### Splitting Momentum lenghts up in iterates
> The reason to do this is reducing the amount of calculations the script goes through, to keep it within the limits of PineScript.

> The iterates will split up momentum lenghts from the largest available **5400** to the smallest usefull **approx 30**

> This can be done Linear, dividing the steps equally, Logarithmic or Exponential.

> Favor goes out to Exponential, as longer momentum lenghts equal each other more.

![Preview of strategy](https://github.com/CMYKSCRIPTS/Momentum/blob/MASTER/DOCS/Exponential%20iterates.png?raw=true)

> In the above image you see momentum indexed from -1 to 1 colored red to green, split exponentially in rows of each iterate lenght.

### Fluid transformations
Short motivation for fluid transformations vs arbitrary settings
#### Triggering entries
Add formula and image.
// Should be scaled to timeframe
#### Weighted entries
Add formula and image
// Focus Should be adjustable
#### Macro trending bias
> A factor (a) limited from -1 to 1 will be applied on the iterates with following formula:

![Trending Transformation](https://github.com/CMYKSCRIPTS/Momentum/blob/MASTER/DOCS/Trending%20transformation.png?raw=true)

> A note here is that a percental based (a) would have its limits from -1 to ∞
If this is what should be applied, the math of the formula needs to be changed accordingly.

> This transformation could be applied flat to all iterates.
But this could mean an unjust bias is applied to the smaller momentum lenghts.

> A simple proposition to improve this, is applying a decay curve to the bias factor.
A complex curve could later be calculated to deviate from this decay curve based on lenghty backtesting and optimization results with ML.

![Trending Transformation Temporal decay curve](https://github.com/CMYKSCRIPTS/Momentum/blob/MASTER/DOCS/Tranding%20transformation%20with%20temporal%20bias%20curve.png?raw=true)

> An example of the decay curve, simple and measured.

![Trending Transformation Temporal decay curve example](https://github.com/CMYKSCRIPTS/Momentum/blob/MASTER/DOCS/Trending%20transformation%20temporal%20bias%20curve%20example.png?raw=true)

#### Macro to micro focus
Add formula and image, Use-case examples

### Strong securities
#### Breakout adaptation
Use-case examples
#### Account balancing
Use-case examples

### Usefull analytical tools
#### Momentum scope
Add image
#### Position average
Add image
#### Open interest
Add image + Use-case
#### Drawdown
Add image + use-case
#### Profit and Loss
Add image + use case

### Tools for automation
#### ?