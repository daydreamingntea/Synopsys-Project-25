---
layout: default
---
<style>
  /* Layout: sidebar + content side by side */
  .page-content {
    display: flex;
    align-items: flex-start;
    gap: 2rem;
  }
  .toc-sidebar {
    position: sticky;
    top: 20px;
    align-self: flex-start;
    width: 200px;
    flex-shrink: 0;
    background: #f6f8fa;
    border: 1px solid #e1e4e8;
    border-radius: 6px;
    padding: 1rem;
    font-size: 0.9rem;
    max-height: calc(100vh - 40px);
    overflow-y: auto;
  }
  .toc-sidebar h4 {
    margin-top: 0;
    margin-bottom: 0.75rem;
    font-size: 1rem;
    color: #159957;
    border-bottom: 1px solid #e1e4e8;
    padding-bottom: 0.5rem;
  }
  .toc-sidebar ul {
    list-style: none;
    margin: 0;
    padding: 0;
  }
  .toc-sidebar li {
    margin-bottom: 0.4rem;
  }
  .toc-sidebar a {
    text-decoration: none;
    color: #333;
    display: block;
    padding: 0.25rem 0.5rem;
    border-radius: 4px;
    transition: background 0.15s ease, color 0.15s ease;
  }
  .toc-sidebar a:hover {
    background: #eaf7ef;
    color: #159957;
  }
  .toc-sidebar a.active {
    background: #159957;
    color: #fff;
  }
  .main-body {
    flex: 1;
    min-width: 0;
  }
  /* Stack on small screens */
  @media (max-width: 800px) {
    .page-content {
      flex-direction: column;
    }
    .toc-sidebar {
      position: static;
      width: 100%;
      max-height: none;
    }
  }
</style>
<div class="page-content">
<nav class="toc-sidebar" id="toc">
  <h4>Contents</h4>
  <ul>
    <li><a href="#recap-video">Recap Video</a></li>
    <li><a href="#personal-journey">Personal-Journey</a></li>
    <li><a href="#abstract">Abstract</a></li>
    <li><a href="#project-description">Project Description</a></li>
    <li><a href="#code">Code</a></li>
    <li><a href="#images">Images</a></li>
  </ul>
</nav>
<div class="main-body" markdown="1">

*Note: Majority of information documenting the process and procedures of this project have been lost. The following information described below will focus on what has been recovered along with personal thoughts/experiences. This was my first time with an engineering project and evidently, is not of high quality nor was it presented at its best.*

# Recap Video

Our display was made by creating a slideshow and printing each slide on a sheet on paper before it was taped onto a tri-fold poster board. The slides were edited into a video format but the content is identical.

<video src="https://github.com/user-attachments/assets/510e611c-4c4d-4188-b843-07eb98fdb569" controls="controls" style="max-width: 100%;"></video>

# Personal Journey

## Origination of Project

The motivation behind this project was to compete in the Synopsys Championship. This project was not my nor my partner's idea, rather it was given to us from a parent. Consequently, a lot of parental guidance was needed. I myself found this project to be unexciting and boring as it was already in an area I had no interest in and was heavy on coding, a skill that I do not possess. 

## Challenges

This was the first project I had done for the Synopsys Championship. Consequently, I was unfamiliar with the application process, expectations, and the presentation of scientific works in general. There was a lack of focus on data collection in this project along with a lack of internal motivation as I did not find it to be something that I would want to invest my time and effort in (but I did anyways).

## Takeaways

While the topic of the project was not my own nor of my interest, having that exposure to the application process and presenting my work is definitely something that I have put to use at some point in time. In fact, after competing in 2025, I was urged to compete again in 2026  where I had less parental guidance and more freedom over my project, pushing me to learn and solve my own problems instead of asking for help from an adult. Even though majority of the information regarding this project was lost, its main impact was its place as a origination of my journey in STEM exploration.

# Abstract

The human eye can only see the visible light spectrum, but there is always invisible waves around us that we cannot perceive. With our "super eye", we will be able to see those invisible waves around us. What we are trying to create is a way to have visible and invisible light included in the same image; thus expanding the range of light a human can experience.

The first approach we took was to map UV and IR light to parts of the visible spectrum before combining a visible and invisible light image; a second approach was to exclude certain parts of an image before combining it with another image (masking). In the case of the flower *Oxalis fontana*, we used the first approach. After combining the two images, we were able to see the pollen concentrated at the center of the flower. For the second approach, we managed to only include the portion of the stovetop (turned on) that can be shown in IR light and combine it with a visible light image. The result was a normal looking kitchen with a stovetop showing a purple glow. 

