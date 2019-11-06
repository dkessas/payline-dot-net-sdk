Composition du SDK

Le SDK  .NET est composé d'une librairie de fonctions qui permet d'utiliser les fonctions de l'API Payline.

Configuration du SDK
Une fois le SDK référencé dans votre projet, vous devez renommer le fichier payline.properties.default.xml en payline.properties.xml et associer des valeurs aux paramètres de configuration.

Exemple de configuration :

<?xml version="1.0"?>
<PaylineProperties xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <DirectPaymentAPIUrl>https://homologation.payline.com/V4/services/DirectPaymentAPI</DirectPaymentAPIUrl>
  <MassPaymentAPIUrl>https://homologation.payline.com/V4/services/MassPaymentAPI</MassPaymentAPIUrl>
  <WebPaymentAPIUrl>https://homologation.payline.com/V4/services/WebPaymentAPI</WebPaymentAPIUrl>
  <ExtendedAPIUrl>https://homologation.payline.com/V4/services/ExtendedAPI</ExtendedAPIUrl>

  <DirectPaymentAPIUrlProd>https://services.payline.com/V4/services/DirectPaymentAPI</DirectPaymentAPIUrlProd>
  <MassPaymentAPIUrlProd>https://services.payline.com/V4/services/MassPaymentAPI</MassPaymentAPIUrlProd>
  <WebPaymentAPIUrlProd>https://services.payline.com/V4/services/WebPaymentAPI</WebPaymentAPIUrlProd>
  <ExtendedAPIUrlProd>https://services.payline.com/V4/services/ExtendedAPI</ExtendedAPIUrlProd>

  <Production>false</Production>
  <accessKey>abcdefghijklmnopqrst</accessKey>
  <merchantID>123456789</merchantID>
  <proxyHost />
  <proxyPort />
  <proxyLogin />
  <proxyPassword />
  <!-- Payline pages language -->
  <DefaultLanguageCode>EN</DefaultLanguageCode>
  <DefaultPaymentCurrency>978</DefaultPaymentCurrency>
  <DefaultOrderCurrency>978</DefaultOrderCurrency>
  <DefaultSecurityMode>SSL</DefaultSecurityMode>
  <DefaultLanguage>english</DefaultLanguage>
  <DefaultPaymentAction>100</DefaultPaymentAction>
  <DefaultPaymentMode>CPT</DefaultPaymentMode>
  <!-- Default cancel URL -->
  <DefaultCancelUrl>https://www.url.fr</DefaultCancelUrl>
  <!-- Default notification URL -->
  <DefaultNotificationUrl>https://www.url.fr</DefaultNotificationUrl>
  <!-- Default return URL -->
  <DefaultReturnUrl>https://www.url.fr</DefaultReturnUrl>
  <!-- Contract type default (ex: 001 = CB, 003 = American Express...) -->
  <DefaultContractNumber>CB</DefaultContractNumber>
  <!-- Contract type multiple values (separator: ;) -->
  <DefaultContractNumberList>CB;</DefaultContractNumberList>
  <SecondContractNumberList></SecondContractNumberList>
  <!-- For 3D Secure authentication -->
  <TermUrl>https://www.url.fr</TermUrl>
  <CustomPaymentPageCode></CustomPaymentPageCode>
  <CustomPaymentTemplateUrl></CustomPaymentTemplateUrl>
  <Web2TokenKey></Web2TokenKey>
  <Web2TokenProdUrl>https://webpayment.payline.com/webpayment/getToken</Web2TokenProdUrl>
  <Web2TokenHomoUrl>https://homologation-webpayment.payline.com/webpayment/getToken</Web2TokenHomoUrl>
  <Web2TokenContractNumber>1234567</Web2TokenContractNumber>
  <Web2TokenCallbackUrl>https://www.url.fr</Web2TokenCallbackUrl>

</PaylineProperties>