# poly-quick-image

[![Buy Me a Coffee](http://static.tonybogdanov.com/github/coffee.svg)](http://ko-fi.co/1236KUKJNC96B)

[Demo & Documentation](http://tonybogdanov.github.io/poly-quick-image/bower_components/poly-quick-image/index.html)

`<poly-quick-image>` uses `<iron-image>` to display a small placeholder (blurred) version of an image while the full
image loads in the background. The placeholder is generated in the browser using `<canvas>` if supported, then cached indefinitely with `localStorage`.

Inherently you can also use the element to display a `background-size:cover` image by setting `sizing="cover"` (formerly achieved with [poly-cover-image](https://github.com/TonyBogdanov/poly-cover-image)).

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

Then, go ahead and download the element's dependencies:

    bower install

## Playing With Your Element

If you wish to work on your element in isolation, it's recommended that you use
[Polyserve](https://github.com/PolymerLabs/polyserve) to keep your element's
bower dependencies in line. You can install it via:

    npm install -g polyserve

And you can run it via:

    polyserve

Once running, you can preview your element at `http://localhost:8080/components/poly-quick-image/`.