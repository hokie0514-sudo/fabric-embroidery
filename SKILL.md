---
name: fabric-embroidery
description: Convert flat images into realistic fabric-and-embroidery artwork while preserving their content, colors, and layout. Use for textile-style image edits, not embroidery-machine stitch files.
---

# Fabric and Embroidery Conversion

Use an available image-editing tool with the user's image as the edit target. This skill supplies instructions, not an image model or API credentials. If no image-editing tool is available, explain that limitation; do not claim to have generated an image or substitute a generic texture filter.

## Workflow

1. Inspect the supplied image. Identify the background fabric, foreground embroidery, text, genuine cutouts, and layer overlaps. Ask for the edit target only when multiple inputs are ambiguous.
2. Read [the conversion prompt](conversion-prompt.md) and use it to guide the edit. Treat the original image as the authority for text, composition, colors, and proportions. Change materials only.
3. Use fine plain-weave fabric for the background and fine, low-relief stitches for foreground text and graphics. Preserve transparency, counters, and underlying layers. Do not add props, frames, watermarks, or decorative stitch patterns absent from the design.
4. Compare the result with the original: check wording, line breaks, colors, silhouettes, spacing, cutouts, and stitch direction. If needed, make at most two focused corrections while locking the remaining design.
5. Save a separate PNG without overwriting the source. Use the user's chosen output folder or the current workspace output folder. Preserve the aspect ratio and report any size change or remaining visible mismatch.
6. Deliver the image preview and saved file. Explain that it is a visual mockup, not a DST/PES embroidery-machine file.

Process multiple images separately unless the user asks for a combined composition. Use any additional reference only for its stated role, such as fabric texture or stitch scale.
