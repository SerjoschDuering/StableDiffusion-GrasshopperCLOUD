# StableDiffusion-GrasshopperCLOUD
A Grasshopper client for the stable-diffusion model hosted by replicate.com, with support for img2img and image in-painting. This implementation allows getting started with grasshopper and stable-diffusion
hassle-free. No local installations are required. However, you will need an account at replicate.com + incl. billing infomration as they host and run the model on their hardware. On average, one prediction (image) will roughly cost one cent (€).


![Untitled](https://github.com/SerjoschDuering/Grasshopper-StableDiffusion/raw/main/images/Untitled.png)
![Untitled](https://github.com/SerjoschDuering/Grasshopper-StableDiffusion/raw/main/images/spcow.PNG)

## Prerequisites

1) Create an Account at replicate.com 

2) Grasshopper Plugins

In order to use this client with an Interface you need the plugin:
- [HumanUI](https://www.food4rhino.com/en/app/human-ui)
- optional: [Aviary](https://www.food4rhino.com/en/app/aviary)
- optional: [Hops](https://developer.rhino3d.com/guides/compute/hops-component/)


## Set-up

1. Open Rhino 7+, launch grasshopper and open SD_Client_UI.gh
2. in the settings tab of the humanUI window paste your authentication token from replicate.com (you will get one when signing up)
3. in the same tab, set the viewport name that will be used to take screen captures
4. switch to the model tab, draw some geometries to the Rhino canvas and hit run model!

![Untitled](https://github.com/SerjoschDuering/StableDiffusion-GrasshopperCLOUD/raw/main/docs/UIA.PNG)

**Sample Images** 

Naturally, the model is not limited to a particular domain

![Untitled](https://github.com/SerjoschDuering/Grasshopper-StableDiffusion/raw/main/images/Untitled%202.png)

![Untitled](https://github.com/SerjoschDuering/Grasshopper-StableDiffusion/raw/main/images/Untitled%203.png)

### Experimental implementation of the image-infill mode:
Interesting for integrating designs into an existing context that should be kept stable. In this example a background image was placed on the canvas and the area of the church was masked with red colored geometry. 
![infill](https://github.com/SerjoschDuering/StableDiffusion-Grasshopper/raw/main/docs/assets/grasshopper/infill.png)

Here are some more examples: A) without using masks B) using masks and geometry and C) only using an image mask
![infill2](https://github.com/SerjoschDuering/StableDiffusion-GrasshopperCLOUD/raw/main/docs/infillExamples.PNG)
