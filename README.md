# image-metadata

## required
* browser (eg. Chrome, firefox, Safari)
* AWS account
* genRetrivePhotoWeb.yaml
* lots of photos (img9.zip)

## create a stack
1. open browser, login to AWS.
2. confirm you are in the "us-east-1" region.
3. go to CloudFormation Console.
4. click "create stack" >> "with new resources (standard)"
5. in step1 page: 
    * select:
        * Prerequisite - Prepare template: Template is ready
        * Specify template: Upload a template file
            * upload file: genRetrivePhotoWeb.yaml
    * click "next" to step2 page.
6. in step2 page: 
    * type in:
        * Stack name: [name it by yourself]
        * Parameters: 
            * BucketName: [name it by yourself]
    * click "next" to step3 page.
7. in step3 page: 
    * Do nothing in this page.
    * click "next" to step4 page.
8. in step4 page: 
    * scroll down the page, and confirm all the 3 checkboxs in "Transforms might require access capabilities"
    * click "create stack" to generate the app, waiting for the status is "CREATE_COMPLETE".
9. click the tab "output", there is a key named "WebURL". It's the web's url, click its value link to go to the web.

## How to retrieve photos' metadata
1. click "Choose Files" to upload all the photos you have.
2. wait for all the photos retieved in the "Show Images:" section.
3. see Screen Shot_9.PNG or Screen Shot_900photo.PNG.
ps. location could be showed slower.

![](https://github.com/mandy-shen/image-metadata/blob/main/Screen%20Shot_900photo.png | width=50)
