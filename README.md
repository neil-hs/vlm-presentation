# CollectionBuilder-CSV

CollectionBuilder-CSV is a robust and flexible "stand alone" template for creating digital collection and exhibit websites using Jekyll and a metadata CSV.
Driven by your collection metadata, the template generates engaging visualizations to browse and explore your objects.
The resulting static site can be hosted on any basic web server (or built automatically using GitHub Actions).

Visit the [CollectionBuilder Docs](https://collectionbuilder.github.io/cb-docs/) for step-by-step details for getting started and building collections!

## Brief Overview of Building a Collection

The [CollectionBuilder Docs](https://collectionbuilder.github.io/cb-docs/) contain detailed information about building a collection from start to finish--including installing software, using Git/GitHub, preparing digital objects, and formatting metadata.
However, here is a super quick overview of the process:

- Make your own copy of this template repository by clicking the green "Use this Template" button on GitHub (see [repository set up docs](https://collectionbuilder.github.io/cb-docs/docs/repository/)). This copy of the template is the starting point for your "project repository", i.e. the source code for your digital collection site!
- Prepare your collection metadata following the CB-CSV template (see our demo [metadata template on Google Sheets](https://docs.google.com/spreadsheets/d/1nN_k4JQB4LJraIzns7WcM3OXK-xxGMQhW1shMssflNM/edit?usp=sharing) and [metadata docs](https://collectionbuilder.github.io/cb-docs/docs/metadata/csv_metadata/)). Your metadata will include links to your digital files (images, pdfs, videos, etc) and thumbnails wherever they are hosted.
- Add your metadata as a CSV to your project repository's "_data" folder (see [upload metadata docs](https://collectionbuilder.github.io/cb-docs/docs/metadata/uploading/)).
- Edit your project's "_config.yml" with your collection information (see [site configuration docs](https://collectionbuilder.github.io/cb-docs/docs/config/)). Additional customization is done via a theme file, configuration files, CSS tweaks, and more--however, once your "_config.yml" is edited your site is ready to be previewed. 
- Generate your site using Jekyll! (see docs for how to [use Jekyll locally](https://collectionbuilder.github.io/cb-docs/docs/repository/generate/) and [deploy on the web](https://collectionbuilder.github.io/cb-docs/docs/deploy/))

Please feel free to ask questions in the main [CollectionBuilder discussion forum](https://github.com/CollectionBuilder/collectionbuilder.github.io/discussions).

----------

## Configuring a New Site from this Template

To configure a new site using this template customized for Your Company, follow these steps:

1. Edit the `_config.yml` file to set your site-specific information:
   - `url`: The full URL where your site will be hosted (e.g., https://yourcompanydomain.com)
   - `baseurl`: The path on the domain if your site is not at the root (e.g., /your-base-path)
   - `title`: The title of your site as it will appear in the banner
   - `tagline`: A short phrase or tagline for your site
   - `description`: A brief description of your collection for meta tags
   - `keywords`: Keywords describing your collection, separated by semicolons
   - `author`: The creator or organization name
   - Organization branding options such as `organization-name`, `organization-link`, and logos

2. Customize the theme settings in `_data/theme.yml`:
   - Set the `featured-image` for the home page banner (default is `/assets/img/your-company-featured-image.jpg`)
   - Adjust map settings, timeline navigation, and other visual options
   - Configure navbar colors, fonts, and icons as desired

3. Add your collection metadata CSV file to the `_data` folder and update the `metadata` field in `_config.yml` to match the filename (without the `.csv` extension). A sample metadata file `demo-compoundobjects-metadata.csv` is included as a starting point.

4. Build and serve your site locally using Jekyll commands:
   - Run `bundle install` to install dependencies
   - Use `bundle exec jekyll serve` to start a local development server

5. When ready, build the site for production with analytics and full features:
   - Use `JEKYLL_ENV=production bundle exec jekyll build` or the `rake deploy` task

This template is designed to be flexible and extensible. For detailed customization options, refer to the documentation in the `docs/` folder or visit the [CollectionBuilder Docs](https://collectionbuilder.github.io/cb-docs/).
# CollectionBuilder-CSV

CollectionBuilder-CSV is a robust and flexible "stand alone" template for creating digital collection and exhibit websites using Jekyll and a metadata CSV.
Driven by your collection metadata, the template generates engaging visualizations to browse and explore your objects.
The resulting static site can be hosted on any basic web server (or built automatically using GitHub Actions).

Visit the [CollectionBuilder Docs](https://collectionbuilder.github.io/cb-docs/) for step-by-step details for getting started and building collections!

## Brief Overview of Building a Collection

The [CollectionBuilder Docs](https://collectionbuilder.github.io/cb-docs/) contain detailed information about building a collection from start to finish--including installing software, using Git/GitHub, preparing digital objects, and formatting metadata.
However, here is a super quick overview of the process:

- Make your own copy of this template repository by clicking the green "Use this Template" button on GitHub (see [repository set up docs](https://collectionbuilder.github.io/cb-docs/docs/repository/)). This copy of the template is the starting point for your "project repository", i.e. the source code for your digital collection site!
- Prepare your collection metadata following the CB-CSV template (see our demo [metadata template on Google Sheets](https://docs.google.com/spreadsheets/d/1nN_k4JQB4LJraIzns7WcM3OXK-xxGMQhW1shMssflNM/edit?usp=sharing) and [metadata docs](https://collectionbuilder.github.io/cb-docs/docs/metadata/csv_metadata/)). Your metadata will include links to your digital files (images, pdfs, videos, etc) and thumbnails wherever they are hosted.
- Add your metadata as a CSV to your project repository's "_data" folder (see [upload metadata docs](https://collectionbuilder.github.io/cb-docs/docs/metadata/uploading/)).
- Edit your project's "_config.yml" with your collection information (see [site configuration docs](https://collectionbuilder.github.io/cb-docs/docs/config/)). Additional customization is done via a theme file, configuration files, CSS tweaks, and more--however, once your "_config.yml" is edited your site is ready to be previewed. 
- Generate your site using Jekyll! (see docs for how to [use Jekyll locally](https://collectionbuilder.github.io/cb-docs/docs/repository/generate/) and [deploy on the web](https://collectionbuilder.github.io/cb-docs/docs/deploy/))

Please feel free to ask questions in the main [CollectionBuilder discussion forum](https://github.com/CollectionBuilder/collectionbuilder.github.io/discussions).

----------

## CollectionBuilder 

<https://collectionbuilder.github.io/>

CollectionBuilder is a project of University of Idaho Library's [Digital Initiatives](https://www.lib.uidaho.edu/digital/) and the [Center for Digital Inquiry and Learning](https://cdil.lib.uidaho.edu) (CDIL) following the [Lib-Static](https://lib-static.github.io/) methodology. 
Powered by the open source static site generator [Jekyll](https://jekyllrb.com/) and a modern static web stack, it puts collection metadata to work building beautiful sites.

The basic theme is created using [Bootstrap](https://getbootstrap.com/).
Metadata visualizations are built using open source libraries such as [DataTables](https://datatables.net/), [Leafletjs](http://leafletjs.com/), [Spotlight gallery](https://github.com/nextapps-de/spotlight), [lazysizes](https://github.com/aFarkas/lazysizes), and [Lunr.js](https://lunrjs.com/).
Object metadata is exposed using [Schema.org](http://schema.org) and [Open Graph protocol](http://ogp.me/) standards.

Questions can be directed to **collectionbuilder.team@gmail.com**

## License

CollectionBuilder documentation and general web content is licensed [Creative Commons Attribution-ShareAlike 4.0 International](http://creativecommons.org/licenses/by-sa/4.0/). 
This license does *NOT* include any objects or images used in digital collections, which may have individually applied licenses described by a "rights" field.
CollectionBuilder code is licensed [MIT](https://github.com/CollectionBuilder/collectionbuilder-csv/blob/master/LICENSE). 
This license does not include external dependencies included in the `assets/lib` directory, which are covered by their individual licenses.
