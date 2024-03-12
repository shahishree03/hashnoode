---
title: "How Image Processing Revolutionizes Data Science (Day -6)"
datePublished: Wed Feb 07 2024 02:48:37 GMT+0000 (Coordinated Universal Time)
cuid: clsb6xgdn000808l28ium2on4
slug: how-image-processing-revolutionizes-data-science-day-6
canonical: https://blog.techlearnindia.com/how-image-processing-revolutionizes-data-science-day-6
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1707273840025/d6cf99f2-3419-4370-ab09-8c141435eec7.png
tags: image-processing, python, data-science

---

Welcome, image manipulators! Today, we embark on a thrilling quest: taming the corrupting forces of **noise** in our Dragon Ball Z images. Just as Goku and Vegeta train to overcome formidable villains, we'll learn noise reduction techniques to restore clarity and unleash the true potential of our images.

**What is Noise?**

Imagine tiny, unwanted pixels like Frieza's ki blasts disrupting the visual harmony of your image. Noise arises from various sources, such as sensor issues, compression artifacts, or external factors. It can mask important details and hinder image analysis.

**Meet the Noise Villains:**

* **Gaussian Noise:** Adds randomly distributed pixel values, like tiny ki blasts scattered across the image, creating a blurry, hazy effect.
    
* **Poisson Noise:** Appears as random "salt-and-pepper" specks, resembling fallen debris after an intense battle.
    
* **Salt-and-Pepper Noise:** Replaces individual pixels with either black (salt) or white (pepper) values, often mimicking scattered energy blasts.
    

**Confronting the Noise Villains:**

**1\. Gauging the Threat:**

* Examine your Dragon Ball Z image closely. What type of noise is present? What level of severity disrupts the image?
    

**2\. Choosing the Right Weapon:**

* **Gaussian Noise:**
    
    * **Gaussian Filtering:** Acts like a calming Senzu Bean, <mark>blurring</mark> the image slightly to <mark>average out noise while preserving edges</mark>.
        
    * **Non-Local Means Filtering:** Similar to Goku's Instant Transmission, intelligently <mark>smoothes noise by considering similar regions within the image</mark>.
        
* **Poisson Noise:**
    
    * **Non-Local Means Filtering:** Effective due to its <mark>noise-specific design.</mark>
        
* **Salt-and-Pepper Noise:**
    
    * **Median Filtering:** Like a Ki blast <mark>deflecting away unwanted pixels</mark>, it <mark>replaces</mark> <mark>each pixel with the median value of its neighbors</mark>, effectively removing salt-and-pepper noise.
        

3\. **Unleashing the Power of Code:**

* Import necessary libraries like `skimage` and `skimage.filters`.
    
* Load your Dragon Ball Z image.
    

```python
from skimage import io
from skimage.util import random_noise

img = io.imread('../input/gokunvegeta/wp3882112.png')
```

* **Part 1: Adding Noise**
    
    ```python
    # Gaussian noise
    img2 = random_noise(img, mode='gaussian')
    io.imshow(img2)
    ```
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1707272128716/af8ec827-c00a-42a9-9a8f-d5dabdf84339.png align="center")
    
    ```python
    # Poisson noise
    img3 = random_noise(img, mode='poisson')
    io.imshow(img3)
    ```
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1707272213074/b0be24dc-ba42-42b8-bb0e-6ce4a6babc7e.png align="center")
    
    ```python
    
    # Salt noise
    img4 = random_noise(img, mode='salt', amount=0.5)
    io.imshow(img4)
    ```
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1707272247137/7fc0f5f4-1835-4ff9-a9f8-c2136d6a5b23.png align="center")
    
    ```python
    
    # Pepper noise
    img5 = random_noise(img, mode='pepper', amount=0.5)
    io.imshow(img5)
    ```
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1707272271750/13aea9d5-5083-43fa-a92b-ff2c0a7ea753.png align="center")
    
    ```python
    
    # Salt & pepper noise
    img6 = random_noise(img, mode='s&p', amount=0.5)
    io.imshow(img6)
    ```
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1707272616179/059f6d01-bd5a-48b6-8a10-37ae3c524043.png align="center")
    

* **Explanation:**
    
    * This code loads your image named `wp3882112.png` and adds different types of noise using the `random_noise` function from `skimage.util`.
        
    * Adjust the path to your actual image.
        
    * The `amount` parameter controls the intensity of salt and pepper noise.
        
    
    **Enhancement:**
    
    * Consider displaying original and noisy images side-by-side for better comparison. Use `plt.subplot()` or create a function to display multiple images.
        
    
    **Part 2: Noise Reduction**
    
    ```python
    from skimage import io
    from skimage import filters
    
    # Gaussian denoising
    img7 = filters.gaussian(img)
    io.imshow(img7)
    
    ```
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1707272944420/ed22e8ac-f8f2-446a-a5ae-ad9aa3013dfc.png align="center")
    
    ```python
    
    # Denoising noisy image with salt & pepper noise
    img8 = random_noise(img, mode='s&p', amount=0.3)
    img9 = filters.gaussian(img8)
    io.imshow(img9)
    ```
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1707272970403/0db25714-0b3e-45f7-a855-f981a64a63d1.png align="center")
    
    ```python
    
    # Median filtering on noisy image
    img10 = random_noise(img, mode='s&p', amount=0.3)
    img11 = filters.median(img10)
    io.imshow(img11)
    ```
    
    ![](https://cdn.hashnode.com/res/hashnode/image/upload/v1707272996889/f5f31c4a-eae8-48da-b306-4f709dc44231.png align="center")
    
* **Explanation:**
    
    * This code applies two common noise reduction filters: Gaussian filter and median filter.
        
    * Gaussian filter is applied directly to the original image and to an image with salt & pepper noise.
        
    * Median filter is applied only to the image with salt & pepper noise.
        
    
    **Enhancement:**
    
    1. **Experiment with parameters:**
        
        * Adjust the `sigma` parameter for Gaussian filtering (controls smoothness).
            
        * Try different window sizes for median filtering.
            
    2. **Compare multiple filters:**
        
        * Apply both Gaussian and median filters to different types of noise and compare the results.
            
    3. **Add comments:**
        
        * Include comments within the code to explain each step and parameter.
            
    
    **Additional Information:**
    
    * Explore other noise reduction techniques like bilateral filtering or non-local means filtering, which are particularly effective for specific noise types.
        
    * Consider using more informative variable names to improve code readability.
        
    
    I hope this enhanced explanation and suggestions empower you to master noise reduction with confidence! 😉