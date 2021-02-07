+++

title = "Code Toggle" 
description = "Code Toggle tryout and showcase.." 
tags = [ "go", "golang", "hugo", "development", ] 
date = "2014-04-02" 
menu = "main" 

+++

## The Config Toggler! 

This is an example for the Config Toggle shortcode. Its purpose is to let users choose a Config language by clicking on its corresponding tab. Upon doing so, every Code toggler on the page will be switched to the target language. Also, target language will be saved in user’s localStorage so when they go to a different pages, Code Toggler display their last “toggled” config language.



>The code-toggler shortcode is not an internal Hugo shortcode. This page’s purpose is to test out a custom feature that we use throughout this site. See: https://github.com/gohugoio/gohugoioTheme/blob/master/layouts/shortcodes/code-toggle.html
>



That Config Toggler 


```toml
baseURL = "https://yoursite.example.com/"
footnoteReturnLinkContents = "↩"
title = "My Hugo Site"

[params]
  AuthorName = "Jon Doe"
  GitHubUser = "spf13"
  ListOfFoo = ["foo1", "foo2"]
  SidebarRecentLimit = 5
  Subtitle = "Hugo is Absurdly Fast!"

[permalinks]
  posts = "/:year/:month/:title/"
```



## Another Config Toggler! 

```json
{
   "author": {
      "homepage": "https://github.com/budparr",
      "name": "Bud Parr"
   },
   "description": "",
   "features": [
      "",
      ""
   ],
   "homepage": "https://github.com/budparr/gohugo.io",
   "license": "MIT",
   "licenselink": "https://github.com/budparr/gohugo.io/blob/master/LICENSE.md",
   "min_version": 0.18,
   "name": "Hugo Theme",
   "tags": [
      "website"
   ]
}
```

