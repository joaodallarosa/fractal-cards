# Fractal Cards

Fractal Cards is a card component experiment using [Fractal](https://github.com/frctl/fractal).


## Requirements
Fractal cards requires: 
- [Fractal](https://github.com/frctl/fractal) 
- [NodeJS](https://nodejs.org/en/) v4.4.7+
- [Gulp](https://gulpjs.com/)
- [SaSS](https://sass-lang.com/)


## Getting Started

First make sure to install all of the project dependencies with:

    npm install

## Run it
Use the following command to build the assets and start **Fractal** on **port 3000**:

    gulp build
# Components
List of components and its variants.

## Button
There are 
**label**: Button label. For example 'Click Me'.
**onClick**: Button click action. For example "console.log('You clicked me!')".


 - Default Button
 - Outline Button
 - Disabled Button

## Card

### card
The base card in its simplest form. When using a card you can set:

**Content**: The card content.
##
**Elevation**: Sets the elevation of the card.
 
| Elevation | Box Shadow in Pixel |
|--|--|
| 1 | 1px 1px 1px |
| 2 | 2px 2px 2px |
| 3 | 3px 3px 3px |
| 4 | 4px 4px 4px |

##
**Corner Roundness**: Sets the 'roundness' of the card.
 
| Corner Roundness | border-radious |
|--|--|
| 1 | 1px |
| 2 | 2px |
| 3 | 3px |
| 4 | 4px |

#
### card--highlight
Highlights an information. For example, could be a city, an event, a person.

**mainTitle**
**secondaryTitle**
**info**
**imageUrl**: Used as the card background cover image.


#
### card--highlight-grid
Responsive grid for displaying multiple Highlight Cards.

Example of context:

```
"context": {
                "cards": [{
                    "mainTitle": "Valtech_",
                    "secondaryTitle": "Front-End",
                    "info": "fnsldf jkldalkjd dsajkljdl aj j jdksaj s klj djalsj dlkaj ljasl jdlkasj ldsjlj ldsja ldjsal",
                    "imageUrl": "/imgs/Lagoa.jpg",
                    "size": "big",
                    "button": {
                        "label": "Explore More",
                        "modifier": "outline",
                        "onClick": "console.log('Explore Floripa :)')"
                    }
                }, {
                    "mainTitle": "Venice",
                    "secondaryTitle": "Italy",
                    "info": "fnsldf jkldalkjd dsajkljdl aj j jdksaj s klj djalsj dlkaj ljasl jdlkasj ldsjlj ldsja ldjsal",
                    "imageUrl": "/imgs/Venice.jpg",
                    "size": "medium",
                    "button": {
                        "label": "Explore More",
                        "modifier": "outline",
                        "onClick": "console.log('Explore Venice')"
                    }
                }]
}
```


**Important:** The parameter 'size' here, also affects how the card is displayed in the grid.

 - 'small': 25% of the grid width; 
 - 'medium': 50% of the grid width;
 - 'big': 100% of the grid width;
