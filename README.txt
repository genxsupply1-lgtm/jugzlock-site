JUGZLOCK.COM – SITE FILES
=========================

WHAT'S HERE
  index.html   the whole site (pages, styles and buy buttons)
  img/         product photos

PUT IT ONLINE (Cloudflare Pages, free)
  1. Cloudflare dashboard > Workers & Pages > Create > Pages > "Upload assets".
  2. Name the project "jugzlock" and drag in this whole folder (or the zip).
  3. Deploy. You get a jugzlock.pages.dev link to check it.
  4. In the project: Custom domains > Set up a custom domain > jugzlock.com
     (then add www.jugzlock.com too). Cloudflare sets up the DNS and SSL.
  To update later: open the project > Create deployment > upload the new folder.

ADD YOUR SQUARE PAYMENT LINKS
  Open index.html and find "EDIT HERE". Each product option has  square:""
  Paste the Square link between the quotes, for example:
     "Black":{price:29.95,square:"https://square.link/u/AbCdEf"},
  Any option left as "" sends the buyer to the matching genx-supply.com page.
  Make the price on the site match the price on the Square link.

ADD / REPLACE PRODUCT PHOTOS
  All product photos are in img/. To swap one, save the new picture as a .jpg
  with the same file name.

EMAIL
  The site lists orders@jugzlock.com. Turn it on in Cloudflare:
  jugzlock.com > Email > Email Routing > forward orders@ to your Gmail.