Due to lack of time and equipment there were certain goals which we were unable to achieve: taking photos ourself with UV light, and experimenting with more ways of combining images. One possibility is to use UV and IR light lamps to capture images to increase the amount of invisible light in the image, allowing certain details to stand out.

# Project Description

*Note: if I'm being honest, this section is basically an improved and longer version of the abstract that is being written from memory.*

## Objective

Devise a method to combine an image taken with visible light with an image taken at invisible light. This will allow a human to "experience" what the image would look like while preserving the details found in the original images. UV light is known to reveal tiny details on flowers and observe faraway galaxies while IR light can reveal thermal signatures and heat leaks in the environment. Being able to "expand" the human vision into these wavelengths while simultaneously "experiencing" an image at the visible light level can inform us about how our perception of the world could alter with our vision. 

## Approach

The parent who had created this project's topic had devised two different methods to combine the images. 

### Mapping

This first approach would use a portion of the visible light spectrum would be used to represent the invisible light. For example, if an image was taken with UV light, we could reserve the purple portion of the visible light spectrum for the UV image. The colors on the UV image would be remapped using the section of the visible light spectrum that has been reserved (which was determined using different functions). The same will be done to the image taken with visible light, the colors will be remapped with our new "compressed" light spectrum before the two images are layered over each other. Once the images are layered, the details of both images may be seen simultaneously. As for the downsides, the coloring of the new combined image will be off, overall quality may decrease (pixelation of image), and the images need to be lined up properly in order for them to combine cleanly. 

##### Visualization of Hue Mapping

Visible light hue mapping (linear, squared, square root, and segmented):

<img width="740" height="175" src="https://github.com/user-attachments/assets/6555670e-e094-4828-9a5c-50ed91fb3fb0" />

UV light hue mapping:

<img width="243" height="173" src="https://github.com/user-attachments/assets/bf4cd4fc-f6f3-4605-8564-a105a61c054f" />


### Masking

Two images are taken, one at visible light and one at an invisible light. An attribute unique to the image with invisible light can be selected and moved onto the visible light image. In our project, we had two images of a stove top that has been turned on. The image taken with IR light had a glowing purple stovetop while the image taken with visible light did not. The images were uploaded to a code where we manually inputted a range of RGB values. Colors matching those values would be taken from the IR image and masked onto the visible light image. The downside of this method is that it requires manual input of the RGB values (as well as trial and error) in order for the correct colors to be masked on properly. It may also result in certain unwanted details to be masked as well. In comparison to the merging method, masking does a better job of preserving the combined image's quality, color, and does not require the two initial images to line up properly for combination to occur. 

## Future Progress

Initially, we had hoped to have more time to take our own photos using a full spectrum camera and combine those images we had taken ourselves. We could have also found images taken in all different environments (e.g. space, the ocean, microscopic world, etc) and combined those images to see the effects of invisible light at different magnifications. As for this project's future, I do not plan on continuing it any time soon or making any further alterations. 


# Code

Any software that can run Python should be able to run this code. All the file names/paths have been altered to roughly describe the image. When it came to switching between the masking and mapping methods or changing certain files, the unused lines of code were simply commented out. There have been many iterations of code for this project and I am unsure if this are the finalized version.

This version of the code will also include the test images that were used. I tried my best to add in comments to help distinguish these images and any sections that were used as tests.

