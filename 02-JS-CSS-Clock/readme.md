Day O2 CSS Clock

HTML vs. Boday in CSS

The difference between <html> and <body> is easy to overlook.
Not a good idea

1. Root Element
   <html> is the root element of a document
   <body> and <head> fall directly inside<html>
   :root has a higher level than <html> 
      (in CSS)
      :root {

      }
      html {

      }

2. Put global styles on <html>
   if any styles are inherited across the board
   eg. background, background-size/color, margin-bottom/top/left/right, font 

3. when working with rem units
   .module{}
   width: 40rem;
   }
   the rem unit is relative to the font-size of <html> element

4. JS difference 
   query: html: document.rootElement
          body: document.body

5. throw bkg-color on html and use CSS as a wrapper 
   so no need to define an extra div-container with a class of "wrapper" (saw someone write <div class="wrapper"> after body tag)
