# Swatches

## What is a Swatch
A swatch is defined as a design option for a product that can be customized. The swatch could be a solid color, or a pattern. 

## Sample Swatch Images 
For this prototype, we have provided sample swatch images you can use. They can be downloaded from this repo. 

![Aloha](https://raw.githubusercontent.com/RauxaRepo/Coding-Challenge-Services-Engineering/master/swatches/aloha-sm.jpg "Aloha") 
![Cubes](https://raw.githubusercontent.com/RauxaRepo/Coding-Challenge-Services-Engineering/master/swatches/cubes-sm.jpg "Cubes")
![Rainbows and Butterflies](https://raw.githubusercontent.com/RauxaRepo/Coding-Challenge-Services-Engineering/master/swatches/rainbow-butterflies-sm.jpg "Rainbows and Butterflies")
![Camo](https://raw.githubusercontent.com/RauxaRepo/Coding-Challenge-Services-Engineering/master/swatches/camo-sm.jpg "Camo") 

## Swatch Specifications

### Image Sizes
- **Large**: Images with the `-lg` suffix. They can be used for the swatch detail view.
- **Small**: Images with the `-sm`. They can be used for the swatch list view.

### Swatch Data Model 

```javascript
{
    "active": Boolean
    "name": String,
    "price": String,
    "image": String,
    "color": String
    "date": String
}
```
### Example
```javascript
{
    "active": true,
    "name": "My Swatch",
    "price": "$10",
    "image": "url to image",
    "color": "#467654",
    "date": "created timestamp"
}
```