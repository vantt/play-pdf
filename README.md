# play-pdf
Learning about pdf generation and playing with various tools


# Learning about Pdf
## How to Calculate page size in inches or centimetres?

Tool to compute:  **https://docupub.com/pdfresize/**

The size of a PDF **is the number of pixels**, and is generally defined by the CropBox or MediaBox setting for each page. 
This provides a set of 4 number (x,y,width,height) to define how big the page is. 
A common value is [0 0 595 842] for an **A4** page .

**Standard dpi is 72 dots per inch.**
So we can convert the CropBox and MediaBox to inches by dividing these numbers by **72**. This gives us (8.26 x 11.69 inch).

**There are 2.54 centimetres per inch**. 
So multiplying by this we get 20.99 x 29.7cm  (20.99 = 8.26x2.54)  (29.7 = 11.69x2.54)

### Formula:
Pixel to Inches:  NumOfPixels / 72
Inches to Cm:     NumOfInches * 2.54
Cm to Pixels:     NumOfCm * 72

## Size Info
### Letter Portrait (wxh)
Pixels: 612   x 792 pixel
Inches: 8.5   x 11 inch
Centi:  21.59 x 27.94 cm
Mili:   215.9 x 279.4 mm

### A4 Portrait (wxh)
Pixels: 595   x 842 pixel
Inches: 8.26  x 11.69 inch
Centi:  20.99 x 29.7 cm
Mili:   209.9 x 297.04 mm

### A5 Portrait (wxh)
Pixels: 420   x 595 pixel
Inches: 5.83  x 8.26 inch
Centi:  14.82 x 20.99 cm
Mili:   148.2 x 209.9 mm