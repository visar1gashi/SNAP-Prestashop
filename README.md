
Midtrans&nbsp; Prestashop Payment Gateway Module
=====================================


Midtrans&nbsp;  :heart: Prestashop!
Let your Prestashop store integrated with Midtrans&nbsp;  payment gateway.

### Description

Midtrans&nbsp;  payment gateway is an online payment gateway. They strive to make payments simple for both the merchant and customers. With this plugin you can allow online payment on your Prestashop store using Midtrans&nbsp;  payment gateway.

Payment Method Feature:
- Midtrans&nbsp; Snap all payment method fullpayment
- Credit card online & offline installment payment
- Credit card BIN & bank transfer promo payment
- Credit card MIGS acquiring channel

### Installation Instruction

#### Minimum Requirements

* Prestashop 1.6
* PHP version 5.4 or greater
* MySQL version 5.0 or greater

#### Installation & Configuration
1. [Download](../../archive/master.zip) the modules from this repository.
2. Extract the modules, then rename the folder modules as **midtranspay** and zip this modules as **midtranspay.zip**
3. Go to your Prestashop administration page and go to **"Modules and Services > Modules and Services"** menu.
4. Click on the **"Add a new module"** and locate the **midtranspay.zip** file, then upload it.
5. Find the **Midtrans Pay** module in the module list and click **install**, then enable it.
6. Find the **Midtrans Pay** module in the module list and click **configure**
  * Fill **Payment Button Display Title** with text button that you want to display to customer
  * Select **Environment**, Sandbox is for testing transaction, Production is for real transaction
  * Fill in the **client key** & **server key** with your corresonding [Midtrans&nbsp;  account](https://dashboard.midtrans.com/) credentials
  * Note: key for Sandbox & Production is different, make sure you use the correct one.
  * **Map payment SUCCESS status to:** select your desired order status when payment is success.
  * **Map payment FAILURE status to:** select your desired order status when payment is failure.
  * **Map payment PENDING/CHALLENGE status to:** select your desired order status when payment is challanged.
  * Other configuration are optional, you may leave it as is.


### Midtrans&nbsp;  MAP Configuration

1. Login to your [Midtrans&nbsp;  Account](https://dashboard.midtrans.com), select your environment (sandbox/production), go to menu `settings > configuration`
   * Payment Notification URL: `http://[your-site-url]/index.php?fc=module&module=midtranspay&controller=notification`
   * Finish Redirect URL: `http://[your-site-url]/index.php?fc=module&module=midtranspay&controller=success`
   * Unfinish Redirect URL: `http://[your-site-url]/index.php?fc=module&module=midtranspay&controller=back`
   * Error Redirect URL: `http://[your-site-url]/index.php?fc=module&module=midtranspay&controller=failure`

#### Get help

* [SNAP-Prestashop Wiki](https://github.com/veritrans/SNAP-Prestashop/wiki)
* [Veritrans registration](https://dashboard.midtrans.com/register)
* [SNAP documentation](http://snap-docs.midtrans.com)
* Can't find answer you looking for? email to [support@midtrans.com](mailto:support@midtrans.com)
