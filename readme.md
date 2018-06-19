
Demo Event Page: http://attendize.website/e/799/attendize-test-event-w-special-guest-attendize
---


*Attendize* is an open-source event ticketing and event management application built using the Laravel PHP framework. Attendize was created to offer event organisers a simple solution to managing general admission events, without paying extortionate service fees.

Current Features (v1.X.X)
---
 - Beautiful mobile friendly event pages
 - Easy attendee management - Refunds, Messaging etc.
 - Data export - attendees list to XLS, CSV etc.
 - Generate print friendly attendee list
 - Ability to manage unlimited organisers / events
 - Manage multiple organisers 
 - Real-time event statistics
 - Customizable event pages
 - Multiple currency support
 - Quick and easy checkout process
 - Customizable tickets - with QR codes, organiser logos etc.
 - Fully brandable - Have your own logos on tickets etc.
 - Affiliate tracking
    - track sales volume / number of visits generated etc.
 - Widget support - embed ticket selling widget into existing websites / WordPress blogs
 - Social sharing 
 - Support multiple payment gateways - Stripe, PayPal & Coinbase so far, with more being added
 - Support for offline payments
 - Refund payments - partial refund & full refunds
 - Ability to add service charge to tickets
 - Messaging - eg. Email all attendees with X ticket
 - Public event listings page for organisers
 - Ability to ask custom questions during checkout
 - Browser based QR code scanner for door management
    
Roadmap
---
 - Theme support
 - Plugin Support
 - Localisation 
 - Increased test coverage
 - Laravel 5.4
 - IOS/Android check-in / door management apps
 - Coupon/discount code support
 - Support for more payment providers
 - WordPress Plug-in 


Contribution
---

Feel free to fork and contribute. I could use the help!

Docker dev environment
---

To run a docker dev entionment do the following:

```
git clone https://github.com/Attendize/Attendize
cd Attendize
cp .env.example .env
chmod -R a+w storage
chmod -R a+w public/user_content
docker-compose build
docker run --rm -v $(pwd):/app composer/composer install
docker-compose up -d
docker-compose run php php artisan attendize:install
```

Attendize will be available at `http://localhost:8080` and maildev at `http://localhost:1080`


