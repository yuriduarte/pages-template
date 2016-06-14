# Pages::Rails

Welcome to Rails Pages Gem. The following will not install all thirdpary dependencies used in the demo. It has to be installed later manually.

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'pages-rails','2.1.4',:git => 'https://github.com/revoxltd/pages-rails.git'
```

Install from branch/tag/release
```
gem 'pages-rails', :git => "https://github.com/revoxltd/pages-rails.git", :ref => "4aded"
gem 'pages-rails', :git => "https://github.com/revoxltd/pages-rails.git", :branch => "2-3-stable"
gem 'pages-rails', :git => "https://github.com/revoxltd/pages-rails.git", :tag => "v2.3.5"
```
And then execute:

    $ bundle

Or install it yourself as:

    $ gem install pages-rails

## Usage
1. Add to your application.js
Will Include core pages.js
```
//= require pages
```

Adding other components like calendar,email etc
```
//= require pages.calendar
//= require pages.email
//= require pages.social
```

2. Add to your application.css
```
*= require pages
```

 or include rtl version
```
*= require pages.rtl
```

Include theme (dont include with pages.rtl or pages, only include the following)
```
 *= require themes/abstract
 ```

##Dependencies

| Plugin | Description | Dep. Status |
| -- | -- | -- |
| jquery.js | Core JS Library | **REQUIRED** |
| mordnerizer.js | Browser Feature Detection | **REQUIRED** |
|bootstrap.js| Core Framework | **REQUIRED**
|jquery-easy.js| Used for animations in IE | **OPTIONAL**
|pace.js| Page Progress Loader | **OPTIONAL**
|jquery-unviel.js|Library Used for displaying retina images|**OPTIONAL**|
|jquery-bez.js|Sidebar Animation Lib for IE9|**OPTIONAL**|
|jquery.ioslist.js| Used Chat list on the quickview| **OPTIONAL**|
|jquery.actual.js|Determine image dimentions| **OPTIONAL**|
|jquery.scrollbar.js|Scrollbar plugin used in sidebar and portlets|**OPTIONAL**|