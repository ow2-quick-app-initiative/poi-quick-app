# _Heritage in…_ Quick App Project

The _Heritage in…_ Quick App project provides a methodology and a set of tools for towns to promote their most precious assets, enabling citizens and institutions to launch new projects focused on local art, culture, history, nature, or whatever is engaging in a place. 

> It's free, open-data, open-source, and crowdsourced

The [Comic Book Route quick app](#Examplesofimplementations) was made with following these methods and code templates in less than one hour.

<img src="https://ow2-quick-app-initiative.github.io/poi-quick-app-implementations/be/brussels/comics/images/screenshots.gif" alt="Screenshots of the Comic Book Route Quick App" title="Brussels Comic Book Route Quick App" height="500">

Learn more details about the methodology and how to use the templates in the following sections.

<!-- vscode-markdown-toc -->
* [Background](#Background)
	* [We all are proud of our heritage](#Weallareproudofourheritage)
	* [Online local heritage promotion](#Onlinelocalheritagepromotion)
* [The project](#Theproject)
* [The methodology](#Themethodology)
	* [Step 1. clone and configure the project](#Step1.cloneandconfiguretheproject)
	* [Step 2. populate the database](#Step2.populatethedatabase)
		* [How to submit new images](#Howtosubmitnewimages)
		* [How to update the database](#Howtoupdatethedatabase)
		* [Real example using Open Data and Linked Data](#RealexampleusingOpenDataandLinkedData)
	* [Step 3. publish the database](#Step3.publishthedatabase)
		* [Database and pictures on GitHub pages](#DatabaseandpicturesonGitHubpages)
		* [How to configure and handle public update proposals](#Howtoconfigureandhandlepublicupdateproposals)
	* [Step 4. customize the app](#Step4.customizetheapp)
		* [Load the project in the IDE](#LoadtheprojectintheIDE)
		* [Select a name for your app](#Selectanameforyourapp)
		* [Change the image](#Changetheimage)
		* [Localize the user interface](#Localizetheuserinterface)
	* [Step 5. run (and publish) the app](#Step5.runandpublishtheapp)
		* [Compile and run the app](#Compileandruntheapp)
        * [Generate your Progressive Web Application](#pwa)
        * [Examples of implementations](#Examplesofimplementations)

* [License](#License)
* [Privacy](#Privacy)
* [Get involved](#Getinvolved)
* [Acknowledgements](#acknowledgements)

<!-- vscode-markdown-toc-config
	numbering=false
	autoSave=true
	/vscode-markdown-toc-config -->
<!-- /vscode-markdown-toc -->

## <a name='Background'></a>Background

### <a name='Weallareproudofourheritage'></a>We all are proud of our heritage 

Every single town has its singularities (and oddities). Some might be famous for their [castles](https://iheartslovakia.com/castles-in-slovakia/), gardens, gastronomy, winemaking, or [unique museums](https://planomagazine.com/planos-past-the-cockroach-hall-of-fame-museum/). 

Old and modern towns have a fascinating history behind them. Of course, municipal libraries, newspapers, and archives hold most of the relevant information for explaining the origin and evolution of those places, but sometimes from a biased approach. 

Complementary to this, citizens can tell old stories and anecdotes that shaped the place's history. Older people might spend days digging into the details of their younghood and how things have changed. Families have ancestors' memories, supported by pictures from a more human and less academic perspective. Why not include this expert and passional knowledge to help understand the history?

### <a name='Onlinelocalheritagepromotion'></a>Online local heritage promotion

Information and communications technology is a town's ally to promote heritage resources and help citizens and visitors understand and learn about these exciting stories. Large cities with enough resources have promotional touristic resources like online and offline guides highlighting their precious assets. Also, small towns and regions may offer tourists something, but sometimes this is challenging due to the lack of skills and resources. 

Having this global challenge in mind, we have created a methodology and open source set of tools for anyone interested in revealing their hometown's most famous assets and hidden gems. Heritage could be referred not only to culture and arts but also to __agricultural traditions__, __architecture__, __natural ecosystems__, __geographical resources__, __science__, __sports__, and many other fields. You only need a list of exciting __points of interest__.

## <a name='Theproject'></a>The project

The _Heritage in…_ Quick App project is a set of tools and a methodology to generate apps and services for towns to promote their local art, culture, history, or whatever they are famous for. 

This methodology follows the following principles:

- __Open data__, making the most of public-sector information, reusing existing datasets and public resources by definition; 
- __Linked Data__, to provide context and enrich databases with high-quality external resources from expert domains that provide in-depth details; 
- __Open source__ for accountability, project replicability, and increasing innovation through the direct reuse of templates and source code;
- __Crowdsourcing__ and __community-driven__. Promoting citizen collaboration, which might help to enrich the database with their stories, also for efficient maintenance;
- __Sustainability__ based on no-cost, easy-to-configure tools, and low-code apps, where only minimum IT skills are required.

This initiative enables individuals to clone an open-source repository with all the instructions, templates, and source code needed to customize and launch their own local heritage project in a few hours. The templates are fully flexible and generic so that you might use them in any scenario, topic, and place.

You can find all the details of the _Heritage in…_ Quick App project in [its GitHub repository](https://github.com/ow2-quick-app-initiative/poi-quick-app). It comprises three main parts: the __methodology__, the __database__, and the __app__.  


## <a name='Themethodology'></a>The methodology

The methodology, based on the principles [listed above](#Theproject), can be applied to any scenario by anyone without limits. The procedure, templates, and code included in the git repository aim to develop proofs of concepts that could evolve and be promoted to production environments.

The main steps of the process are described below:

* [Step 1. clone and configure the project](#Step1.cloneandconfiguretheproject) from __GitHub__; 
* [Step 2. populate the database](#Step2.populatethedatabase), using __open data__ or other means you like;
* [Step 3. publish the database](#Step3.publishthedatabase) and set up __GitHub Pages__;
* [Step 4. customize the app](#Step4.customizetheapp), changing colors, icons, and descriptions;
* [Step 5. run (and publish) the app](#Step5.runandpublishtheapp).

<img src="https://ow2-quick-app-initiative.github.io/poi-quick-app/sample/images/methodology-all.jpg" alt="Methodology of Heritage in… Quick App project" width="100%">

### <a name='Step1.cloneandconfiguretheproject'></a>Step 1. clone and configure the project

1. Access the [git repository](https://github.com/ow2-quick-app-initiative/poi-quick-app). 
2. Fork the project into your projects (`Reuse this template`).

You might access the public database and documentation under the `/docs` directory. There, you will find the template of the database `/docs/sample/data.json`. You can rename the `sample` directory following your rules.

The application code (a quick app) is under the `/quick-app` directory.

See the complete structure of the project in the following picture.

<img src="https://ow2-quick-app-initiative.github.io/poi-quick-app/sample/images/methodology-repo.jpg" alt="File structure of the repository" height="500">


### <a name='Step2.populatethedatabase'></a>Step 2. populate the database

Note that all the documents and directories within `/docs` will be exposed and accessible from the Web. 

The database document is at `/docs/sample/data.json`.

Every project has two resource types:

- *images* (`./images/xxxxx.jpg`): light pictures in square format. If possible 1x1 ratio for a homogenous look and feel; the lighter, the better (50Kb per image would be fine).
- *database* (`./data.json`): JSON file with the app's configuration (name, colors, privacy texts, etc.) and the points of interest you want to show in the app. 

You can download it to your computer, modify the texts, or add a new element based on your knowledge. 

Once you have the final version, pull the content to the git repository (and repeat every time you want to modify the content).

You might want to introduce a moderation process for the maintenance, reviewing the pull requests and changes over the content. Also, you can use issues and comments to open the participation to users that are not familiar with GitHub.

#### <a name='Howtosubmitnewimages'></a>How to submit new images

The images are in the `./images` directory. 

You can find a mistake, or you want to modify and rewrite the file with a new version. 

If you have new images to add, just upload your new ones in the folder. 

Please, use the identifier of the point of interest you are referring to (see attribute `id` of the [Point of Interest](#points-of-interest)).


#### <a name='Howtoupdatethedatabase'></a>How to update the database

The database is in the JSON file named `data.json` (`/sample/data.json`). Initially, you have an empty file you can use to quick start the project.

Please be sure that this document has the correct format (syntax and content). You can test it locally using any JSON schema validation tool against the JSON schema you can find in the repository ([schema.json](https://ow2-quick-app-initiative.github.io/poi-quick-app/schema.json)). 

This JSON document contains two main parts, represented by the main keys of the root object:

1. `meta`: metadata about the project
2. `content`: multilingual content and setup of the application (based on localized information)

##### Metadata of the project

Example of a project named `fr/paris` for the City of Paris: 

```js
{
    "meta": {
        "app_id": "org.example.paris",        
        "app_title": "Paris Street Heritage",
        "version": 12,
        "updated": "2022-10-26",
        "source_url": "https://ow2-quick-app-initiative.github.io/poi-quick-app/fr/paris/data.json",
        "matomo_base_url": "https://example.org/my-matomo-instance?id=1",                
        "marketplace_url": "https://appgallery.huawei.com/app/FinalURL"
    },
    "content": {
        "en": {},
        "fr": {},
        "es": {}
    }    
}
```

- `app_id` (`string`) The package identifier as specified in the `manifest.json` document.
- `app_title` (`string`) The title to identify the application.
- `version` (`integer`) The non-negative integer that represents the version of this document (this will be used by the app to find the latest version).
- `updated` (`date`) The date in ISO 8601 format (`YYYY-MM-DD`) when this document was last updated. 
- `source_url` (`URL`) The URI of this document on the Web (once it´s published).  
- `matomo_base_url` (`URL`) The base URI for a [Matomo analytics](https://en.wikipedia.org/wiki/Matomo_(software)) instance (empty if you don't want it).
- `marketplace_url` (`URI`) The URI to the application if it is listed in a marketplace (e.g, URL to the AppGallery)

##### Content of the project

Following the example of the City of Paris, we can __localize the content into any language__, using the [ISO 639-1](https://www.loc.gov/standards/iso639-2/php/English_list.php) codes (assigning a two-letter code for the language). You can also specify the concrete region (using a `-` character and the concrete [ISO 3166-1](https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes) (Alpha-2 code). 

``` json
{
    "meta": {},
    "content": {
        "en_GB": {},
        "en_US": {},
        "fr": {},
        "es": {}
    }
}
```

The project must contain at least one language tag (e.g., `en`). 

Every key of the `content` object is a language tag that must contain JSON objects with the same keys but with different translations and content localized according to the language.

The content language tags are objects with the following structure:

```js
{
    "meta": {},
    "content": {
        "LANG": {
            "app": {},      // App configuration (color, texts)
            "pois": []      // Points of Interest
        }
    }
}
```

- `app` is an object that contains general information to configure the application for this language.
- `pois` is an array of objects with points of interest or database items. 


```js
{
    "meta": {},
    "content": {
        "en": {
            "app": {
                "theme": {
                    "brand": "#B11623",             // Main color of the theme
                    "complementary": "#FAFAFA"      // Secondary color of the theme
                },
                "repository_url": "https://github.com/ow2-quick-app-initiative/poi-quick-app/",
                "text_info": "This project was created by...",
                "text_acknowledge": "We would like to thanks...",
                "text_feedback": "Please let us know if you want to contribute...",
                "feedback_url": "https://ow2-quick-app-initiative.github.io/poi-quick-app/fr/paris/#contributors",
                "issue_url": "https://github.com/ow2-quick-app-initiative/poi-quick-app/issues/new?labels=fr/paris"
            },
            "pois": [
                {
                    "id": "eiffeltower",
                    "lat": "48.865157817905896",
                    "lon": "2.2938185078918156",
                    "type": "tower",
                    "name": "Eiffel Tower",
                    "images": [
                        "https://ow2-quick-app-initiative.github.io/poi-quick-app/fr/paris/images/eiffeltower_1.jpg",
                        "https://ow2-quick-app-initiative.github.io/poi-quick-app/fr/paris/images/eiffeltower_2.jpg"
                    ],
                    "description": "The Tour Eiffel (French) is a iron lattice tower, named after the engineer Gustave Eiffel, whose company designed and built the tower",
                    "more": "Locally nicknamed La dame de fer (French for Iron Lady), it was constructed from 1887 to 1889 as the centerpiece of the 1889 World's Fair and was initially criticized by some of France's leading artists and intellectuals for its design, but it has become a global cultural icon of France and one of the most recognizable structures in the world",
                    "attributions": [
                        "John Smith", 
                        "Jane Doe Inc."
                    ], 
                    "urls": [
                        "https://en.wikipedia.org/wiki/Eiffel_Tower"
                    ]
                },
                {
                    // Other PoI...
                }
            ]
        }
    }
}
```

###### App configuration

The app can be configured with localized texts, URLs, and themes, depending on the user's locale. Each language tag in the `content` member has an object to configure and customize the application (`app` key). You can customize it through the following members:

- `theme` (`object`) The main look-and-feel colors:  
  - `brand` (`string`) The primary color in HEX format (e.g., `#B11623`)
  - `complementary` (`string`) The secondary color in HEX format (e.g., `#FAFAFA`)
- `repository_url` (`url`) The URL to the repository where the project is hosted (where this database is maintained).
- `text_info` (`string`) Text to explain the project. It will be shown in the _about_ section.
- `text_acknowledge` (`string`) Text with acknowledgements about the project. It will be shown in the _about_ section.
- `text_feedback` (`string`) Text with information explaining how to contribute with the project. It will be shown in the _about_ section.
- `feedback_url` (`url`) A URL linking to a page where the contributors can get involved. It will be shown in the _about_ section.
- `issue_url` (`url`) A URL with customized parameters in the querystring that will be used to report individual issues on specific items. It will be linked to the individual items. See [How to configure and handle public update proposals](#Howtoconfigureandhandlepublicupdateproposals) for more details.


###### Points of Interest

The PoIs are the main items of the database, described in the `poi` attribute as an array of objects with the following members: 

- `id` (`string`) Unique identifier for the item (e.g., `eiffeltower`).
- `name` (`string`) Short text with the title of the point of interest (e.g., `Eiffel Tower`).
- `lat` (`string`) Latitude component of the item coordinates in WGS84 format (e.g.,`48.8651`).
- `lon` (`string`) Longitude component of the item coordinates in WGS84 format (e.g.,`2.2909`).
- `type` (`string`) Short text with the type of the item, according to your own taxonomy (e.g.,`sculpture`, `painting`,...).
- `images` (`array` of `url`) One or more absolute URLs with pictures about the item. These images could be external, but it is recommended to host them under the same repository as the database. See [How to submit new images](#how-to-submit-new-images) for more details.
- `description` (`string`) One paragraph text with a concise description of the item.
- `more` (`string`) Extended text with more details of the item.
- `urls` (`array` of `url`) One or more absolute URLs to external related resources (e.g., to Wikipedia, official sources, etc.).
- `attributions` (`array` of `string`). List of texts with the names of the contributors to the content or images of this item, if any.


#### <a name='RealexampleusingOpenDataandLinkedData'></a>Real example using Open Data and Linked Data

The [Brussels Comic Book Route Quick App](https://github.com/ow2-quick-app-initiative/poi-quick-app-implementations/tree/main/quick-app/be/brussels/comics) was made through this methodology and templates. The database is based on a dataset by the [BXL Open Data](https://opendata.brussels.be/page/home/) initiative.

The data, almost perfect and distributed in Comma Separated Value (CSV) format, was curated using [OpenRefine](https://openrefine.org/). Subsequently, the database was enriched with external sources like [Wikidata](https://www.wikidata.org/wiki/Wikidata:Main_Page) through __linked data__.  

This is just an example, but it shows how powerful and productive these tools may be for simple projects.  

Read the illustrative [step-by-step guide on how the Brussels Comic Book Route project was created](https://ow2-quick-app-initiative.github.io/poi-quick-app-implementations/be/brussels/comics/step_by_step_development_guide.pdf).

### <a name='Step3.publishthedatabase'></a>Step 3. publish the database

#### <a name='DatabaseandpicturesonGitHubpages'></a>Database and pictures on GitHub pages

The project's content (i.e., general information, database, and images) is served from an HTTP server using GitHub pages. The application will check if the internal version of the database is older than the version published on the Web. Thus, all the updates on the database must be made in the public git repository to keep an up-to-date version available from the applications that will visualize the content. 

In concrete, Github Pages must be configured using a custom Continuous Integration (CI) action (included in the repository) to publish the `./doc` directory of the principal repository into the `gh-pages` repository branch.

This method uses GitHub Pages (i.e., the content of the root directory in the `gh-pages` branch) to serve the latest valid version of the content (i.e., database and images). 

An intermediate CI action validates the format of the data.json document. The validation is performed against a JSON schema included in the repository. If the latest version of the database pushed to the repository is not valid, the deployment of the new version is halted, keeping the previous version. This action prevents mistakes and avoids corrupt databases causing failures in the app.

##### Activate GitHub Pages

The open source project includes the CI actions. Once you have access to these CI actions, you only need to configure the project with the following steps:

1. Create a gh-pages branch that will be used to publish the content. 
2. Create a personal token 
  a) (`Profile` > `Settings` > `Developer Settings` > `Personal access tokens`)
  b) `Generate new token` > Add a name + [no expiration] + check “repo” in the scope > `Generate token`
  c) Copy the token generated in the clipboard
3. Create a secret with your token
  a) `Project’s Settings` > `(Security) Secrets` > `Actions`
  b) New repository secret with 
    - Name:  `ACCESS_TOKEN`
    - Value: the token (in your clipboard)
4. You can verify that the CI Action works properly (`Project's Actions`) and re-run the jobs with failure (after that, they must be in green)
5. In project's `Settings` > `Pages` you can see the public URL of your site with the template of the documentation. 

<img src="https://ow2-quick-app-initiative.github.io/poi-quick-app/sample/images/methodology-ci.jpg" alt="Summary of the workflow of the CI actions" width="70%">

#### <a name='Howtoconfigureandhandlepublicupdateproposals'></a>How to configure and handle public update proposals 

User's feedback is handled through GitHub issues guaranteeing transparent communication and proper attribution. Issues might be classified using tags to indicate the project to which they belong. 

The title of the issues should contain the same name or identifier of the point of interest to avoid misunderstandings.   

You also can create an issue template to have a homogeneous format (see [.github/ISSUE_TEMPLATE/update_request.md](https://github.com/ow2-quick-app-initiative/poi-quick-app/tree/main/.github/ISSUE_TEMPLATE/update_request.md)) and use it for new issues. 

In the [app configuration](#app-configuration), we configure the template URL for the issues for the project. If you want to handle issues by language, you can specify different tags or templates according to your needs. 

For instance:

```js
{
    //...
    "issue_url": "https://github.com/ow2-quick-app-initiative/poi-quick-app/issues/new?labels=uk/london&template=update_request.md&title=Update+request+of+"
    //...
}
```

Note that the application will append the name of the point of interest at the end of the URL, so the GitHub issue will contain the full name of the point of interest in the title.


### <a name='Step4.customizetheapp'></a>Step 4. customize the app

The final outcome is an app, implemented as a [Quick App for Android](https://quick-app-initiative.ow2.io/editorials/2022-06-23-what-is-a-quick-app/), with a service for locals and tourists, with basic and intuitive functionality. The app uses contextual information collected by the device, like the precise user's location, and serves the data and images through an appealing and straightforward user interface.

The `/quick-app` directory contains the code of the quick app.

Feel free to tweak the code of the quick app (see the [developer´s documentation](https://quick-app-initiative.ow2.io/developers/)), but the application is ready to run, so you only need to configure it:

#### <a name='LoadtheprojectintheIDE'></a>Load the project in the IDE

Load the quick app project (`/quick-app/src/`) in your favorite editor ([Huawei Quick App IDE](https://developer.huawei.com/consumer/en/quickApp-ide), [Generic Quick App IDE](https://www.quickapp.cn/docCenter/IDEPublicity)).


#### <a name='Selectanameforyourapp'></a>Select a name for your app

Choose a name for your app and change it in the `.manifest.json`´s `name` member.

Example of manifest by default:

```js
{
    "package": "org.example.myquickapp",
    "name": "City Street Heritage",  // <-- The name of the app
    "versionName": "0.1",
    "versionCode": 1,
    "minPlatformVersion": 1078,
    "icon": "/common/images/logo.png",
    // ...
}
```    

Read more details [about the Quick App manifest](https://quick-app-initiative.ow2.io/developers/guide/manifest.html).


#### <a name='Changetheimage'></a>Change the image 

Rewrite the app´s main logo and the icon with your own images.

Just overwrite `/common/images/logo.png` (flexible dimensions) and `/common/images/logo-216.png` (216 x 216px)

#### Load the database 

Overwrite the first version of the database generated in [step 2](#Step2.populatethedatabase) over `/common/json/data.json`.

This database file will be used in case the app is offline.

<img src="https://ow2-quick-app-initiative.github.io/poi-quick-app/sample/images/methodology-app-maintenance.jpg" alt="How the app works in summary" width="70%">

#### <a name='Localizetheuserinterface'></a>Localize the user interface

The application offers a multilingual user interface and content adapted to the requirements of the specific implementations. The internationalization resources are decoupled from the app logic to facilitate the localization of resources into additional languages.

Internationalization string resources are in the `/quick-app/src/i18n/` directory and they are named using the [ISO 639-1](https://www.loc.gov/standards/iso639-2/php/English_list.php) codes (assigning a two-letter code for the language). You can also specify the concrete region (using a `-` character and the concrete [ISO 3166-1](https://en.wikipedia.org/wiki/List_of_ISO_3166_country_codes) (Alpha-2 code) plus the `.json` extension.


Example of the `en.json` document:

```js
{
    "message": {
        "app": {
            "geolocation" : {
                "request" : "I need geolocation to work",
                "description": "This app uses your geolocation to show the artworks nearby, nothing else. Please grant it :)",
                "no": "No, thanks",
                "yes": "Yes, I'm okay"
            }
        },
        "tabs": [
            {
                "title": "Cards",
                "icon": "\ue3b6"
            },
        // ...
```

### <a name='Step5.runandpublishtheapp'></a>Step 5. run (and publish) the app

#### <a name='Compileandruntheapp'></a>Compile and run the app

1) Install the dependencies

The app requires the external `geolib` library for geographic functions (e.g., `getDistance(from, to)`)

Other libraries may be added to the `package.json` document in the root directory.

```bash
npm install
```

2) Test the app within the IDE

You also can generate the RPK app package and distribute it where you want.

If you want to promote the app, you can publish the quick app in [AppGallery](https://developer.huawei.com/consumer/en/service/josp/agc/index.html#/) or other marketplaces.

#### <a name='pwa'></a>Generate your Progressive Web Application

Alternatively, you can try the database generated on the Web. We have developed a simple web application, [heritagein.info](http://heritagein.info), that uses that database (`data.json`) to display and interact with it. The Web version has similar functionalities to the quick app, available on any web browser. 

In reality, [heritagein.info](http://heritagein.info) is a __meta app__ that enables us to generate unlimited _heritage in..._ apps just passing a parameter with the URL to your `data.json`. 

For instance, we can visualize the places in the database generated for the Brussels Comic Book Route ( 
`https://ow2-quick-app-initiative.github.io/poi-quick-app-implementations/be/brussels/comics/data.json`), including the URL in the query string as follows.

```
https://heritagein.info/_/?url=https://ow2-quick-app-initiative.github.io/poi-quick-app-implementations/be/brussels/comics/data.json
``` 

Just change the `url`parameter to test your outcomes. Visit the home page and find some existing implementations that follow this methodology. 

##### How to generate a new PWA?

We maintain a public [configuration file](https://github.com/ow2-quick-app-initiative/poi-quick-app/blob/main/docs/implementations.json), which the application uses to generate the concrete instances for each configuration file. Each instance listed in this document is a Progressive Web Application. The system generates dedicated [manifest.json](https://developer.mozilla.org/en-US/docs/Web/Manifest) for each of them. 

This implementations.json document includes a `towns` array with objects that will identify every implementation. For instance:
  
```js
"towns" : [
         // ...,
	 { 
	 "name": "Paris Cultural Heritage",
	 "id": "paris",
	 "location": "Paris (🇫🇷)",
	 "source_url": "https://github.io/cultural-quick-app/fr/paris/data.json",
	 "country": "France",
	 "lang": [ "en", "fr", "es" ]
	 },
```

The meta app will generate a new instance for you under the path indicated by the `id` member. So, we will have a nicer URL (i.e., `heritagein.info/paris/`). 

The heritagein.info app implements [language negotiation](https://www.w3.org/International/questions/qa-when-lang-neg), but you can force the locale, including it as a parameter in the path of the URL, just after the id of the implementation (e.g., `heritagein.info/paris/fr/` for French or `heritagein.info/paris/en/` for English). If no content or UI elements are localized to this language, the system will return `en`(English) by default or the first locale found in the database. 

#### <a name='Examplesofimplementations'></a>Examples of implementations

* [Leuven Cultural Heritage](https://ow2-quick-app-initiative.github.io/poi-quick-app-implementations/be/leuven/heritage/). Historical places and monuments in Leuven 🇧🇪. [See result](https://heritagein.info/leuven/).
* [Oeratoom](https://ow2-quick-app-initiative.github.io/poi-quick-app-implementations/be/leuven/oeratoom/). Big Bang Theory artwork in Leuven (🇧🇪). [See result](https://heritagein.info/oeratoom/).
* [Comic Book Route](https://ow2-quick-app-initiative.github.io/poi-quick-app-implementations/be/brussels/comics//). Wall paintings in Brussels (🇧🇪). [See result](https://heritagein.info/comics/).
* [Middelheim Museum](https://ow2-quick-app-initiative.github.io/poi-quick-app-implementations/be/antwerpen/middelheimmuseum/data.json). Open-air musseum in Antwerpen (🇩🇪). [See result](https://heritagein.info/middelheim/).
* [Eckernförde Heritage](https://ow2-quick-app-initiative.github.io/poi-quick-app-implementations/de/eckernforde/). Historical buildings in Eckernförde 🇩🇪. [See result](https://heritagein.info/eckernforde/).

Share yours! We are collecting all [the existing implementations in machine-readable format](https://github.com/ow2-quick-app-initiative/poi-quick-app/blob/main/docs/implementations.json). This will help the tools to produce new Web applications based on your database. 

Just update the file or [send us the information](https://github.com/ow2-quick-app-initiative/poi-quick-app/issues/new) about what you have done.

## <a name='License'></a>License

This project's documentation, content, and data folders are licensed under a [CC-BY license](https://github.com/ow2-quick-app-initiative/poi-quick-app/blob/main/LICENSE).

All other code in this repository is licensed under the [MIT license](https://github.com/ow2-quick-app-initiative/poi-quick-app/blob/main/LICENSE-CODE).

## <a name='Privacy'></a>Privacy

These apps are based on open data and automatic processing of the data. The community's content is enriched and curated, so it's available to anyone who wants to get involved. Local experts are welcome to refine the definitions, names, and pictures and add new points of interest to the app.

The app doesn't collect any personal data. The quick app may perform a call to a [Matomo instance](https://en.wikipedia.org/wiki/Matomo_(software)) to measure its performance, but no personal data is shared. You can just [check the code](https://github.com/ow2-quick-app-initiative/poi-quick-app/blob/0e30a81f203796156ecb29b30437fb18f9f83309/quick-app/src/app.ux#L222) that generates a random identifier.  

## <a name='Getinvolved'></a>Get involved

> Do you want to improve the content, translations or enhance the original code? 

This project aims to be as much collaborative as possible, so we will be pleased to have you onboard. You can contribute in many ways:

- Translate the user interface of the apps (or enhance the existing automatic translations);
- Improve the quality of the databases for specific implementations;
- Create your own project for your own purposes (even you can sell it);
- Enhance the quality of the code (we are aware there is room for improvement... a lot);
- Submit new pictures or more points of interest...

If you are familiar with Github, just fork the repository and push your contributions. 

The code of the quick app is in the [`/quick-app`](https://github.com/ow2-quick-app-initiative/poi-quick-app/tree/main/quick-app) folder of the repository. The web application is in the [poi-quick-app-web repository](https://github.com/ow2-quick-app-initiative/poi-quick-app-web/).

If you don´t know how to start, please login to Github and [raise an issue with your intentions and suggestions](https://github.com/ow2-quick-app-initiative/poi-quick-app/issues/new).

Thank you!

## Acknowledgements

Pictograms used in the images:

- Cloud by Aya Sofya from NounProject.com
- App by Adrien Coquet from NounProject.com
- Folder by HideMaru from NounProject.com
- Jpg by Ilham Fitrotul Hayat from NounProject.com
- Json by Md Moniruzzaman from NounProject.com
- Csv by Ilham Fitrotul Hayat from NounProject.com
- User by Benny Chaw from NounProject.com
- Terminal by Hare Krishna from NounProject.com