## Contribly AMP example

An AMP validated example of the Contribly contribute widget operating inside an AMP iframe.

[View the working example here.](http://contribly-amp-example.s3-website-eu-west-1.amazonaws.com/)

See the comments in [index.html](index.html) for an explanation of the design considerations.

The AMP iframe is using the Contribly contribute widget iframe wrapper to load the JavaScript contribute widget.
The wrapper registers a Contribly callback to receive notification when then form has loaded and rendered.
It then attempts to determine the height of the form before requesting an AMP iframe resize.

View the source of the [iframe wrapper](https://s3-eu-west-1.amazonaws.com/contribly-widgets/contribute/amp-iframe.html) to see how this achieved.
