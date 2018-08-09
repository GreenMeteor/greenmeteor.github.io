# Customizing Themes

### Custom Email Colors

#### Quick How To for Custom color email

- Step 1: Make sure to have a `variables.less` within your `less` folder.
- Step 2: Take the code from the [`humhub/static/less/variables.less`](https://github.com/humhub/humhub/blob/master/static/less/variables.less) and add it to `/YOUR-THEME/less/variables.less`.
- Step 3: Edit the color code you want everything to be then you're done.
- Step 4: Finally make sure that you clear your site's cache in `ACP -> Settings -> Advanced -> Cache`

### Removing "Powered by"

#### Email
For email layout copy the whole  mail folder from [`/protected/humhub/views/mail`](https://github.com/humhub/humhub/tree/master/protected/humhub/views/mail) and on [line 699](https://github.com/humhub/humhub/blob/master/protected/humhub/views/mail/layouts/html.php#L699) remove what you're looking for (Note : You'll have to remove it from [line 10](https://github.com/humhub/humhub/blob/master/protected/humhub/views/mail/layouts/text.php#L10) in `text.php` as well) Once you done this please move the whole folder into `/YOUR-HUMHUB/themes/YOURTHEME/views`

#### Login/Sign Up
For this you do the same thing you did above, copy [`/protected/humhub/modules/user/views/layouts`](https://github.com/humhub/humhub/blob/master/protected/humhub/modules/user/views/layouts/main.php) (The whole folder!) edit and remove [line 27](https://github.com/humhub/humhub/blob/master/protected/humhub/modules/user/views/layouts/main.php#L27), once that is done place the whole user folder into `/YOUR-HUMHUB/themes/YOURTHEME/views`

> Note: More will be added if asked.
