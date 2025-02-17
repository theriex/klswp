# klswp

Visible pages and supporting files from wp site.  Static site issues:
  - index.html renders reasonably well, but the nav bar links don't work.
    You have to open eaach index.html file from the corresponding folder to
    see that page.
  - Some images are not rendered.  Inspecting the element source shows the
    img html, and the src file for the image was pulled down.  The rendering
    fail seems to to be due to wp image preload css errors that fail when
    viewing outside the wp server environment.
  - The box bullet images on the research page are css animations that do
    not render outside the wp server environment, and are not based on any
    image references in the html.  These would need to be recreated if the
    site was rebuilt from scratch.
  - Some of the formatting is a bit skewed because it relies on animation
    effects not incorporated into the static pages.

Should be enough to reconstruct the content for the site.
