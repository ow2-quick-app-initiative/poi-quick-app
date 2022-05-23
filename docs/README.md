# Local Cultural Heritage Quick App

The Local Cultural Heritage Quick App promotes cultural heritage collections in small and medium cities through open data and crowdsourcing. 

> It's free, open-source, and collaborative 

Any city can implement its own application in a few hours. They only need one or more experts to feed the first version of the database.   
Currently, we have the following proofs of concept:

- [Leuven (Belgium)](https://pbesteu.github.io/cultural-heritage-quick-app/be/leuven) 
- [Eckernförde (Germany)](https://pbesteu.github.io/cultural-heritage-quick-app/de/eckernforde) 

Some screenshots:

<img src="https://pbest.eu/cultural-heritage-quick-app/be/leuven/images/screenshots.png" alt="Screenshots of the Leuven application" width="100%">

## Start a new project for your town

If you want to start a new project, you only need to:

- configure the [quick app](https://github.com/pbesteu/poi-quick-app/tree/main/quick-app) of this repository, and
- configure the sample [database and documentation](https://github.com/pbesteu/poi-quick-app/tree/main/docs/sample) that feeds the quick app.

## License

This project's documentation, content, and data folders are licensed under a [CC-BY license](./LICENSE).

All other code in this repository is licensed under the [MIT license](./LICENSE-CODE).

## Privacy

These apps are based on open data and automatic processing of the data. The community's content is enriched and curated, so it's available to anyone who wants to get involved. Local experts are welcome to refine the definitions, names, and pictures and add new points of interest to the app.

The app doesn't collect any personal data, so relax. We won't sell anything.

The quick app may perform a call to a [Matomo instance](https://en.wikipedia.org/wiki/Matomo_(software)) to measure its performance, but no personal data is shared. You can just [check the code](https://github.com/pbesteu/poi-quick-app/blob/0e30a81f203796156ecb29b30437fb18f9f83309/quick-app/src/app.ux#L222) that generates a random identifier.  

## Developers

> Do you want to contribute to the code?

Just fork the repository and start sending your contributions. The code of the quick app is in the [`/quick-app`](https://github.com/pbesteu/poi-quick-app/tree/main/quick-app) folder of the repository. 

Feel free to [raise issues](https://github.com/pbesteu/poi-quick-app/issues/new) on the code.


## Acknowledgments

- Banner picture by [Kasturi Roy on Unsplash](https://unsplash.com/photos/WLlupsRhjyw).