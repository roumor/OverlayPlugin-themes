#OverlayPlugin Themes

## Updated for 4.0 Stormblood
#### Please be patient as we go through and update the overlays. Some overlays may be discontinued as their contribers may not be playing the game anymore. If you have a particular overlay you would like to see updated let us now. 

## Moving to Cloud Hosted Overlways

We are in the process of moving all of these overlays to be hosted so that users can always have hte most recent version of the overlways without the hastle of downloading new files every time. 

This will mean that any customization that you have made to downloaded plugins themes will no longer work as you will be using the most recent version directly from this repo. 

For now. `http://ffxiv.evileeyore.com` will be hosting the files in teh exact format as this repo.

For now to Load RDMTY set your URL in Overlayplugin to: `http://ffxiv.evileeyore.com/rdmty_default.html`

this might change in the future to use folders instead of direct html file locations. IE: `http://ffxiv.evileeyore.com/rdmty/`


## Usage
`git clone` or download the ZIP package to a directory (i.e. your ACT directory)

In ACT -> Plugins -> OverlayPlugin.dll settings, for URL, browse to the folder where you extracted the ZIP and then select the HTML file of your choice.

## Screenshots
### rdmty_default.html
### Requires OverlayPlugin >= 0.3.3.3!!
* Collapse/expand detailed statistics for the encounter
* Switch between DPS, Healer, or Tanking views
![rdmty features](/screenshots/rdmty_explanation.png?raw=true "rdmty
features")
![rdmty Healing](/screenshots/rdmty_healing.png?raw=true "rdmty
Healing")
![rdmty Tanking](/screenshots/rdmty_tanking.png?raw=true "rdmty
Tanking")

### rdmty_no_job_colors.html
![rdmty with single color for bars](/screenshots/rdmty_no_job_colors.png?raw=true "rdmty with single color for bars")

### kyitrai
![kyitrai](/screenshots/kyitrai.png?raw=true "kyitrai")

### Immutable
![Immutable](/screenshots/immutable.png?raw=true "Immutable")

### xephero.html
![xephero](/screenshots/xephero.png?raw=true "xephero")

### elizar2006
![elizar2006](/screenshots/elizar2006_miniparse.jpg?raw=true "elizar2006")

### momokotomoko
![momokotomoko](/screenshots/momokotomoko_miniparse.jpg?raw=true "momokotomoko")

### tristoune
![tristoune](/screenshots/tristoune_miniparse.jpg?raw=true "tristoune")

### Vertigo
![miniparseVertigo](/screenshots/miniparseVertigo.jpg?raw=true "miniparseVertigo")

## Contributing Your Own Layouts

### Naming
Give your `HTML` files a descriptive name, i.e. **your tag**_**description**.html
Use a single CSS and JS file for all of your similar themes.
* `CSS` - **your tag**.css
* `JS` - **your tag**.js


### Future
In order to make it easier to maintain, as well as customize, let's try to standardize the layouts.
Let's split the HTML file into separate CSS and JS files (use `rdmty_compact_dps.html` as an example for now).  

In In the future, `React` will probably be dropped in favor of something a bit more familiar (probably just templates using `handlebars`). However if you are going to be using a framework please inlcude your source files so we can help contribute to keeping the files up to date. IE: .jsx files. 

If you want to build a bit complexity and want more than 1 app js file please create a folder for yourself under app/YOUR_OVERLAY/ This will help keep the repo as clean as possible. 

### Directory Structure
* `app` - Your JS application files (not third party libraries)
* `css` - CSS files
* `images` - Any image resources should be put in here
* `lib` - JS library files

The user currently has only one interface to customize the layout from ACT (without modifying any files): selecting the HTML file.  Make the HTML file as descriptive as possible and try to not modify much code in the HTML file (besides customization variables and CSS/JS file names).  This way, if we were to get support for more customization options in ACT plugin, it would be easier to modify the themes for this.
