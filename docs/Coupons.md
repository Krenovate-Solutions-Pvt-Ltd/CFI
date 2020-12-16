#   **Coupons**

##  **Introduction**

Coupons are a great way to offer discounts and rewards to your customers, and can help promote sales across your shop.

Coupons can be uploaded/imported one by one or in bulk.

In this section, you will learn the bulk methodology to upload/import multiple coupons in one go. This is done by uploading a CSV file using the **Ultimate CSV Importer PRO.**

##  **CSV File**

Before we learn how to upload coupons, let's learn about a CSV file. 

### **What is a CSV File?**

It is an excel file with the extension ".CSV". All the required data is populated in this CSV file in a pre-defined format. The file has columns dedicated to each field corresponding to the fields in the backend.

Maintaining the format of all columns is of utmost importance in order to import all data correctly.

A sample CSV file is below:

![sample csv](images\Coupons\samplecsv.jpg)

<a href="https://docs.google.com/spreadsheets/d/1chs891NJEUcwYyTBVv-hyAN_eOvG_WWfjxFOwAkjEtI/edit?usp=sharing" target="_blank">**Sample CSV**</a> 


### **CSV Columns**

The below table gives a brief description of all the column fields of a CSV file:


**WP Fields** | **CSV Header** | **Description** | **CSV Sample Value**
---------|----------|---------|---------
 *Coupon Code | coupon_code | It is used to specify the code of the coupon in the CSV file. You can generate coupon code by using numerical, alphabet, and special character.  | JJ8kC
 Description | Description | Enter text to describe the coupon | Discount for product
 *Status | post_status | Specify the status for the coupon | publish
 *Discount Type | discount_type | Mention one of the discount types:  Cart Discount; Cart % Discount; Product Discount; Product % Discount | fixed_cart = Cart Discount; percent = Cart % Discount; fixed_product = Product Discount; percent_product = Product % Discount
 *Coupon Amount | coupon_amount | Specify the coupon amount in decimal form without thousand separators and currency symbols. According to the Discount type please specify the coupon amount in the CSV file | 34.896
 Individual Use | individual_use | Specify that the coupon is used in conjunction with other coupons or not. Yes - not used in conjunction with other coupons; No - Used in conjunction with other coupons | yes/no
 *Product Ids | product_ids | Enter the id of the products which you want to be discounted | 27,532,756
 Exclude Product Ids | exclude_product_ids | Enter the id of the products which you do not want to discount | 275,327
 Usage Limit | usage_limit | Specifies how many times a coupon can be used by all customers before being invalid. | Enter numeric value
 Usage Limit Per User | usage_limit_per_user | Specify how many times a coupon can be used by each customer before being invalid for that customer. | Enter numeric value
 Limit Usage | limit_usage_to_x_items | Specify how many items the coupon can be applied to before being invalid. This field is only displayed if there is one or more products that the coupon can be used with, and is configured under the Usage Restrictions. | Enter numeric value
 *Expiry Date | expiry_date | Specify the coupon expiry date | **Date format to be followed : yyyy-mm-dd** eg: 2015-02-14
 Free Shipping | free_shipping | Specify if shipping required or not | Yes/No
 Exclude Sale Items | exclude_sale_items | Specify whether the coupons apply to items on sale or not. Yes - coupons should not apply to items on sale; No - coupons apply to items on sale | yes/no
 Product Categories | product_categories | Specify the category id of the product to be discounted | 740,062
 Exclude Product Categories | exclude_product_categories | Specify the category id of the product not to be discounted | 1,510,172
 Minimum Amount | minimum_amount | Allows you to set the minimum subtotal needed to use the coupon.  Note: The sum of the cart subtotal + tax is used to determine the minimum amount. | Enter numeric values
 Maximum Amount | maximum_amount | Allows you to set the maximum subtotal allowed when using the coupon. | Enter numeric value
 Customer Email | customer_email | Allows Emails/Email restrictions – Email address or addresses that can use a coupon. It can be left blank. | abc@xyz.com

### **Mandatory Rules to Follow**

While entering data in the CSV columns, few rules are mandatory to be followed:

-   Date format to be followed : **yyyy-mm-dd**
-   For fields where product id or category has to be entered : the excel field format should always be **"Text"**
-   Column fields with a star "*" in the above table are required fields, rest are optional.
-   Leaving “Products” and “Exclude Products” blank allows the coupon to be applied to the entire store.

##  **How to Import Coupons?**

Here, you will see a step by step tutorial on how to import coupons using the Ultimate CSV Importer. Follow the below steps:

*   <a href="https://online.crushfitnessindia.com/wp-admin" target="_blank">Go to **online.crushfitnessindia.com**</a>
*   Login with the credentials.
*   Go to -> **Ultimate CSV Importer Pro** at the bottom on left side panel.

    ![dashboard](images\Coupons\dashboard.jpg)

### **Import/Update**

-   Go to -> **Import/Update**
-   Choose the location from where you want to upload the file.
-   Select the respective file.

    ![import](images\Coupons\import.jpg)

-   Click the option -> **New Item**

    ![new item](images\Coupons\newitem.jpg)

-   Under **Import each record as** -> Select **WooCommerece Coupons** from list

    ![wcoupons](images\Coupons\wcoupons.jpg)

-   Click -> **Continue**

Once the CSV file is uploaded, the fields in the mentioned sections have to be mapped with the respective fields as in the images below:

![core fields](images\Coupons\corefields.jpg)

![coupon meta fields](images\Coupons\couponmetafields.jpg)

![coupon meta fields1](images\Coupons\couponmetafields1.jpg)

-   On the next screen, click -> **Import**

    ![import1](images\Coupons\import1.jpg)

-   Once the file import is complete, you will see the below screen with the import details:

    ![import complete](images\Coupons\importcomplete.jpg)


##  **Check Coupon Import**

In order to check if the coupons have been uploaded correctly, follow the below steps:

-   Go to -> **Marketing** -> **Coupons**

    ![marketing](images\Coupons\marketing.jpg)

-   Check for the added coupon codes in the list

    ![coupon list](images\Coupons\couponlist.jpg)

-   Click on coupon code and check the Coupon Data fields, to confirm if the coupon details such as linked product id etc have been uploaded appropriately.

    ![coupondata](images\Coupons\coupondata.jpg)

    ![coupondata1](images\Coupons\coupondata1.jpg)

    ![coupondata2](images\Coupons\coupondata2.jpg)


## **Help & Guides**

-   :computer: Watch the <a href="https://www.youtube.com/watch?v=b3Ix0WB3Bwg&t=196s" target="_blank">**Video Tutorial**</a> to understand how to use the CSV Importer.
-   :computer: Click here to <a href="https://docs.woocommerce.com/document/coupon-management/#section-1" target="_blank">**Learn How to Add a Coupon manually**</a> and about all the fields.