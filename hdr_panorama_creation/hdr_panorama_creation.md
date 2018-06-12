Introduction

In this guide we will go over a workflow for creating spherical HDR maps, suitable for use in an image based lighting based pipeline.

At a high level, there will be three steps:

1. Panoramic photography, using Magic Lantern and a fish eye lens
2. Aligning the photos using Autopano Pro
3. Merging the LDR panoramas into a final HDR (and removing the tripod) using Photoshop

Step 1. Panoramic photography

Take the photos, using 5 brackets, 3 elevation, 6 angles for a total of 90 photos.

# Step 2. Aligning photos

![Alt text](images/autopano/open_files.png "Optional title")

![Alt text](images/autopano/create_stacks_by_n.png "Optional title")

![Alt text](images/autopano/create_stacks_by_n_options.png "Optional title")

![Alt text](images/autopano/image_properties_images.png "Optional title")

![Alt text](images/autopano/image_properties_crop.png "Optional title")

![Alt text](images/autopano/images_grouped.png "Optional title")

![Alt text](images/autopano/settings_detection.png "Optional title")

![Alt text](images/autopano/settings_panorama.png "Optional title")

![Alt text](images/autopano/settings_render.png "Optional title")

![Alt text](images/autopano/settings_detected.png "Optional title")

![Alt text](images/autopano/final_render.png "Optional title")

![Alt text](images/autopano/should_have_ldr_files.png "Optional title")

# Step 3. Creating final HDR

![Alt text](images/photoshop/merge_to_hdr_menu.png "Optional title")

Now that we have our 5 exposure panoramas, we want to merge those together to create the single HDR panorama. To do this we will use the Merge to HDR option in Photoshop.

![Alt text](images/photoshop/merge_to_hdr_pro_options.png "Optional title")

Select the 5 bracketed exposure panoramas.

![Alt text](images/photoshop/merge_to_hdr_pro.png "Optional title")

Here we can see the 5 exposures which are being combined into the single HDR panorama.

![Alt text](images/photoshop/select_tripod.png "Optional title")

Our final step will be to remove the tripod from the panorama. Use the magic wand to select the tripod.

![Alt text](images/photoshop/expand_selection.png "Optional title")

Expand the selection to get a bit of the surrounding, non tripod image data.

![Alt text](images/photoshop/expand_selection_options.png "Optional title")

![Alt text](images/photoshop/expanded_selection.png "Optional title")

![Alt text](images/photoshop/fill_menu.png "Optional title")

We will then use the Content Aware fill to eliminate the tripod.

![Alt text](images/photoshop/content_fill_options.png "Optional title")

![Alt text](images/photoshop/content_filled.png "Optional title")

![Alt text](images/photoshop/export_exr.png "Optional title")

Finally, export the HDR panorama as an EXR.
