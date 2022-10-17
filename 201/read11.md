# Readings: Audio, Video, Images

## Video and Audio Content

1. The ability to use video and audio on the web has evolved since the early 2000s because the first influx of online videos and audio were made possible by proprietary plugin-based technologies like Flash and Silverlight. Both of them had security and accessibility issues, and are now obsolete, in favor of native HTML solutions **<video>** and **<audio>** elements.
2. **src** is used in the same way as for the <img> element. the src (source) attribute contains a path to the video you want to embed. It works in exactly the same way.
**controls** allows the user to be able to control video and audio playback (it's especially critical for people who have epilepsy.) At a minimum, the interface must include a way to start and stop the media, and to adjust the volume.
3. It is important to have **fallback content** inside the <video> element because it will be displayed if the browser accessing the page doesn't support the <video> element, allowing us to provide a fallback for older browsers.
4. *Audio and Video* were lost in the world, one would play visuals with no sound to compliment. The other would play sound with nothing to see. Until one day they meet and their abilities were a sight unseen! After that they never left each other's side for eternity.

## A Complete Guide To Grid

1. Grid's layout differs from Flex because Flex has one-directional flow whereas Grid does not.
2. A few Grid terms to be familiar with:

    - **Grid container:** The element on which display: grid is applied. It’s the direct parent of all the grid items. In this example container is the grid container.
    - **Grid item:** The children (i.e. direct descendants) of the grid container. Here the item elements are grid items, but sub-item isn’t.
    - **Grid line:** The dividing lines that make up the structure of the grid. They can be either vertical (“column grid lines”) or horizontal (“row grid lines”) and reside on either side of a row or column. Here the yellow line is an example of a column grid line.
    - **Grid Cell:** The space between two adjacent row and two adjacent column grid lines. It’s a single “unit” of the grid. Here’s the grid cell between row grid lines 1 and 2, and column grid lines 2 and 3.
    - **Grid Track:** The space between two adjacent grid lines. You can think of them as the columns or rows of the grid. Here’s the grid track between the second and third-row grid lines.
    - **Grid Area:** The total space surrounded by four grid lines. A grid area may be composed of any number of grid cells. Here’s the grid area between row grid lines 1 and 3, and column grid lines 1 and 3.

## Responsive Images

1. Developers should make images responsive because  Responsive image technologies were implemented recently to solve the problems of different screen sizes and resolutions by letting you offer the browser several image files, either all showing the same thing but containing different numbers of pixels (resolution switching), or different images suitable for different space allocations (art direction).
2. A few Responsive Image terms to be familiar with:

    - **<img>**: lets you point the browser to a single source file.
    - **srcset**: defines the set of images we will allow the browser to choose between, and what size each image is.
    - **sizes**: defines a set of media conditions (e.g. screen widths) and indicates what image size would be best to choose, when certain media conditions are true.
3. **srcset** more helpful for responsive images than CSS or JavaScript because when the browser starts to load a page, it starts to download (preload) any images before the main parser has started to load and interpret the page's CSS and JavaScript. That mechanism is useful in general for reducing page load times, but it is not helpful for responsive images — hence the need to implement solutions like srcset.

### Sources

- <https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Video_and_audio_content>
- <https://css-tricks.com/snippets/css/complete-guide-grid/>
- <https://developer.mozilla.org/en-US/docs/Learn/HTML/Multimedia_and_embedding/Responsive_images>

[Back To Home](../README.md)
