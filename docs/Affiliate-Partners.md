#   **Affiliate Partners**

Affiliate Marketing is the process of earning commissions by promoting other people’s (or company’s) products. 

An Affiliate partner promotes a brand's products/services on their site.

A consumer clicks on the brand's promotion on the affiliate's site and is redirected to the brand's website.

Below, we will see how to create an Affiliate Partner:


##  **Create an Affiliate Partner**

*   Go to <a href="https://www.mycrush.fit/wp-admin" target="_blank">**mycrush.fit/wp-admin**</a>
*   Login with the credentials.
*   Go to -> **Affiliate Partners** -> **Add New**

    ![dashboard](images\Affiliate-Partner\dashboard.jpg)

### **Name**

-   Add the affiliate name in this field.

    ![name](images\Affiliate-Partner\name.jpg)


### **Affliate Partners Field Group**

####    **Logo**

-   Insert an affiliate related image. Select image from the list.

    ![logo](images\Affiliate-Partner\logo.jpg)

####    **Redeem Code**

-   The coupon codes that can be redeemed are uploaded using a CSV File.

    ![redeem code](images\Affiliate-Partner\redeemcode.jpg)

####    **Signup**

-   In this field, enter the code from the URL of the [Sign-up](#sign-up-page) page.

####    **Signin**

-   In this field, enter the code from the URL of the [Sign-in](#sign-in-page) page.

![signupin](images\Affiliate-Partner\signupin.jpg)


### **Publish**

-   Click **Publish** to save the affiliate partner created.

    ![publish](images\Affiliate-Partner\publish.jpg)

Once the affiliate partner is published, a code is generated in the URL. 

**Copy the code in the URL and paste it in the Sign-in and Sign-up pages.**

##  **Create Sign-up and Sign-in Pages**

To give the customers the option of Sign-up or Sign-in, two pages have to be created. Follow the below steps for the same:

*   Go to <a href="https://www.mycrush.fit/wp-admin" target="_blank">**mycrush.fit/wp-admin**</a>
*   Login with the credentials
*   Go to -> **Pages** -> **Add New**

    ![add new page](images\Affiliate-Partner\pageaddnew.jpg)


### **Sign-up Page**

For the sign-up page, the below fields need to be filled:

####    **Add Title**

-   Add title as "Affiliate name-Signup""

####    **Shortcode**

-   In the shortcode field, a pre-defined format needs to be entered. The code from the affiliate partner URL is entered in the shortcode. The below format should be used:

    **[affliate-form affliate='Code copied from the affiliate partner URL']**

![signup](images\Affiliate-Partner\signup.jpg)

-   Copy the code from the URL and paste in the Sign-up field of the Affiliate Partner.

    ![signup code](images\Affiliate-Partner\signupcode.jpg)


### **Sign-in Page**

For the sign-in page, the below fields need to be filled:

####    **Add Title**

-   Add title as "Affiliate name-Signin""

####    **Shortcode**

-   In the shortcode field, a pre-defined format needs to be entered. The code from the affiliate partner URL is entered in the shortcode. The below format should be used:


    **[affliate-form-sign-in affliate="Code copied from the affiliate partner URL"]**

![signin](images\Affiliate-Partner\signin.jpg)  

-   Copy the code from the URL and paste in the Sign-in field of the Affiliate Partner.

    ![signin code](images\Affiliate-Partner\signincode.jpg)


##  **Upload coupons using CSV File**

The redeemable coupons provided to customers are uploaded using a CSV file. Follow below steps to create a CSV file:

### **Create a CSV File**

Create a new excel file and save it with .csv extension.

### **CSV Columns to be populated**

The CSV file should have the below columns in order to upload the affiliate partner coupons. Below columns should be filled manually:

####    **redeem-code**

These are the codes which need to be uploaded and are offered to the users to redeem. Below are some rules to be followed while entering the codes in the CSV file:

-   All codes should be alpha-numeric without any special characters.
-   A single code can be used for multiple product ids.
-   Multiple codes can be used for a single product id.
-   A single coupon code can be used multiple times.

####    **redeem-code-product-id**

This field consists of the product id designated to various products available to the users. This will specify the product on which the coupon can be redeemed. Follow below rules while filling this field:

-   Enter "product id" = for any other class. For eg: 12322, 12323


####    **redeem-code-used**

This field shows if the coupon code has been redeemed or not. While updating the CSV file, this field by default is "0".


####    **redeem-code-user-email**

This field gets updated with the user email when the code is redeemed. 

**Some important points to remember:**

-   Once a coupon code is created, it cannot be deleted or edited.
-   Only new coupon codes can be added to the existing file.
-   Column names are very important and should be entered correctly otherwise the coupons will not work properly.

Below is a Sample CSV:

![csv1](images\Affiliate-Partner\csv1.jpg)

<a href="https://docs.google.com/spreadsheets/d/1OVrRBuuLrbxcec-43ZHRcpN3yOezVG2Jy1lBkTsSFPA/edit?usp=sharing" target="_blank">**Sample CSV - Affiliate**</a> 

### **Importing the CSV File**

The final step is to upload the coupon codes so they can be applied. This is done by importing the updated CSV file. Follow the steps below:

1.  Go to-> **Crush Reports** at the left side panel.

    ![export1](images\Affiliate-Partner\export1.jpg)

2.  Click -> **Import Affiliate** 

    ![importaff](images\Affiliate-Partner\importaff.jpg)

3.  **Select Affiliate** - for whom the coupons need to be uploaded 

    ![selectaff](images\Affiliate-Partner\selectaff.jpg)

4.  **Coupon CSV** - choose the csv file to be uploaded

    ![couponcsv](images\Affiliate-Partner\couponcsv.jpg)

5.  Click **Import Codes** to move to start uploading

    ![importcode](images\Affiliate-Partner\importcode.jpg)

6.  The file import % or finished status will be displayed on the screen.

    ![importstatus](images\Affiliate-Partner\importstatus.jpg)


##  **Crush Reports**

Crush Reports section displays downloadable reports about all the affiliates. The reports provide information about the redeemable codes and the products on which the coupons are applied. It displays the status of the coupons - if redeemed or not.

To access reports:

*   Go to <a href="https://www.mycrush.fit/wp-admin" target="_blank">**mycrush.fit/wp-admin**</a>
*   Login with the credentials
*   Go to -> **Crush Reports**

![crush reports](images\Affiliate-Partner\crushreports.jpg)

![reports](images\Affiliate-Partner\reports.jpg)

The below fields are tracked in the report:

1.  **ID**
2.  **redeem-code:** This is the coupon code provided to the customer
3.  **redeem-code-product-id:** This the product id for the respective products on which the coupon is applicable.
4.  **redeem-code-product-name:** This is the name of the product on which the coupon is applicable.
5.  **redeem-code-status:** This field provides information if the coupon code has been redeemed or not.

    -   0 = means not redeemed yet
    -   1 = means coupon has been redeeemed

6.  **redeem-code-user-email:** This field captures the email id of the customer who has redeemed the coupon

    ![report sample](images\Affiliate-Partner\reportsample.jpg)

:bookmark: <a href="https://docs.google.com/spreadsheets/d/1Pcw6t6xGXr2EZsd0m1V36IXb2m4ZmjnUMc-gSxW7lLk/edit?usp=sharing" target="_blank">**Sample Crush Report**</a> 