```python

# Imports
import matplotlib.pyplot as plt
import cv2
import numpy as np

# Read image
# VS or VL stands for visible light

PhotoSelection = 5

match PhotoSelection:
    case 1:
        imagePath = "/Users/Name/Downloads/"
        # Toys
        # This case is a test
        vl_img = cv2.imread(imagePath + "toy.JPG")
        uv_img = cv2.imread(imagePath + "toy_blue.JPG")
    case 2:
        imagePath = "/Users/Name/Downloads/"
        # Flowers at gate
        # This case was used in the mapping method
        vl_img = cv2.imread(imagePath+"gateflower_red.JPG")
        # vl_img = cv2.imread(gateflower_yellow.JPG")
        uv_img = cv2.imread(imagePath+"gateflower_blue.JPG")
    case 3:
        imagePath = "/Users/Name/Downloads/"
        # 1. Geranium sylvaticum - A large-flowered species with a strong UV signature in the fashion of a typical bull's-eye pattern. The UV-absorbing central area coincides with the visible-light nectar guide marks. It is instructive to compare the UV marks of this species with its close relative, G. pratense, and note the obvious differences between these species.
        # This case was used in the mapping method
        vl_img = cv2.imread(imagePath+"GERA_SYL_VL_I030609652.jpg")
        uv_img = cv2.imread(imagePath+"GERA_SYL_UV_I030609653.jpg")
    case 4:
        imagePath = "/Users/Name/Downloads/"
        # 2. Taraxacum vulgare  - This species has virtually no visual indication of a bull's-eye pattern. UV reflectance of the outer petals is high, but variable, and so is the area extent of the dark central zone in the bull's eye pattern. The common dandelion comprises a myriad of apomictic microspecies and this probably gives the observed variability in UV patterns. Still, dandelions are among the easiest subjects for perfecting your UV photographic skills.
        # This case was used in the mapping method
        vl_img = cv2.imread(imagePath+"tarax_vis.jpg")
        uv_img = cv2.imread(imagePath+"tarax_UV.jpg")
    case 5:
        imagePath = "/Users/Name/Downloads/"
        # 3. Oxalis fontana Bunge - Only occurring as a rare weed in Norway, Upright Yellow Sorrel displays a very prominent and nice UV pattern on its light yellow petals.
        # This case was used in the mapping method
        vl_img = cv2.imread(imagePath+"oxalisfontana.jpg")
        uv_img = cv2.imread(imagePath+"oxalisfontanauv.jpg")
    case 6:
        imagePath = "/Users/Name/Downloads/"
        # Color vs wavelength
        # This case is a test
        vl_img = cv2.imread(imagePath + "visible-spectrum-nm.png")
        uv_img = cv2.imread(imagePath + "visible-spectrum-nm.png")
    case 7:
        imagePath = "/Users/Name/Downloads/"
        # Color vs Hue
        # This case is a test
        vl_img = cv2.imread(imagePath + "cona-hue-ranges-map.png")
        uv_img = cv2.imread(imagePath + "cona-hue-ranges-map.png")
    case 8:
        imagePath = "/Users/Name/Downloads/"
        # Color vs Hue
        # This case is a test
        vl_img = cv2.imread(imagePath + "studioghibli.jpg")
        uv_img = cv2.imread(imagePath + "studioghibli.jpg")
    case 9:
        imagePath = "/Users/Name/Downloads/"
        # Color vs Hue
        # This case is a test
        vl_img = cv2.imread(imagePath + "totoroflowers.png")
        uv_img = cv2.imread(imagePath + "totoroflowers.png")
    case 10:
        imagePath = "/Users/Name/Downloads/"
        # Color vs Hue
        # This case is a test
        vl_img = cv2.imread(imagePath + "1338664.png")
        uv_img = cv2.imread(imagePath + "1338664.png")
    case 11:
        imagePath = "/Users/Name/Downloads/"
        # Color vs Hue
        # This case was used in the masking method
        vl_img = cv2.imread(imagePath + "Stove_2_VS_IMG_0162.JPG")
        uv_img = cv2.imread(imagePath + "Stove_2_720nm_IMG_0163.JPG")

    case _:
        print("****** Input has no match ******")
        exit(-1)


# Scale your BIG image into a small one:
scalePercent = 0.4
# Calculate the new dimensions
width = int(vl_img.shape[1] * scalePercent)
height = int(vl_img.shape[0] * scalePercent)
newSize = (width, height)


# Resize the image:
vl_img = cv2.resize(vl_img, newSize, None, None, None, cv2.INTER_AREA)
vl_img_rgb = cv2.cvtColor(vl_img, cv2.COLOR_BGR2RGB)
uv_img = cv2.resize(uv_img, newSize, None, None, None, cv2.INTER_AREA)
uv_img_rgb = cv2.cvtColor(uv_img, cv2.COLOR_BGR2RGB)

# HSV domain
vl_hsv = cv2.cvtColor(vl_img, cv2.COLOR_BGR2HSV)
vl_h, vl_s, vl_v = cv2.split(vl_hsv)
h_org = vl_h.reshape(-1)  # Save h values
uv_hsv = cv2.cvtColor(uv_img, cv2.COLOR_BGR2HSV)
uv_h, uv_s, uv_v = cv2.split(uv_hsv)

# Update the gray scale IR photo by assigning color
if PhotoSelection == 31:
    #uv_h = np.full_like(uv_h, 120)    # This IR photo Hue is zero since there is no color. Give it red color
    #uv_hsv[:,:,0] = 120  # Set Hue directly
    uv_s = np.full_like(uv_s, 200)
    uv_hsv[:,:,1] = 200
    print('Update color to grayscale image')

# Mapping color
MappingSelection = 1 # Choose mapping scheme
Weight_rgb = 0.5     # Weigt of visible light picture when add in RGB domain

match MappingSelection:
    case 1:
        # Linear
        Weight_hue = 0.75    # Hue range of visible light picture (0, 0.75) * 180
        Scale_uv_sv = 1      # Multiple UV V&S value during remapping to increase its impact when adding with VL pic
        vl_h_remap = (vl_h*Weight_hue).astype('uint8')    # Change Hue range
        uv_h_remap = (uv_h*(1-Weight_hue) + 180*Weight_hue).astype('uint8')
        uv_s_remap = (np.clip(uv_s.astype('uint16')*Scale_uv_sv, 0, 255)).astype('uint8')
        uv_v_remap = (np.clip(uv_v.astype('uint16')*Scale_uv_sv, 0, 255)).astype('uint8')
    case 2:
        # Square
        Weight_hue = 0.75    # Hue range of visible light picture (0, 0.75) * 180
        Scale_uv_sv = 1      # Mulitple UV V&S value during remapping to increase its impact when adding with VL pic
        vl_h_remap = (Weight_hue*np.square(vl_h/180)*180).astype('uint8')    # Change Hue range
        uv_h_remap = (uv_h*(1-Weight_hue) + 180*Weight_hue).astype('uint8')
        uv_s_remap = (np.clip(uv_s.astype('uint16')*Scale_uv_sv, 0, 255)).astype('uint8')
        uv_v_remap = (np.clip(uv_v.astype('uint16')*Scale_uv_sv, 0, 255)).astype('uint8')
    case 3:
        # Square root
        Weight_hue = 0.75    # Hue range of visible light picture (0, 0.75) * 180
        Scale_uv_sv = 1      # Mulitple UV V&S value during remapping to increase its impact when adding with VL pic
        vl_h_remap = (Weight_hue*np.sqrt(vl_h/180)*180).astype('uint8')    # Change Hue range
        uv_h_remap = (uv_h*(1-Weight_hue) + 180*Weight_hue).astype('uint8')
        uv_s_remap = (np.clip(uv_s.astype('uint16')*Scale_uv_sv, 0, 255)).astype('uint8')
        uv_v_remap = (np.clip(uv_v.astype('uint16')*Scale_uv_sv, 0, 255)).astype('uint8')
    case 4:
        # Piecewise linear
        Weight_hue = 0.75    # New Hue point of original hue of 1 (1 represent 180 deg, which is max Hue)
        Weight_org_hue_1 = 0.5 # Original Hue point of mid segment
        Weight_hue_1 = 0.2     # New Hue point of mid segment
        Scale_uv_sv = 1      # Multiple UV V&S value during remapping to increase its impact when adding with VL pic
        index_vl_h_seg1 = np.where(vl_h<=180*Weight_org_hue_1)  # Take Hue index belonging to 1st segment
        index_vl_h_seg2 = np.where(vl_h>180*Weight_org_hue_1)   # Take Hue index belonging to 2nd segment
        vl_h_remap = vl_h
        vl_h_remap[index_vl_h_seg1] = (Weight_hue_1*vl_h[index_vl_h_seg1]).astype('uint8')    # Change Hue of 1st segment
        Slope_seg2 = (Weight_hue - Weight_hue_1)/(1-Weight_org_hue_1)
        vl_h_remap[index_vl_h_seg2] = (Slope_seg2*vl_h[index_vl_h_seg2] + Weight_hue_1*180).astype('uint8') # Change Hue of 2nd segment
        uv_h_remap = (uv_h*(1-Weight_hue) + 180*Weight_hue).astype('uint8')
        uv_s_remap = (np.clip(uv_s.astype('uint16')*Scale_uv_sv, 0, 255)).astype('uint8')
        uv_v_remap = (np.clip(uv_v.astype('uint16')*Scale_uv_sv, 0, 255)).astype('uint8')
    case _:
        print("****** Mapping Selection wrong ******")
        exit(-2)

# Convert HSV to RGB
vl_hsv_remap = cv2.merge([vl_h_remap, vl_s, vl_v])
vl_img_remap_rgb = cv2.cvtColor(vl_hsv_remap, cv2.COLOR_HSV2RGB)
# Convert HSV to RGB
uv_hsv_remap = cv2.merge([uv_h_remap, uv_s_remap, uv_v_remap])
uv_img_remap_rgb = cv2.cvtColor(uv_hsv_remap, cv2.COLOR_HSV2RGB)
# Add 2 photo in RGB
comb_img_rgb = (vl_img_rgb.astype('uint16')*Weight_rgb + uv_img_rgb.astype('uint16')*(1-Weight_rgb)).astype('uint8')  # Change to uint16 to avoid overflow
comb_img_remap_rgb = (vl_img_remap_rgb.astype('uint16')*Weight_rgb + uv_img_remap_rgb.astype('uint16')*(1-Weight_rgb)).astype('uint8')  # Change to uint16 to avoid overflow


# ====================================
#         show combine  img
# ====================================
fig = plt.figure(figsize=(12,10))
ax1 = fig.add_subplot(3,2,1)
ax2 = fig.add_subplot(3,2,2)
ax3 = fig.add_subplot(3,2,3)
ax4 = fig.add_subplot(3,2,4)
ax5 = fig.add_subplot(3,2,5)
ax6 = fig.add_subplot(3,2,6)
ax1.imshow(vl_img_rgb)
ax1.set_title('Original ')
ax2.imshow(vl_img_remap_rgb)
ax2.set_title('Original Remap')
ax3.imshow(uv_img_rgb)
ax3.set_title('UV ')
ax4.imshow(uv_img_remap_rgb)
ax4.set_title('UV Remap')
ax5.imshow(comb_img_rgb)
ax5.set_title('Direct RGB add - no color remap - VL+UV')
ax6.imshow(comb_img_remap_rgb)
ax6.set_title('Combined - color remap - VL+UV')



# ****************************
#         Photo Mask
# ****************************

MaskSelection = 1

match MaskSelection:
    case 1:
        # Mask in RGB domain
        imgmask_in = vl_img  # Input to this process
        imgmask_in_rgb = cv2.cvtColor(imgmask_in, cv2.COLOR_BGR2RGB)  # Convert to RGB for plot
        # Here, you define your target color as a tuple of three values: RGB. [130, 158, 0] is green color
        MaskColor = [130, 158, 0]
        # You define an interval that covers the values in the tuple and are below and above them by 20
        MaskRange = 50
        # BGR (NOT RGB) color range - cannot be less than 0. That's why the color values have been adjusted here:
        # Be aware that opencv loads image in BGR format,
        MaskBoundaries = [([MaskColor[2], MaskColor[1]-MaskRange, MaskColor[0]-MaskRange],
                   [MaskColor[2]+MaskRange, MaskColor[1]+MaskRange, MaskColor[0]+MaskRange])]

        # for each range in mask boundary list,
        for (lower, upper) in MaskBoundaries:
            print('Boundaries = ', MaskBoundaries)
        #    print('image shape', vl_img.shape[0], vl_img.shape[1])

            # You get the lower and upper part of the interval:
            lower = np.array(lower, dtype=np.uint8)
            upper = np.array(upper, dtype=np.uint8)

            # cv2.inRange is used to binarize (i.e., render in white/black) an image
            # All the pixels that fall inside your interval [lower, upper] will be white
            # All the pixels that do not fall inside this interval will
            # be rendered in black, for all three channels:
            MaskColor = cv2.inRange(imgmask_in, lower, upper)
            MaskColor_rgb = cv2.cvtColor(MaskColor, cv2.COLOR_BGR2RGB)

            # Now, you AND the mask and the input image
            # All the pixels that are white in the mask will
            # survive the AND operation, all the black pixels will remain black
            imgmask_out = cv2.bitwise_and(imgmask_in, imgmask_in, mask=MaskColor)
            imgmask_out_rgb = cv2.cvtColor(imgmask_out, cv2.COLOR_BGR2RGB)

            # You can use the mask to count the number of white pixels.
            # Remember that the white pixels in the mask are those that
            # fall in your defined range, that is, every white pixel corresponds
            # to a green pixel. Divide by the image size and you got the
            # percentage of green pixels in the original image:
            ratio_mask = cv2.countNonZero(MaskColor)/(imgmask_in.size/3)
            # This is the color percent calculation.
            colorPercent = ratio_mask * 100

            # Print the color percent, use 2 figures past the decimal point
            print('mask pixel percentage:', np.round(colorPercent, 2))
    case 2:
        # Mask in Hue domain
        imgmask_in = uv_hsv  # Input to this process
        imgmask_in_rgb = cv2.cvtColor(imgmask_in, cv2.COLOR_HSV2RGB)  # Convert to RGB for plot
        MaskHue = 30    # Hue target, 30 - green, 150 - magenta
        MaskRange = 30   # Hue range
        # HSV boundries. Only care Hue. S and V take full value of [0, 255]
        MaskBoundaries = [([MaskHue-MaskRange, 0, 50],
                   [MaskHue+MaskRange, 255, 255])]

        # for each range in mask boundary list,
        for (lower, upper) in MaskBoundaries:
            print('Boundaries = ', MaskBoundaries)
            # You get the lower and upper part of the interval:
            lower = np.array(lower, dtype=np.uint8)
            upper = np.array(upper, dtype=np.uint8)

            # cv2.inRange is used to binarize (i.e., render in white/black) an image. All the pixels that fall inside your interval [lower, upper] will be white
            # All the pixels that do not fall inside this interval will be rendered in black, for all three channels:
            MaskColor = cv2.inRange(imgmask_in, lower, upper)
            MaskColor_rgb = cv2.cvtColor(MaskColor, cv2.COLOR_BGR2RGB)

            # AND the mask and the input image. All the pixels that are white in the mask will survive the AND operation, all the black pixels will remain black
            #imgmask_out = cv2.bitwise_and(imgmask_in, imgmask_in, mask=MaskColor)
            #imgmask_out_rgb = cv2.cvtColor(imgmask_out, cv2.COLOR_HSV2RGB)  # Convert to RGB for plot
            imgmask_out = cv2.bitwise_and(imgmask_in, imgmask_in, mask=MaskColor)
            imgmask_out_rgb = cv2.cvtColor(imgmask_out, cv2.COLOR_HSV2RGB)  # Convert to RGB for plot

            # Use the mask to count the number of white pixels. The white pixels in the mask are those that fall in the defined range
            ratio_mask = cv2.countNonZero(MaskColor)/(imgmask_in.size/3)
            colorPercent = ratio_mask * 100   # This is the color percent calculation.

            # Print the color percent, use 2 figures past the decimal point
            print('mask pixel percentage:', np.round(colorPercent, 2))

        print("case 2 - HSV mask")
    case 3:
        # Mask in HSV value domain
        imgmask_in = uv_hsv  # Input to this process
        imgmask_in_rgb = cv2.cvtColor(imgmask_in, cv2.COLOR_HSV2RGB)  # Convert to RGB for plot
        #MaskHue = 150  # Hue target, 30 - green, 150 - magenta
        MaskValue = 180  # Hue target, 30 - green, 150 - magenta
        #MaskRange = 10  # Hue range
        # HSV boundries. Only care Hue. S and V take full value of [0, 255]
        MaskBoundaries = [([0, 0, MaskValue],
                           [180, 255, 255])]

        # for each range in mask boundary list,
        for (lower, upper) in MaskBoundaries:
            print('Boundaries = ', MaskBoundaries)
            # You get the lower and upper part of the interval:
            lower = np.array(lower, dtype=np.uint8)
            upper = np.array(upper, dtype=np.uint8)

            # cv2.inRange is used to binarize (i.e., render in white/black) an image. All the pixels that fall inside your interval [lower, upper] will be white
            # All the pixels that do not fall inside this interval will be rendered in black, for all three channels:
            MaskColor = cv2.inRange(imgmask_in, lower, upper)
            MaskColor_rgb = cv2.cvtColor(MaskColor, cv2.COLOR_BGR2RGB)

            # AND the mask and the input image. All the pixels that are white in the mask will survive the AND operation, all the black pixels will remain black
            imgmask_out = cv2.bitwise_and(imgmask_in, imgmask_in, mask=MaskColor)
            imgmask_out_rgb = cv2.cvtColor(imgmask_out, cv2.COLOR_HSV2RGB)  # Convert to RGB for plot

            # Use the mask to count the number of white pixels. The white pixels in the mask are those that fall in the defined range
            ratio_mask = cv2.countNonZero(MaskColor) / (imgmask_in.size / 3)
            colorPercent = ratio_mask * 100  # This is the color percent calculation.

            # Print the color percent, use 2 figures past the decimal point
            print('mask pixel percentage:', np.round(colorPercent, 2))

        print("case 3 - HSV value msk")
    case _:
        print("****** Mask Selection wrong ******")
        exit(-3)


# Change vL image with anti-mask
AntiMaskColor_rgb = cv2.cvtColor(~MaskColor, cv2.COLOR_BGR2RGB)
vlimgmask_out = cv2.bitwise_and(vl_hsv, vl_hsv, mask=~MaskColor)
vlimgmask_out_rgb = cv2.cvtColor(vlimgmask_out, cv2.COLOR_HSV2RGB)  # Convert to RGB for plot
comb_img_mask_rgb = vlimgmask_out_rgb + imgmask_out_rgb

# ====================================
#         show mask img
# ====================================
fig2 = plt.figure(figsize=(12,8))
ax2_1 = fig2.add_subplot(3,3,1)
ax2_2 = fig2.add_subplot(3,3,2)
ax2_3 = fig2.add_subplot(3,3,3)
ax2_4 = fig2.add_subplot(3,3,4)
ax2_5 = fig2.add_subplot(3,3,5)
ax2_6 = fig2.add_subplot(3,3,6)
ax2_7 = fig2.add_subplot(3,3,7)
ax2_8 = fig2.add_subplot(3,3,8)
ax2_9 = fig2.add_subplot(3,3,9)

ax2_1.imshow(imgmask_in_rgb)
ax2_1.set_title('For Mask Gen')
ax2_2.imshow(MaskColor_rgb)
ax2_2.set_title('Mask')
ax2_3.imshow(imgmask_out_rgb)
ax2_3.set_title('Img after mask ')
ax2_4.imshow(vl_img_rgb)
ax2_4.set_title('VL Original')
ax2_5.imshow(AntiMaskColor_rgb)
ax2_5.set_title('Anti Mask')
ax2_6.imshow(vlimgmask_out_rgb)
ax2_6.set_title('VL img after anti-mask')
ax2_9.imshow(comb_img_mask_rgb)
ax2_9.set_title('Combined after mask')

plt.show()

```

