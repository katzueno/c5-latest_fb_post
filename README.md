# Latest Facebook Page Post Display

This is an add-on for ConcreteCMS (concrete5) which displays Facebook Page's post using PHP SDK instead of Facebook's social graph plug-ins.

This add-on is for ConcreteCMS site admins

- who can tweak HTML/CSS by yourself
- who want to control the look of Facebook Page's post. Who doesn't want to use Facebook default plug-in.
- who doesn't mind of going through an extra step to create a Facebook app, secret key, and generate tokens

# How to set it up

## Create your Facebook App

As of June 2021, the steps may change.
You will need to obtain your app ID and secret key.

- Create a Facebook page or your facebook account already manage Facebook Page which properly administrative rights
- Register you as a developer at [Facebook Developer](https://developers.facebook.com/)
- Visit [Facebook Developers App](https://developers.facebook.com/apps/) page
- Click `Create App` button
    - Select `Business` type
    - Enter requireed info such as app email address, business manager account
    - Click `Create App`
    - Enter your facebook Password
- Obtain your App ID and secret
    - Go to `Setting` and then `Basic` menu
    - Obtain your App ID and secret key
- Add a Facebook user if you don't administrate the Facebook Page
    - If you don't manage Facebook Page, you have to add the Facebook page manager at least as `Test User` from `Role` menu.

This instruction may change over the course of the year. Please help submit PR to correct the step if this step is out-dated.

## Get Access Token

WIP

## Upload and install this add-on onto your concrete5 site

- (If you are getting the package directly from GitHub) Run `composer install` to obtain vendor files (Facebook SDK)
- Upload the package file onto your concrete5 site
- Install a package

## Creata a block template to match your theme

Creata a block template (custom template) to match the look of your Facebook page.

## Place a block into a area

Place a block into the area.

# Cache

## Block Cache is 300 seconds

It is **HIGHLY RECOMMENDED** to enable concrete5's block cache for production site.

If you disable block cache and getting many access, you may be blocked from Facebook.

The default block cache TTL of this block is 300 sec.

This means that your block may take up to 5 min to display the latest Facebook post.

If you enable full page cache, the block may not update the latest Facebook Post more than 5 min.

# Version history & changelog

Date | Version | Note
----|-------|------
2021/7/4 | 0.1 | Initial development version as MVP
