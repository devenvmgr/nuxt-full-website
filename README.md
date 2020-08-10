# nuxt-full-website

The goal of this project is to allow future Rockys (and maybe you) to quickly scaffold a Vue-Tailwind project. 




## TODO LIST

Priority: 
[] - Add a background that looks all funky (like this) --> https://blog.hubspot.com/hubfs/shopify-blog-1.png
[] - Add a border 
[] - Add Popups with toast - https://getbootstrap.com/docs/4.3/components/toasts/
[] - Add Popups that take over the screen.
[] - Add Popups that spit canvas
[] - Add Popups that spit video


Secondary: 
[] - Set tailwind to purge. 
[] - fix footer to be 3-col. 
[] - Fix hero image to look like this https://codetiburon.com/app/uploads/2017/05/2-1.png
[] - Fix Nav to look like this (logo + menu + cta) https://codetiburon.com/app/uploads/2017/05/3.png
[] - make mobile responsive
[] - move tailwind classes into vue side of things. 
[] - Tailwind SASS -- https://tailwindcss.com/docs/using-with-preprocessors/
[] - Fix the form to be contact us.
[] - Add button code to make buttons look normal. 
[] - Image Carosel is garbage. --> https://getbootstrap.com/docs/4.3/components/carousel/
[] - Fix Center CTA
[] - Add bootstrap Accordion -- https://getbootstrap.com/docs/4.3/components/collapse/
[] - Add badges -- https://getbootstrap.com/docs/4.3/components/badge/
[] - In blog, add pagination - https://getbootstrap.com/docs/4.3/components/pagination/
[] - Add Popovers
[] - Add tabbed content - But sexy - https://blog.hubspot.com/hubfs/transferwise-landing-page-1.png

Wishlist: 

## Component List

* BITS - these are reusable components. They are given props. 
  * ImageColumn - Image, Header, Body, Button. (all are optional)
  * TestimonialColumn - Text, circular image, name, and title
  * Popup - header, body, footer

* Containers - These are using bits to generate other content. Modify these boys.
  * Header - Contains Navigation. 
  * [not yet] Header-Dropdowns - Contains Navigation WITH dropdowns. 
  * Footer - Contains a 3-col system (branding, links, links) with copyright bottom col.
  * HeroImage - Big Splash Image with Text/buttons. 
  * ImageColumn_Group - uses 3-5 ImageColumn bits.
  * ImageColumn_Hero - uses a single ImageColumn and design code.
  * Testimonial_Group - uses 3-5 TestimonialColumn bits.
  * BlogContent - Title, subtext, 2 paragraph snippet and button.
  * SocialButtons - a list of social media buttons. 
  * FormContactUs - a standard form. 
  * CenterCTA - A call to action center area. 
  * Popup_Button - A call to the popup bit.

## Build Setup

```bash
# install dependencies
$ npm install

# serve with hot reload at localhost:3000
$ npm run dev

# build for production and launch server
$ npm run build
$ npm run start

# generate static project
$ npm run generate
```

For detailed explanation on how things work, check out [Nuxt.js docs](https://nuxtjs.org).
