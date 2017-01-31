# chartjs-heatmap

## Installation

Add the Chart.js 2 library :

https://github.com/chartjs/Chart.js

Import the library after Chart.js :

`<script src="path/to/lib/heatmap.js"></script>`

## Example of usage
    
    var heatmap = new Chart(element, {
        type: 'heatmap',
        data: {
            xLabels: ['2014', '2015', '2016', '2017'],
            yLabels: ['Strength', 'Intelligence', 'Stamina', 'Spirit'],
            datasets: [{
                data: [{
                    y: 0, // index of 'Strength'
                    x: 0, // index of '2014'
                    a: 0.5, // alpha of the color [0, 1]
                    v: 500, // value
                }, {
                    y: 2, // index of 'Stamina'
                    x: 0, // index of '2014'
                    a: 0.2, // alpha of the color [0, 1]
                    v: 250, // value
                }, {
                     y: 1, // index of 'Intelligence'
                     x: 3, // index of '2017'
                     a: 1, // alpha of the color [0, 1]
                     v: 1000, // value
                }]
            }]
        },
        options: {
            yColors: [ // colors for each lines
                {r: 0,   g: 150, b: 136},
                {r: 255, g: 235, b: 59},
                {r: 255, g: 152, b: 0},
                {r: 244, g: 67,  b: 54}
            ],
        }
    });
