# About of Mues Framework

This framework development for Mues Sites since 2016. 

## CSS Contains

- Grid System
  - In Percent
  - In Piece
- Advenced Padding Structure
- Useful Class Structure and Variables
- Multi-Use Grid System (1 ~ 100 Percent or 1-12 Piece)
- Ability to develop for all devices at the same time
  - Mobile
  - Vertical Tablet
  - Horizontal Tablet

## Javascript Contains

- jQuery
- [NiceScroll](https://github.com/inuyaksa/jquery.nicescroll)
- [Owl Carousel](https://github.com/OwlFonk/OwlCarousel)
- Special Lightbox - Image/Video Support
- Mobile View Proportional Support
- Special Icon Font Creator

## CSS Variables

### Grid System (In Percent)

- Minimum value: `1` 
- Maximum value: `100`

Class Name | Meaning | Using
------------ | ------------- | ------------- 
MS-PT       | Mues Percent  |  MS-20
MS-MW-PT       | Mues Mobile Width Percent  |  MS-MW-20
MS-TW-PT       | Mues Tablet Width Percent  |  MS-TW-20
MS-HTW-PT       | Mues Horizontal Tablet Width Percent  |  MS-HTW-20


Class Name | What's Happend
------------ | ------------- 
MS-20       | `width: 20%` (All Devices)
MS-MW-20       | `width: 20%` (Just Mobile Devices) 
MS-TW-20       | `width: 20%` (Just Vertical Tablet Devices) 
MS-HTW-20       | `width: 20%` (Just Horizontal Tablet Devices) 

#### Multiple Using

```html
<div class='Mues MS-20 MS-MW-100 MS-TW-30 MS-HTW-50'></div>
```

```css
.Mues {
    display: block;
    float: left;
    box-sizing: border-box;
}

.MS-20 { 
    width: 20%; 
} 

/*********************************************************/
/*                    Grid System (Mobile)               */
/*********************************************************/
@media only screen and (min-width: 320px) and (max-width: 415px) {
  .MS-MW-100 { 
      width: 100% !important; 
  } 
}

/*********************************************************/
/*                    Grid System (Tablet)               */
/*********************************************************/
@media only screen and (min-width: 416px) and (max-width: 800px) {
  .MS-TW-30 { 
      width: 30% !important; 
  } 
}

/*********************************************************/
/*                    Grid System (Tablet (H) )          */
/*********************************************************/
@media only screen and (min-width: 801px) and (max-width: 1200px) {
  .MS-TW-50 { 
      width: 50% !important; 
  } 
}

```
> no more code, manage every device just single line

___

### Grid System (In Piece)

- Minimum value: `2` 
- Maximum value: `10`

Class Name | Meaning | Using
------------ | ------------- | ------------- 
MS-GW-PC       | Mues Grid Width Piece  |  MS-GW-3


Class Name | What's Happend
------------ | ------------- 
MS-GW-3       | `width: 33.3333%`

#### Multiple Using

```html
<div class='Mues MS-GW-3 MS-MW-100 MS-TW-30 MS-HTW-50'></div>
```

```css
.Mues {
    display: block;
    float: left;
    box-sizing: border-box;
}

.MS-GW-3 { 
    width: 33.3333%; 
} 

/*********************************************************/
/*                    Grid System (Mobile)               */
/*********************************************************/
@media only screen and (min-width: 320px) and (max-width: 415px) {
  .MS-MW-100 { 
      width: 100% !important; 
  } 
}

/*********************************************************/
/*                    Grid System (Tablet)               */
/*********************************************************/
@media only screen and (min-width: 416px) and (max-width: 800px) {
  .MS-TW-30 { 
      width: 30% !important; 
  } 
}

/*********************************************************/
/*                    Grid System (Tablet (H) )          */
/*********************************************************/
@media only screen and (min-width: 801px) and (max-width: 1200px) {
  .MS-TW-50 { 
      width: 50% !important; 
  } 
}

```

___

### Advenced Padding Structure 

Class Name | Meaning | Using
------------ | ------------- | ------------- 
MS-PD-LR-PX       | Mues Padding Left & Right Pixel  |  MS-PD-LR-20
MS-PD-TB-PX       | Mues Padding Top & Bottom Pixel  |  MS-PD-TB-20
MS-PD-AC-PX       | Mues Padding All Corners Pixel  |  MS-PD-AC-20

### Advenced Padding Structure (What's Happend)

Class Name | What's Happend
------------ | ------------- 
MS-PD-LR-20       | `padding-left: 20px; padding-right: 20px`
MS-PD-TB-20       | `padding-top: 20px; padding-bottom: 20px`
MS-PD-AC-20       | `padding: 20px;`

___

### Container Sizes

Device Width Max/Min | Container Size
------------ | ------------- 
1200px/~       | `width: 1200px`
1200px/1100px       | `width: 1099px`
1100px/1000px       | `width: 999px`
1000px/900px       | `width: 899px`
900px/800px       | `width: 799px`
~/800px       | `width: 100%`

___

### Useful Classes

Class Name | Meaning
------------ | ------------- 
.NPL       | Remove padding-left
.NPR       | Remove padding-right
.NPT       | Remove padding-top
.NPB       | Remove padding-bottom
.FL       | Lean to the left
.FR       | Lean to the right
.Clear       | Clear line
.Inline       | Change display status
.Container       | Call general container
.FullImage       | For img element in this element width: 100%, height: auto
.Relative       | Change position status relative
.NM       | Remove margin
.NP       | Remove padding
.TR       | Change text align status right
.TL       | Change text align status left
.TC       | Change text align status center


Class Name | What's Happend
------------ | ------------- 
.NPL       | `padding-left: 0 !important;`
.NPR       | `padding-right: 0 !important;`
.NPT       | `padding-top: 0 !important;`
.NPB       | `padding-bottom: 0 !important;`
.FL       | `float: left !important;`
.FR       | `float: right !important;`
.Clear       | `clear: both; display: block !important;`
.Inline       | `float: none !important; display: inline-block !important;`
.Container       | `Different resolutions for all devices.`
.FullImage       | `width: 100%; height: auto; display: block;` (For img element in this element)
.Relative       | `position: relative;`
.NM       | `margin: 0 !important;`
.NP       | `padding: 0 !important;`
.TR       | `text-align: right !important;`
.TL       | `text-align: left !important;`
.TC       | `text-align: center !important;`


