- 👋 Hi, I’m @malandro0
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-
braintree.dropin.create({
  authorization: 'CLIENT_AUTHORIZATION',
  container: '#dropin-container',
  googlePay: {
    googlePayVersion: 2,
    merchantId: 'merchant-id-from-google',
    transactionInfo: {
      totalPriceStatus: 'FINAL',
      totalPrice: '123.45',
      currencyCode: 'USD'
    },
    allowedPaymentMethods: [{
      type: 'CARD',
      parameters: {
        // We recommend collecting and passing billing address information with all Google Pay transactions as a best practice.
        billingAddressRequired: true,
        billingAddressParameters: {
          format: 'FULL'
        }
      }
    }]
  }
}, callback);
<!---
malandro0/malandro0 is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
