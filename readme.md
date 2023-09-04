# Responsive images

## Lighthouse issue - Image elements do not have explicit width and height

- when an image is inserted in the html as in the following from the index.html `<img src="./assets/image-hero.webp" alt="" class="img" />`, Lighthouse indicates that an `Image elements do not have explicit width and height`. A link for further details to the reasons why the sizes are important is given [Images without dimensions #](https://web.dev/optimize-cls/?utm_source=lighthouse&utm_medium=devtools#images-without-dimensions). The main reason behind this approach is to allow browsers to reserve the correct amount of space in the document whilst the image is loading
- the illustration is done using `display: flex` where the mobile has a column direction which is changed to row in medium to desktop.
![Mobile at 375px - lighthouse image without explicit sizes warning](screenshots/image-no-sizes.png)
![Mobile at 375px - img has no explicit sizes set - devtools open ](screenshots/mobile-showing-dimensions-no-sizes.png)
![Tablet at 900px - image has no explicit sizes](screenshots/tablet-dimensions-no-sizes.png)

![Mobile at 375px - image has explicit sizes ](screenshots/mobile-scr-sizes.png)
![Tablet at 900px - image has explicit sizes](screenshots/tablet-scr-sizes.png)
![Desktop - image has explicit sizes](screenshots/desktop-explicit-sizes.png)

![image without sizes video demostration](screenshots/image-without-sizes-edit.mp4)
![image with sizes video demo](screenshots/image-with-sizes-edit.mp4)
