# Publishing as a Website
Exporting Construct game into a website using Microsoft azure

* Before beginning ensure that you have activated your student access to azure be following the fourth session

## Lets Begin
  1. Open a web browser
  2. Go to [portal.azure.com](https://portal.azure.com/)
  3. Log in with the credentials that you activated your dream spark account with

## Creating a new website
  1. Click on "New" in the top left corner of the portals home page
  2. Click on "Web + Mobile" under the Market Place heading
  3. Click on "Web App"
  4. Fill out the information about your web app
    - Note you should get a tick next to your "App Service Name"
    - To access the website once completed you will go to yourWebAppsName.azurewebsites.net
  5. Leave the other fields as the default and click **Create** at the bottom  

##### Azure is now deploying the Web App in the background
##### Whilst waiting open the Construct 2 application with the game you would like to deploy

## Exporting the game to OneDrive
  1. Click on the root folder in Construct 2 in the top right
  2. Change the "Name" of your game to what you desire in the top left under
  3. After this open up the home ribbon and click "Export Project"
  4. Choose "HTML5 website" in the **Web** Group and click on "Next"
  5. Choose the directory you would like to export the files to eg. Desktop and click "Next"
  6. Click "Normal style" and then "Export"
  7. After you have gone through this process you will have a folder containing all the relevant files in the directory you chose.

#### Now let's go back to the browser with Azure
 * Your Web App should automatically open up in the portal
 * If it doesn't open up, click the tile named after your Web App in the portals home page

## Loading website onto Azure
  1. Click settings
  2. Scroll down and under the "PUBLISHING" group click "Continuous deployment"
  3. Choose source and pick "OneDrive"
  4. Choose "Authorization" and click the **Authorize** button
    - By having a Microsoft account you will have access to One Drive
  5. Click on **Yes** in the window that opens
    - A folder is now created in your One Drive that is linked to the Web App you have deployed
  6. Click "Okay" after choosing the folder that is created.

## Adding Files to One Drive
  1. Open a new tab in your browser
  2. Go to [onedrive.com](https://onedrive.live.com/about/en-nz/)
    - An "Apps" folder will now be created in your One Drive
  3. Click on the "Apps" folder, "Azure Web Apps" and then the folder which your Web App is named after
  4. Select all the items from the directory you exported to from Construct
  5. Drag these files into your One Drive folder in One Drive
    - It will take a moment for all the files to upload
    - Ensure that the file structure in the browser is the same as the one on your local machine i.e. if there is an images folder make sure that it exists as it is. All other files should be in the root level of the folder

## Final Synchronization and Browsing
  1. Go back to the tab with Azure
  2. Click on "Sync" under Deployments and then choose "Yes"
    - The One Drive folder is now being checked for any changes to the folder and uploading and publishing them
  3. Once Synchronization is complete click on **Browse**
    - A new tab will open automatically and run your game in the browser

#### You can now share this link with friends and family and let them enjoy your game as well.
#### Congratulation you have successfully created a game and published it to Azure

A video walkthrough by our student partners can also be found on [YouTube](https://www.youtube.com/watch?v=Jvt18Y_ky1c)
