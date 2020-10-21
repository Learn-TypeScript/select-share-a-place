[Understanding TypeScript - 2020 Edition](https://www.udemy.com/course/understanding-typescript/)

Don't limit the Usage of TypeScript to Angular! Learn the Basics, its Features, Workflows and how to use it!

Created by Maximilian Schwarzmüller

- This is the continue of the `drug-n-drop` repo.

Take care of billing account in Google Cloud Platform, after finishing this app.

### Notes:

13. **Time to Practice! Let's build a "Select & Share a Place" App (incl. Google Maps)**

- rm -rf .git => to remove the version control we downloaded.

* (170). Setting Up a Google API Key

- Check Q&A [Alternative to Google Geocoding API](https://www.udemy.com/course/understanding-typescript/learn/lecture/16936070#questions/8913424) about [Nominatim](http://nominatim.org/release-docs/latest/api/Search/)

* (171). Using Axios to Fetch Coordinates for an Entered Address

- Check Q&A [This API project is not authorized to use this API](https://www.udemy.com/course/understanding-typescript/learn/lecture/16936076#questions/12778327) ...enable also Geocoding API.
- [Status codes](https://developers.google.com/maps/documentation/geocoding/overview#StatusCodes)
  The "status" field within the Geocoding response object contains the status of the request, and may contain debugging information to help you track down why geocoding is not working.
- Check also on [Stackoverflow](https://stackoverflow.com/questions/38153734/do-i-need-to-hide-api-key-when-using-google-maps-js-api-if-so-how) about hiding api keys in index.html file.

* (172). Rendering a Map with Google Maps (incl. Types!)

- To show a map in the webpage go to: [JavaScript API](https://developers.google.com/maps/documentation/javascript/overview)

- google.maps... will be available globaly, because of new `<script defer async src="https://maps.googleapis.com/maps/api/js?key=API_KEY"></script>` we set in `index.html`, but TS doesn't know that. So we use `declare` like: `declare var google: any`

- To add a marker go to [Adding a Google Map with a Marker to Your Website](https://developers.google.com/maps/documentation/javascript/adding-a-google-map)

- To avoid typos in google code (e.g. map instead of maps: `new google.map.Map` instead of `new google.maps.Map`), use [@types/googlemaps](https://www.npmjs.com/package/@types/googlemaps). Now we don't even need to `declare var google: any`.

* Check also: [Working with Maps without a Credit Card](https://www.udemy.com/course/understanding-typescript/learn/lecture/16996108#content)

* These links might also be interesting:

- Google Maps Pricing: https://cloud.google.com/maps-platform/pricing/sheet/

- Google Geocoding API: https://developers.google.com/maps/documentation/geocoding/start

- Google Maps JS SDK: https://developers.google.com/maps/documentation/javascript/tutorial
