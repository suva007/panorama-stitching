# panorama-stitching

![Portion-Watermarking](https://socialify.git.ci/suva007/panorama-stitching/image?description=1&font=Raleway&pattern=Brick%20Wall&theme=Dark)
- <a href="https://github.com/suva007/panorama-stitching/blob/main/panorama.ipynb" title="Link to notebook" style="background-color:#FFFFFF;color:#000000;text-decoration:none">📚 Link to notebook </a>

## Prerequisite
- Sift and surf cannot be used with new versions of open-cv that is why using orb local invariant descriptor.
- Orb is based on = FAST keypoint detector and the BRIEF descriptor
- ![image](https://user-images.githubusercontent.com/38084433/148696156-b5ea863b-9886-4587-af16-6cc2954d9f02.png)
- (lighter than p, darker than p or similar to p).
- If more than 8 pixels are darker or brighter than p than it is selected as a keypoint.
- In brief, each keypoint is described by a feature vector which is 128–512 bits string.
- ![image](https://user-images.githubusercontent.com/38084433/148696198-5a6b6047-8392-4511-8d9e-fd70c0e63947.png)
- BRIEF is not rotation invariant , so ORB uses rotation aware brief.

## Implementation
- STEP 1 : READ IMAGES AND TRANSFROM THEM TO GRAYSCALE.
![image](https://user-images.githubusercontent.com/38084433/148696278-48a65596-7cb8-4a39-b689-ca354783286e.png)

- STEP 2 : Function to Detect & Describe the Feature Descriptors.

- STEP 3 : Displaying Keypoints Extracted from the function call of previous step.

![image](https://user-images.githubusercontent.com/38084433/148696299-b1695c10-aa26-43e6-8381-cbae4166a27c.png)

- STEP 4 : Create and return a Matcher Object

- STEP 5 : RAW Matches
![image](https://user-images.githubusercontent.com/38084433/148696376-584a94ae-6e76-4ff6-a9e4-cf632de02f8d.png)

- STEP 6 : Homography Matrix computation

- STEP 7 : Panaroma Correction

![image](https://user-images.githubusercontent.com/38084433/148696397-27437b8c-491e-4e5f-86cf-88cfec790ca0.png)

- STEP 8 : Transform the panorama image to grayscale and threshold it
![image](https://user-images.githubusercontent.com/38084433/148696409-15ef261e-0584-40a6-bf19-a3f20bf191c4.png)

## :wink: Thanks

