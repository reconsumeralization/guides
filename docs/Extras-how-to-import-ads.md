# How to import ads

It’s much easier to import advertisements instead of inserting them one by one.

## How to use this feature

Create a CSV file in utf8 with header (lower case): user_name user_email title description date category location price address phone website locale* stock* image_1 image_2 image_3 image_4 .. (as many images as you have setup in the system)

 - **user_name:**  Name for user if doesn’t exists will get created.
 -  **user_email:**  Email address of user if doesn’t exists will get created.
 -  **title:**  Title of the ad, will be used later for the url for SEO.
 -  **description:**  Ad description details. Allows bbcode.
 -  **date:**  Published date, in format YYYY-MM-DD (for example 2014-05-09).
 -  **category:**  Name of the category will be created if doesnt exists.
 -  **location:**  Name of the location will be created if doesnt exists.
 -  **price:**  Price, numeric (optional).
 -  **address:**  Address of the ad, (optional).
 -  **phone:**  Phone number (optional).
 -  **website:**  Website (optional).
 -  **locale:**  locale of the ad, ex fr_FR (* optional, only add in the header if you have multilingual enabled).
 -  **stock:**  number (* optional, only add in the header if you have stock control enabled).

**Images:**

We allow to upload as many images as you configured, so if you allow 4 images in the CSV you need to have 4 columns, even if they are empty add them. Images allow remote images like  [http://lorempixel.com/1200/800/technics/](http://lorempixel.com/1200/800/technics/s)  or local, using as base your site root, for example /images/import/ad1_pic3.png. The images will be downloaded, resized, thumbed, and deleted on completion.
image_1
image_2
image_3
image_4

**Custom Fields:**

Note : If you have custom fields created, it is mandatory that you add the fields in the CSV file as headers, with the prefix  **cf_**. 

For example, if you have a custom field called “currency_name” in your site, you need to include it in the CSV file headers as “cf_currency_name”.

[**Download Sample CSV file**](https://raw.githubusercontent.com/yclas/guides/master/samples/import_ads_with_cf_example.csv) working for 4 images without locale or stock.

You can use this easy import tool to add all of your ads with a press of a button. You simply need to follow those steps:

-   Log into your  **Admin Panel**.
-   Go to  **Tools**  >  **Import Ads**.
-   Click on  **Choose File**  to select your CVS file and then press  **Upload**.
-   Now click on **Process**  on the **Process Queue** box which is displayed on the right side of the page.

You can now see the imported ads on **Manage** -> **Advertisements**.


**Related posts:**

-   [How to use import tool for categories and locations?](Classifieds-how-to-import-tool-for-categories-and-location.md)

-   [How to manage advertisements?](Classifieds-manage-advertisements.md)
