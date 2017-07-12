# Highcharts-More

The universal **highcharts-more** module. This module can be loaded as an ES6, AMD, CommonJS or global module, in NodeJS or in the browser. It works with most modern module loaders ([ES6](https://github.com/ModuleLoader/es6-module-loader), [RequireJS](https://github.com/requirejs/requirejs), [SystemJS](https://github.com/systemjs/systemjs)). This package is generated based on the **latest** [highcharts v5.0.12](https://github.com/highcharts/highcharts/releases/tag/v5.0.12) release.
> [highcharts-more](https://www.npmjs.com/package/highcharts-more-node) requires the [highcharts](https://www.npmjs.com/package/highcharts) module

### What is Highcharts?
[Highcharts JS](http://www.highcharts.com/) is a JavaScript charting library based on SVG, with fallbacks to VML and canvas for old browsers. To avoid bloating the Highcharts core library, the Highcharts team deploy new chart types and features in a separate file called [highcharts-more.js](https://github.com/highcharts/highcharts-dist/blob/master/highcharts-more.js). In short, highcharts-more is extra functionality on top of Highcharts without modifying it's core code. It also allows you to use some charts types which don't exist in the "original" highcharts such as bubble, range, gauge and pollar charts.

### Installation
```bash
$ npm install highcharts-more-node
```

### Example Usage
> Please note that there are several ways to use Highcharts. For general installation instructions, see [the docs](http://www.highcharts.com/docs/getting-started/installation).

First, install the [highcharts](https://www.npmjs.com/package/highcharts) and [highcharts-more](https://www.npmjs.com/package/highcharts-more-node) packages.
```bash
$ npm install highcharts-more-node
```

Now import highcharts-more into your projects which will also import the **highcharts** core module.
```js
// import Highcharts-More (no need to import `highcharts` since it's wrapped by `highcharts-more`)
import {Highcharts} from 'highcharts-more-node'
// OR
import Highcharts from 'highcharts-more-node'   


export class GaugeChartExample {

  constructor() {
  
    // create the chart
    Highcharts.chart({
      chart: {
        type: 'gauge' // available ONLY with highcharts-more
      },
      // ...................................
      // ... chart configuration options ...
      // ...................................
    });
  };
  
}
```


##### Helpful links

* Official website:  [www.highcharts.com](http://www.highcharts.com)
* Download page: [www.highcharts.com/download](http://www.highcharts.com/download)
* Licensing: [www.highcharts.com/license](http://www.highcharts.com/license)
* Support: [www.highcharts.com/support](http://www.highcharts.com/support)
* Issues: [Working repo](https://github.com/highcharts/highcharts/issues)
