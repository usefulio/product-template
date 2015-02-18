The admin application is for the power users of the product (usually the product owner, not the clients).

The advantage of splitting this out into a separate project is less boilerplate namespacing.

E.g. the route /admin/payments becomes /payments
Access control is done at one level - on login instead of every single page.
More sensitive code is not even available on the client or server of the main customer facing application reducing spillover.

./start is a bash script with the instructions to properly run this application locally
./deploy is a bash script with the instructions to properly deploy this application