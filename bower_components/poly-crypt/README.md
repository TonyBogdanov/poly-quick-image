# poly-crypt

[![Buy Me a Coffee](http://static.tonybogdanov.com/github/coffee.svg)](http://ko-fi.co/1236KUKJNC96B)

[Demo & Documentation](http://tonybogdanov.github.io/poly-crypt/bower_components/poly-crypt/index.html)

`<poly-crypt>` provides a family of cryptographic algorithms through a [Polymer](https://polymer-project.org) element.

## Dependencies

Element dependencies are managed via [Bower](http://bower.io/). You can
install that via:

    npm install -g bower

And init your project with:

    bower init

## Installation

Install the component with:

    bower install --save poly-crypt

## Playing With Your Element

If you wish to work on your element in isolation, it's recommended that you use
[Polyserve](https://github.com/PolymerLabs/polyserve) to keep your element's
bower dependencies in line. You can install it via:

    npm install -g polyserve

And you can run it via:

    polyserve

Once running, you can preview your element at `http://localhost:8080/components/poly-crypt/`.

## Example Usage

### Md5

    <poly-crypt auto algorithm="md5" input="Hello World"></poly-crypt>

Output will be: `b10a8db164e0754105b7a99be72e3fe5`

### Sha1

    <poly-crypt auto algorithm="sha1" input="Hello World"></poly-crypt>

Output will be: `0a4d55a8d778e5022fab701977c5d840bbc486d0`

### Base64 Encode

    <poly-crypt auto algorithm="base64encode" input="Hello World"></poly-crypt>

Output will be: `SGVsbG8gV29ybGQ=`

### Base64 Decode

    <poly-crypt auto algorithm="base64decode" input="SGVsbG8gV29ybGQ="></poly-crypt>

Output will be: `Hello World`

---

If you don't add the `auto` attribute, you must call `encrypt()` each time `input` and / or `algorithm` are changed to re-generate the `output`.