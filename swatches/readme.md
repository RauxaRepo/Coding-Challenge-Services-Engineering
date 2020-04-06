# Swatches

## What is a Swatch
A swatch is defined as a design option for a product that can be customized. The swatch could be a solid color, or a pattern. 

## Sample Swatch Images 
For this prototype, we have provided sample swatch images you can use. They can be downloaded from this repo. 

## Technical Specifications

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
    "date": "date created"
}
```