---
layout: default
---
# ARC Fog Modeling Project
### Goes-18, CMPIP6, MODIS (SST, LST)
---
## Project Poster

<canvas id="pdf-canvas"></canvas>
<script src="https://cdnjs.cloudflare.com/ajax/libs/pdf.js/3.11.174/pdf.min.js"></script>
<script>
  pdfjsLib.getDocument('Arc_poster.pdf').promise.then(pdf => {
    pdf.getPage(1).then(page => {
      const canvas = document.getElementById('pdf-canvas');
      const context = canvas.getContext('2d');
      const viewport = page.getViewport({scale: 0.4});
      canvas.width = viewport.width;
      canvas.height = viewport.height;
      page.render({canvasContext: context, viewport: viewport});
    });
  });
</script>

