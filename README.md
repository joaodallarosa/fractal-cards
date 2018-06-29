# Fractal Cards

Fractal Cards is a card component experiment using [Fractal](https://github.com/frctl/fractal).


## Requirements
Fractal cards requires: 
- [Fractal](https://github.com/frctl/fractal) 
- [NodeJS](https://nodejs.org/en/) v4.4.7+
- [Gulp](https://gulpjs.com/)
- [SaSS](https://sass-lang.com/)


## Getting Started

Install project dependencies and Gulp:

    npm install
    npm install gulp

## Run it
Use the following command to build the assets and start up **Fractal** on **port 3000**:

    gulp build
    
# Components
List of components and its variants.

## Button
Context variables:

**label**: Button label. For example 'Click Me'.

**onClick**: Button click action. For example "console.log('You clicked me!')".

Variants:

 - **default**

 - **outline**

 - **disabled**

## Card

Variants:

### card
Blank card in its simplest form.

Context variables:

**content**: The card content. For example ("content": "<html>Hello World :)</html>").
##
**elevation**: Elevation of the card(CSS property 'shadow-box').
 
| elevation | shadow-box |
|--|--|
| 0 | none |
| 1 | 1px 1px 1px |
| 2 | 2px 2px 2px |
| 3 | 3px 3px 3px |
| 4 | 4px 4px 4px |

##
**corner-roundness**: Sets the 'roundness' of the card edges.
 
| Corner Roundness | border-radious |
|--|--|
| (default) | 8px |
| 0 | 0px |
| 1 | 5px |
| 2 | 10px |
| 3 | 15px |
| 4 | 20px |

#
### card--highlight
Highlights an information. For example, could be a city, an event, a person.

Context variables:

**mainTitle**

**secondaryTitle**

**info**

**imageUrl**: Used as the card background cover image.


#
### card--highlight-grid
Responsive grid for displaying multiple Highlight Cards.

Context variables: As the grid is just a grid displaying Highlight Cards, the Context receives an array of 'card--highlight'

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


**Important:** The parameter 'size', also affects how the card is displayed in the grid.

 - 'small': 25% of the grid width; 
 - 'medium': 50% of the grid width;
 - 'big': 100% of the grid width;
