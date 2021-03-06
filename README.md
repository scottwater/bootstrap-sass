# Bootstrap for Rails

`bootstrap-sass` is an SASS-powered version of [Twitter's Bootstrap](http://github.com/twitter/bootstrap), ready to drop right into your asset-pipeline powered Rails applications.

Enjoy.

## Usage

In your gemfile:

    gem 'bootstrap-sass', '~> 1.4.4'

### CSS

In your SCSS file of choice:

    @import "bootstrap"; /* Use this to get all of Bootstrap's @mixins and $variables */

Want to configure a variable? Thanks to bernado, this is now awesome *and* easy! Just define the variables you want to change *before* importing Bootstrap. SASS will respect your existing definition and won't overwrite it with the Bootstrap defaults.

    $gridColumns: 12;
    $gridColumnWidth: 60px;
    $gridGutterWidth: 20px;
    @import "bootstrap";

### Javascript

In your Javascript manifest:

    // Loads all Bootstrap javascripts
    //= require bootstrap
    
    // Alternatively, you can load individual modules
    //= require bootstrap-scrollspy
    //= require bootstrap-modal
    //= require bootstrap-dropdown

Simples.

## Versioning
We try to stick to Bootstrap versioning wherever possible. The major and minor version numbers will always represent the Twitter Bootstrap version, but no guarantees are made for the tiny version number, since waiting for Bootstrap to update so I can push out a fix sucks.

## Branches
Master will usually represent the latest release of `bootstrap-sass`. Other branches contain experimental code, or are a relatively close mirror of other Bootstrap branches.