# Images

Majority of the images were lost over time (I deleted them to clear up storage) and so the following figures are the remaining ones that I managed to recover. The same goes for the combined images. Feel free to try and run the code with the images to see the results (although I am unsure if the code is the finalized/functional version).

Originally, we removed the filter on a camera to create a full spectrum camera. Lenses were placed on top of the camera to only allow light of certain wavelengths to be captured.

All of the flower photos were taken by [Bjørn Rørslett](http://www.naturfotograf.com/UV_flowers_list.html#OXALIDCX).

## Testing the Lenses

The follow images below were taken by the students using a full spectrum camera and colored lenses. I am including the images that have been recolored using Python code (I don't think the code for the recoloring was included in the "Code" section). The purpose of recoloring was to introduce us to image recoloring by altering the RGB values in the image.

### Set One

Original image taken with a normal camera:

<img width="100%" src="https://github.com/user-attachments/assets/57872104-db88-492a-a513-71fb167addf1" />

Full spectrum camera with red lens:

<img width="100%"  src="https://github.com/user-attachments/assets/b8052293-5afb-40c6-9adc-973ee306d025" />

Full spectrum camera with green lens:

<img width="100%" src="https://github.com/user-attachments/assets/850552ae-4ea7-46e8-84fa-34a1bd6a92e3" />

Full spectrum camera with blue lens:

<img width="100%" src="https://github.com/user-attachments/assets/1f315d33-367a-491e-8908-6f4167becd25" />

Recolored image (magenta):

<img width="100%" src="https://github.com/user-attachments/assets/72340eed-5257-46e7-aca5-94ce9636d210" />

Recolored image (yellow):

<img width="100%" src="https://github.com/user-attachments/assets/59051d5b-2057-41e2-88f7-2c30c49bc4a3" />

### Set Two

Original image taken with a normal camera:

<img width="100%" src="https://github.com/user-attachments/assets/db13b06d-f72d-4dcf-b0ee-e26876d43443" />

Full spectrum camera with red lens:

<img width="100%" src="https://github.com/user-attachments/assets/c8fb6a70-8cb8-463b-9e69-d83b131c71fa" />

Full spectrum camera with green lens:

<img width="100%" src="https://github.com/user-attachments/assets/aaaa49a1-c8e8-4227-afe6-d7d6d431ac5b" />

Full spectrum camera with blue lens:

<img width="100%" src="https://github.com/user-attachments/assets/b03a5d27-6458-4a4a-a59b-1e2db6ba6b2f" />

Recolored image (magenta):

<img width="100%" src="https://github.com/user-attachments/assets/03f5a0b3-5699-4e2b-9202-4ff177b20bd2" />

Recolored image (yellow):

<img width="100%" src="https://github.com/user-attachments/assets/a426a5b1-8b76-4968-ae4a-7b3f684c8cdf" />


## Mapping Photos

*vl_h stands for visible light hue*

Some of the images may have been shifted to allow the combined image to align better, the altered images also have decreased quality since the ones with higher quality have been lost.

### Geranium Svlvaticum 

#### Linear Mapping

Table of images:

<img width="100%" src="https://github.com/user-attachments/assets/66921f10-6ded-41db-b6f3-2d36d25f622b" />

HSV distribution in images:

<img width="700" height="400" src="https://github.com/user-attachments/assets/57d8807d-140a-423f-9999-44aa53d57548" />

#### Segmented Mapping

Table of images: 

<img width="100%" src="https://github.com/user-attachments/assets/ecce81ce-37c1-444b-b899-73e26ee595ef" />

HSV distribution in images:

<img width="700" height="400" alt="Notebook (2)" src="https://github.com/user-attachments/assets/df1a9d3a-e831-485a-b9fa-99881a31a9e1" />

#### Squared Mapping 

Table of images:

<img width="100%" src="https://github.com/user-attachments/assets/2c9b4200-c359-4740-b01f-d4558a0aa0f2" />

HSV distribution in images:

<img width="700" height="400" src="https://github.com/user-attachments/assets/4d02f456-b012-4c59-98c2-2ffd3889f1b8" />

#### Square Root Mapping

Table of images:

<img width="100%" src="https://github.com/user-attachments/assets/384de720-0555-4574-9a43-5e6faf9d2c4f" />

HSV distribution in images:

<img width="700" height="400" src="https://github.com/user-attachments/assets/bac4d7df-8ced-4b9a-be63-e0717744bc0e" />


### Oxalis Fontana 

#### Linear Mapping

Table of images:

<img width="100%" src="https://github.com/user-attachments/assets/41a68abd-52c6-403a-9a7d-f0f52f2327c5" />

HSV distribution in images:

<img width="700" height="400" src="https://github.com/user-attachments/assets/3c622e7c-95b9-4256-b5f1-5c972144af4e" />

#### Segmented Mapping

Table of images:

<img width="100%" src="https://github.com/user-attachments/assets/11aa21b4-c068-4ec8-acaa-cfff3da90c67" />

HSV distribution in images:

<img width="700" height="400" src="https://github.com/user-attachments/assets/baecf42e-1977-4d75-9f95-4b957b08f75b" />

#### Quadratic Mapping

Table of images:

<img width="100%" src="https://github.com/user-attachments/assets/1b2e00cb-84a6-4a78-a4f1-d88b83fb9028" />

HSV distribution in images:

<img width="700" height="400" src="https://github.com/user-attachments/assets/ed59f73f-4d60-43f3-be91-d73d5dbf1d9e" />

#### Square Root Mapping

Table of images:

<img width="100%" src="https://github.com/user-attachments/assets/5e793fc1-2be4-4edb-a321-8153659fb475" />

HSV distribution in images:

<img width="700" height="400" src="https://github.com/user-attachments/assets/d1aaa7d9-049c-4861-b9bc-89dcfd10f0f8" />

### Kitchen Stove

#### Linear Mapping

Table of images:

<img width="100%" src="https://github.com/user-attachments/assets/9e9b734d-078e-4200-8d6d-eae31acdcfad" />

HSV distribution in images:

<img width="700" height="400" src="https://github.com/user-attachments/assets/c06ad8f0-67e1-41a6-adde-4ff41d32d2a8" />


## Masking Photos

### Kitchen Stove

Table of images:

<img width="100%" src="https://github.com/user-attachments/assets/ab397d72-0109-4c77-b436-a0125e423367" />
